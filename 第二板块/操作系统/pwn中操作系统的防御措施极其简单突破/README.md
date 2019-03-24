记录pwn中常见的几种情况

往往是配合漏洞进行利用的，这篇个人不进行实例结合，只做理论性的初步分析

有机会下篇介绍相关的实例
一.防护

参考：

http://tacxingxing.com/2017/07/14/relro/
https://blog.csdn.net/one_of_a_kind/article/details/84037586
https://www.cnblogs.com/Spider-spiders/p/8798628.html

利用checksec和gcc来说明保护措施

1.

gcc -m32 -no-pie -z execstack -fno-stack-protector -o demo1 demo.c

-m指定32位，

-no-pie 不启用地址随机化（也可系统层面：echo 0 > /proc/sys/kernel/randomize_va_space）

-z execstack 关掉栈保护

-fno-stack-protector 关掉DEP

root@kali:~/pwn/demo# checksec demo1
[*] '/root/pwn/demo/demo1'
    Arch:     i386-32-little
    RELRO:    Partial RELRO
    Stack:    No canary found
    NX:       NX disabled
    PIE:      No PIE (0x8048000)
    RWX:      Has RWX segments

2.

对比默认的

gcc demo.c -o demo2

root@kali:~/pwn/demo# checksec demo2
[*] '/root/pwn/demo/demo2'
    Arch:     amd64-64-little
    RELRO:    Partial RELRO
    Stack:    No canary found
    NX:       NX enabled
    PIE:      PIE enabled


个人kali中gcc默认没有堆栈保护 Stack: No canary found

且RELRO为Partial RELRO

3.

解决no canary found

-fstack-protector：
启用堆栈保护，不过只为局部变量中含有 char 数组的函数插入保护代码。
-fstack-protector-all：
启用堆栈保护，为所有函数插入保护代码。
-fno-stack-protector

gcc demo.c -fstack-protector -o demo3

root@kali:~/pwn/demo# checksec demo3
[*] ‘/root/pwn/demo/demo3’
Arch: amd64-64-little
RELRO: Partial RELRO
Stack: Canary found
NX: NX enabled
PIE: PIE enabled

4.

解决 Partial RELRO

gcc -z now -fstack-protector -o demo4 demo.c

root@kali:~/pwn/demo# checksec demo4
[*] ‘/root/pwn/demo/demo4’
Arch: amd64-64-little
RELRO: Full RELRO
Stack: Canary found
NX: NX enabled
PIE: PIE enabled

可以看到，全部开启

Full RELRO 保护got表不被修改，got是什么？存储函数全局地址的

Canary found 栈堆保护，标识符查看是否被溢出

NX enabled 开启DEP（数据不可执行保护）

PIE enabled 开启ALRS （地址随机化）
二.攻击与突破

就防御而言，来谈攻击与突破，再记录几种常见的思路

1.

三种方法突破canary防御

参考：https://www.baidu.com/baidu?wd=Canary+%E7%BB%95%E8%BF%87%E6%8A%80%E6%9C%AF&tn=monline_4_dg&ie=utf-8

（1）一种是 修改__stack_chk_fail函数在got表中的地址 （对应特定的情况，能修改got表）

__stack_chk_fail函数 是canary机制判定受到栈溢出的情况下，执行的函数

（2）另一种是泄露canary地址，最后再修改正确即可

（3）canary多进程程序爆破

2.

突破 Full RELRO

got表没有办法写

这种情况也不一定非要改写got表

ret2libc 技术

（1）其中有一种较简单的是，程序里直接有system之类的函数，只要我们能劫持ret到这个函数并执行即可

（2）还有一种在地址不变的情况下，得到系统system的地址

（3）在地址变的情况下，通过偏移得到system的地址

3.

突破 NX enabled

一旦开启，stack上的数据就不再可执行

原先只要有漏洞，直接一个shellcode过去就可以拿到shellcode，现在只有找system之类的执行函数了

和突破 Full RELRO 类似，不再赘述

4.

突破 PIE enabled

每次程序启动，其分配的地址变化

现在类似，找lib版本，程序里泄露函数地址，通过偏移找system地址

无法获得偏移的时候，关键在找gadgets地址突破



