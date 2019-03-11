#文件上传  
  
原理：个人理解即借助一些操作达到解析webshell的目的  
  
形式：php5.3.4之前的截断，Nginx，apache，IIS的解析漏洞，大小写双写绕过过滤，windows下的系统特性，gif头特性绕过，条件竞争绕过  
参考：  
https://github.com/LandGrey/upload-labs-writeup  
http://www.youknowi.xin/2018/10/%e6%96%87%e4%bb%b6%e4%b8%8a%e4%bc%a0%e7%9a%84%e5%a7%bf%e5%8a%bf/  
http://www.youknowi.xin/2019/01/%e5%8f%a6%e7%b1%bb%e7%9a%84%e4%b8%8a%e4%bc%a0%e7%bb%95%e8%bf%87waf%ef%bc%88%e8%bd%ac%e8%bd%bd%ef%bc%89/  
  
危害：直接获取webshell，然后呢  
  
预防：  
1.更新版本  
2.彻底：白名单+重命名+上传目录（限制执行权限），当然配合其他漏洞另说  
  
  
  
