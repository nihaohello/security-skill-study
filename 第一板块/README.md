人的惰性吧，第一版块，有部分是自己熟悉，也做过记录的，就没有怎么再次写  
第一板块：  
一.了解渗透测试的步骤、方法、流程、熟练掌握各种渗透测试工具。  
步骤：  
方法：端口扫描、系统指纹探测、服务漏洞扫描及利用、程序漏洞分析检测、Web攻击、弱点扫描及入侵部署防御和攻击分析追踪；  
流程：  
掌握各种工具:熟练使用WVS、burp suite、Sqlmap Nmap、Fiddler、Snort、Nessus、Metasploit，Kali Linux等常见安全测试工具  
二.  
熟悉常见的Web安全漏洞原理及利用技术（SQL注入、xss跨站脚本、文件上传、csrf跨站伪造请求、文件包含、越权、SSRF，命令注入，解析漏洞 目录遍历、获取Webshell等）；  
三.  
owasp top10  
  
  
  
├── 一-了解渗透测试的步骤-方法-流程-熟练掌握各种渗透测试工具  
│   ├── 了解渗透测试的步骤、方法、流程  
│   │   ├── 重点写出第二点信息收集  
│   │   │   ├── 信息收集.pdf  
│   │   │   └── README.md  
│   │   ├── 重点写出第三点漏洞探索  
│   │   │   ├── 漏洞探索.pdf  
│   │   │   └── README.md  
│   │   └── README.md  
│   ├── 掌握各种工具熟练使用WVS、burp suite、Sqlmap Nmap、Fiddler、Snort、Nessus、Metasploit，Kali Linux等常见安全测试工具  
│   │   ├── burp suite  
│   │   │   └── README.md  
│   │   ├── Kali Linux  
│   │   │   └── README.md  
│   │   ├── Metasploit  
│   │   │   └── README.md  
│   │   ├── nmap  
│   │   │   ├── nmap基础操作.pdf  
│   │   │   ├── nmap脚本.pdf  
│   │   │   └── README.md  
│   │   ├── README.md  
│   │   └── sqlmap  
│   │       ├── README.md  
│   │       ├── sqlmap基础操作.pdf  
│   │       └── sqlmap脚本.pdf  
│   └── README.md  
└── README.md  
├── 二-熟悉常见的Web安全漏洞原理及利用技术SQL注入-xss跨站脚本-文件上传-csrf跨站伪造请求-文件包含-越权-SSRF-命令注入-解析漏洞-目录遍历-获取Webshell等  
│   ├── 反序列化漏洞  
│   │   ├── Java反序列化漏洞.pdf  
│   │   ├── Java反序列化漏洞poc进阶.docx  
│   │   ├── php反序列化漏洞.pdf  
│   │   └── README.md  
│   ├── 劫持  
│   │   └── README.md  
│   ├── 逻辑漏洞  
│   │   └── README.md  
│   ├── 文件上传  
│   │   └── README.md  
│   ├── csrf  
│   │   ├── README.md  
│   │   └── xss+csrf.pdf  
│   ├── README.md  
│   ├── sql  
│   │   ├── 反序列化注入  
│   │   │   └── README.md  
│   │   ├── 框架注入  
│   │   │   └── README.md  
│   │   ├── 命令注入  
│   │   │   └── README.md  
│   │   ├── 数据库注入  
│   │   │   ├── 数据库注入的类似点  
│   │   │   │   ├── 报错注入.pdf  
│   │   │   │   ├── 个人以前学习关于mysql注入的随笔.zip  
│   │   │   │   ├── 联合注入.pdf  
│   │   │   │   ├── 时间盲注.pdf  
│   │   │   │   ├── bool盲注.pdf  
│   │   │   │   └── README.md  
│   │   │   ├── access注入.pdf  
│   │   │   ├── mysql注入.pdf  
│   │   │   ├── oracle注入.pdf  
│   │   │   ├── README.md  
│   │   │   ├── sqlite注入.pdf  
│   │   │   └── sql_server注入.pdf  
│   │   ├── 组件注入  
│   │   │   └── README.md  
│   │   └── README.md  
│   ├── ssrf  
│   │   └── README.md  
│   ├── xml注入  
│   │   ├── README.md  
│   │   ├── xml基础以及攻击防御.pdf  
│   │   └── xxe攻击.pdf  
│   └── xss  
│       ├── 作者如何利用xss漏洞shua盒子rank的.pdf  
│       ├── README.md  
│       ├── xss基础攻击与防御.pdf  
│       └── xss+csrf.pdf  
├── 三-owasp-top10  
│   ├── Broken AccessControl  
│   │   └── README.md  
│   ├── Broken Authentication  
│   │   └── README.md  
│   ├── Cross-SiteScripting  
│   │   ├── 作者如何利用xss漏洞shua盒子rank的.pdf  
│   │   ├── README.md  
│   │   ├── xss基础攻击与防御.pdf  
│   │   └── xss+csrf.pdf  
│   ├── Injection  
│   │   ├── 反序列化注入  
│   │   │   └── README.md  
│   │   ├── 框架注入  
│   │   │   └── README.md  
│   │   ├── 命令注入  
│   │   │   └── README.md  
│   │   ├── 数据库注入  
│   │   │   ├── 数据库注入的类似点  
│   │   │   │   ├── 报错注入.pdf  
│   │   │   │   ├── 个人以前学习关于mysql注入的随笔.zip  
│   │   │   │   ├── 联合注入.pdf  
│   │   │   │   ├── 时间盲注.pdf  
│   │   │   │   ├── bool盲注.pdf  
│   │   │   │   └── README.md  
│   │   │   ├── access注入.pdf  
│   │   │   ├── mysql注入.pdf  
│   │   │   ├── oracle注入.pdf  
│   │   │   ├── README.md  
│   │   │   ├── sqlite注入.pdf  
│   │   │   └── sql_server注入.pdf  
│   │   ├── 组件注入  
│   │   │   └── README.md  
│   │   └── README.md  
│   ├── Insecure Deserialization  
│   │   ├── Java反序列化漏洞.pdf  
│   │   ├── Java反序列化漏洞poc进阶.docx  
│   │   ├── php反序列化漏洞.pdf  
│   │   └── README.md  
│   ├── README.md  
│   ├── Security Misconfiguration  
│   │   └── README.md  
│   ├── Sensitive DataExposure  
│   │   └── README.md  
│   ├── UsingComponents with Known Vulnerabilities  
│   │   └── README.md  
│   └── XML ExternalEntities  
│       ├── README.md  
│       ├── xml基础以及攻击防御.pdf  
│       └── xxe攻击.pdf  
