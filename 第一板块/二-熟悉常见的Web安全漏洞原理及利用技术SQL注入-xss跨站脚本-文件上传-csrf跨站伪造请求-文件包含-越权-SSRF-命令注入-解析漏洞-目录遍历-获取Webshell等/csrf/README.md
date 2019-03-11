#csrf  
  
原理：个人理解即盗用cookies模拟用户操作  
  
形式：get操作 post表单  
  
危害：危害用户账户  
  
预防：限定referer，token设置  
  
提升：  
这里利用xss，来获取token，获取cookie，突破referer限制和token限制  
  
  
  
