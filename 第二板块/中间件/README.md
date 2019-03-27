1.  
什么是中间件：解决一些通用麻烦的问题，趋于模块化  
百度百科：https://baike.baidu.com/item/%E4%B8%AD%E9%97%B4%E4%BB%B6/452240?fr=aladdin  
web服务器:  
web服务器用于提供http服务，即向客户端返回信息，其可以处理HTTP协议，响应针对静态页面或图片的请求，控制页面跳转，或者把动态请求委托其它程序（中间件程序）等。  
web中间件:  
web中间件用于提供系统软件和应用软件之间的连接，以便于软件各部件之间的沟通，其可以为一种或多种应用程序提供容器。  
web容器:  
web容器用于给处于其中的应用程序组件（JSP，SERVLET）提供一个环境，是中间件的一个组成部分，它实现了对动态语言的解析。比如tomcat可以解析jsp，是因为其内部有一个jsp容器。  
  
  
  
2.常见的web中间件极其漏洞  
参考：  
https://www.cnblogs.com/qmfsun/p/4055627.html  
https://blog.csdn.net/u012114090/article/details/80611456（WEB服务器和中间件）  
https://blog.csdn.net/leizi191110211/article/details/51594039  
https://github.com/99bt/F-MiddlewareScan（扫描脚本，更新于3年前）  
https://www.360zhijia.com/anquan/433223.html  （相应漏洞极其演示）  
https://www.chainnews.com/articles/163141368429.htm（详细的）  
http://www.mchz.com.cn/cn/service/Safety-Lab/info_26_itemid_2068.html（iis相关的）  
https://www.cnblogs.com/sunshineyan/p/8954532.html（iis相关的）  
https://blog.csdn.net/wizardforcel/article/details/60957024 (较详细的)  
https://blog.csdn.net/qq_29647709/article/details/81946976（较详细的）  
https://www.freebuf.com/articles/web/192063.html（相应漏洞极其演示）  
https://blog.csdn.net/fly_hps/article/details/80781925（web服务器与中间件）  
  
  
一、 常见 web 中间件及其漏洞概述  
（一） IIS  
1、PUT 漏洞  
2、短文件名猜解  
3、远程代码执行  
4、解析漏洞  
（二） Apache  
1、解析漏洞  
2、目录遍历  
（三） Nginx  
1、文件解析  
2、目录遍历  
3、CRLF 注入  
4、目录穿越  
（四） Tomcat  
1、远程代码执行  
2、war 后门文件部署  
3.弱口令  
（五） jBoss  
1、反序列化漏洞  
http://www.youknowi.xin/?s=jboss  
2、war 后门文件部署  
（六） WebLogic  
1、反序列化漏洞  
2、SSRF  
3、任意文件上传  
4、war 后门文件部署  
（七）其它中间件相关漏洞  
1、FastCGI 未授权访问、任意命令执行  
2、PHPCGI 远程代码执行（此漏洞影响 php-5.3.12 以前的版本，mod 方式、fpm 方式不受影响）  
(八)struts2  
也是一个比较多漏洞的点  
命令执行  
（九）spring  
反序列化命令执行  
  
