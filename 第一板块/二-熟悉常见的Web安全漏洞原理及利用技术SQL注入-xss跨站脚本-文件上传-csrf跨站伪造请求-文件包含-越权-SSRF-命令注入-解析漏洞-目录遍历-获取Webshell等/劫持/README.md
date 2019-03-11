#劫持  
  
原理：即登陆接口存在csrf，导致数据泄露和跳转的导向劫持  
  
形式：利用csrf结合xss伪造referer，获取cookies，利用jsonp接口导致数据的泄露  
  
危害：数据泄露，用户账户受损  
  
预防：httponly，token，referer，验证的唯一性（输入原密码等）  
  
  
  
  
