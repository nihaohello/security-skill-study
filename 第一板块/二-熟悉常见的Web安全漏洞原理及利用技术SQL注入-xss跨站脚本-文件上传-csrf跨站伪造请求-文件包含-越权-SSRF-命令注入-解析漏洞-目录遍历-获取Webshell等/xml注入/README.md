#xml注入  
  
也就是我们常说的xxe  
  
原理：simplexml_load_string解析了我们的攻击代码  
  
形式：调用外部实体，监听vps，接受反弹数据  
可参考个人文章：http://www.youknowi.xin/2018/07/xxe%e6%94%bb%e5%87%bb/  
  
危害：读取敏感文件，ssrf  
  
预防：过滤符号（暂时未过多思考）  
  
  
  
