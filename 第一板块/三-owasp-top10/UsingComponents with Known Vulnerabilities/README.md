#使用已知漏洞组件  
这也是最轻松的利用，利用现成的工具，poc，exp进行利用  
所以，对于框架组件漏洞，个人而言一直都是用到什么去搜索什么  
  
其实框架而言，本身基本是安全的，不安全是偶尔爆一些安全问题，以及开发人员关闭了安全防护，或者代码逻辑存在问题  
  
  
PHP：  
php 开发框架：http://baijiahao.baidu.com/s?id=1604870874054619554&wfr=spider&for=pc  
zendframwork 搜到的最新漏洞是13年的  参考：https://www.linuxidc.com/Linux/2013-03/80620.htm  
Yii  一个sql：https://www.anquanke.com/vul/id/1127885   一个文件上传：https://blog.csdn.net/m0_37645820/article/details/73747155  
CakePHP  最新漏洞没有搜索到  
Symfony   与Drupal这款cms 远程代码执行  参考：https://www.4hou.com/vulnerable/12904.html  https://www.4hou.com/vulnerable/12904.html  
Thinkphp  2018 远程代码执行  
CodeIgniter  2016年任意代码执行  
CanPHP   2012年sql漏洞  
Laravel  16年17年远程代码执行  19年PHP框架Lavarel被发现存在高危漏洞：https://www.leiphone.com/news/201901/vd9cN3CO3igneBzx.html  
SlimFramework   16年 xxe漏洞  
SpeedPHP 参考：SpeedPHP一次简单渗透：https://www.xiaoxiaowu.me/web/1802.html  
  
  
Java：  
Java 开发框架：https://blog.csdn.net/shenshaoqiu/article/details/78650613  
常用的就是前面三个（个人猜的）  
后面的用到再搜索  
struts2 听闻只维护老项目了 常用工具有windows下以及github上的struts2脚本扫描  
spring mvc  2018年目录穿越漏洞 https://paper.seebug.org/665/  
Hibernate   16年的注入，18年的反序列化：https://xz.aliyun.com/t/2031 and http://www.codersec.net/2018/01/java%E5%8F%8D%E5%BA%8F%E5%88%97%E5%8C%96%E6%BC%8F%E6%B4%9E-%E9%87%91%E8%9B%87%E5%89%91%E4%B9%8Bhibernate(%E4%B8%8A)/  
JSF  
Vaadin  
Google Web Toolkit  
Grails  
Mybatis  
Dubbo  
Maven  
RabbitMQ  
Log4j  
redis  
shiro  
  
  
  
python：  
python 开发框架： https://www.cnblogs.com/suzhigang/p/6208244.html  https://www.cnblogs.com/shaosks/p/7237809.html  https://baijiahao.baidu.com/s?id=1610038438439925424&wfr=spider&for=pc  
django  
flask  
web2py  
webpy  
scrapy  
tornado  
bottle  
pylons  
  
  
  
  
web应用服务器  
参考：https://www.cnblogs.com/vipyoumay/archive/2017/08/31/7455431.html（https://www.cnblogs.com/vipyoumay/archive/2017/08/31/7455431.html）  
weblogic  
J2EE  
jboss  
Glassfish  
Apache Tomcat  
Apache Geronimo  
  
  
  
  
各大容器的解析漏洞  
  
  
  
  
