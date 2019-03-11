#owasp  
参考：  
https://www.owasp.org/index.php/Top_10-2017_Top_10  
https://blog.sucuri.net/2018/10/owasp-top-10-security-risks-part-i.html  
  
  
1.Injection  
起因：包含各种数据库和各种语言的注入  
防御：  
2.Broken Authentication  
包含认证的逻辑和暴力破解  
3.Sensitive data exposure  
起因：敏感数据暴露  
防御：  
4.XML External Entities (XXE)  
起因：xml外部实体，许多较旧或配置不当的XML处理器评估XML文档中的外部实体引用。外部实体可用于使用文件URI处理程序，内部文件共享，内部端口扫描，远程代码执行和拒绝服务攻击来公开内部文件。  
  
5.Broken Access control  
解释起来像越权  
起因：对经过身份验证的用户的限制通常不会得到严格执行。攻击者可以利用这些漏洞访问未经授权的功能和/或数据，例如访问其他用户的帐户，查看敏感文件，修改其他用户的数据，更改访问权限等。  
  
  
6.Security misconfigurations  
安全配置  
  
7.Cross Site Scripting (XSS)  
xss  
  
8.Insecure Deserialization  
反序列化攻击  
  
  
9.Using Components with known vulnerabilities  
通过已知组件进行漏洞利用  
  
  
10.Insufficient logging and monitoring  
记录和监控问题  
  
