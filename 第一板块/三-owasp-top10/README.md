#owasp  
参考：  
https://www.owasp.org/index.php/Top_10-2017_Top_10  
https://blog.sucuri.net/2018/10/owasp-top-10-security-risks-part-i.html  
https://www.cnblogs.com/cn-36/p/6723536.html（不错的）  
https://blog.csdn.net/john1337/article/details/70313886  （其中的举例很棒）  
http://www.cnblogs.com/shellr00t/p/6774267.html  
https://blog.csdn.net/sweetfire/article/details/78616438  
https://www.freebuf.com/articles/web/155145.html   不错  
  
  
  
跨站请求伪造’和‘未经验证的重定向和转发  
owasp 13年  
1.injection  
2.Broken Authentication and session management  
3.cross-site scripting(xss)  
4.insecure direct object references  
5.security-misconfigurations  
6.sensitive data exposure  
7.misssing function level access contr  
8.cross-site request forgery(csrf)  
9.using components with known vulnerabilities  
10.unvalidataed redirects and forwords  
  
4（不安全的直接对象引用） and 7（应用层访问控制缺失） 合并为==》  5（中断访问控制）  
delete（删除） 8（csrf） and 10（未经验证的重定向和转发）  
  
owasp 17年  
1.Injection  
2.Broken Authentication  
3.Sensitive DataExposure  
4.XML ExternalEntities  
5.Broken AccessControl  
6.Security Misconfiguration  
7.Cross-SiteScripting  
8.Insecure Deserialization  
9.UsingComponents with Known Vulnerabilities  
10.InsufficientLogging & Monitoring  
  
  
  
推荐靶机平台bwapp  
参考：http://www.youknowi.xin/?s=bwapp  
  
  
.  
├── Broken AccessControl  
│   └── README.md  
├── Broken Authentication  
│   └── README.md  
├── Cross-SiteScripting  
│   ├── 作者如何利用xss漏洞shua盒子rank的.pdf  
│   ├── README.md  
│   ├── xss基础攻击与防御.pdf  
│   └── xss+csrf.pdf  
├── Injection  
│   ├── 反序列化注入  
│   │   └── README.md  
│   ├── 框架注入  
│   │   └── README.md  
│   ├── 命令注入  
│   │   └── README.md  
│   ├── 数据库注入  
│   │   ├── 数据库注入的类似点  
│   │   │   ├── 报错注入.pdf  
│   │   │   ├── 个人以前学习关于mysql注入的随笔.zip  
│   │   │   ├── 联合注入.pdf  
│   │   │   ├── 时间盲注.pdf  
│   │   │   ├── bool盲注.pdf  
│   │   │   └── README.md  
│   │   ├── access注入.pdf  
│   │   ├── mysql注入.pdf  
│   │   ├── oracle注入.pdf  
│   │   ├── README.md  
│   │   ├── sqlite注入.pdf  
│   │   └── sql_server注入.pdf  
│   ├── 组件注入  
│   │   └── README.md  
│   └── README.md  
├── Insecure Deserialization  
│   ├── Java反序列化漏洞.pdf  
│   ├── Java反序列化漏洞poc进阶.docx  
│   ├── php反序列化漏洞.pdf  
│   └── README.md  
├── README.md  
├── Security Misconfiguration  
│   └── README.md  
├── Sensitive DataExposure  
│   └── README.md  
├── UsingComponents with Known Vulnerabilities  
│   └── README.md  
└── XML ExternalEntities  
├── README.md  
├── xml基础以及攻击防御.pdf  
└── xxe攻击.pdf  
  
