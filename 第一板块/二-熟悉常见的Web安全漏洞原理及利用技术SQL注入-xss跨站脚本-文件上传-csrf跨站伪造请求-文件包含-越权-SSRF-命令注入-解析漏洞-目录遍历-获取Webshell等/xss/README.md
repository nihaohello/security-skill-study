#跨站脚本攻击  
  
即xss，常配合csrf  
1.xss攻击和基础，大概记录了初级的攻击利用，防御  
2.作者如何利用xss漏洞shua盒子rank的文档是个人的一篇的平台投稿  
3.计划再简单记录一篇xss和csrf的记录  
4.更多的xss技术性分析，大概会放在各大浏览器学习主题进行深入  
  
  
原理：个人理解是拼接了js，html代码  
形式：xsser.me平台，beef xss平台，xss蠕虫  
危害：主流两种，盗取cookies，组合csrf  
预防：htmlspecialchars() 函数把预定义的字符转换为 HTML 实体（注意第二个参数）  
  
  
