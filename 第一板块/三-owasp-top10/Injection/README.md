#sql  
  
原理：sql注入的个人理解就是拼接了sql语句  
  
形式：sqlmap中有几个注入形式，TUBE    T是时间   U是联合   B是bool      E是报错  
  
危害：拖库，写马  
  
预防：不让它拼接sql语句  
黑名单，即过滤替换敏感词汇，早先预防的操作  
预参数化，即把输入当作内容，不再参与拼接sql语句  
  
sql注入常出现的地方：  
一切入库操作  
get参数，id查询的地方等  
post参数，登陆框，留言板等  
为什么可能会有接下来三个，防止一些其他危险操作，xss，csrf等  
cookies参数入库  
refer参数入库  
user-agent参数入库  
  
  
  
  
#Injection  
  
常见的注入，以及对应的预防方法  
  
  
数据库注入：  
mysql注入  
oracle注入  
sql server注入  
access注入  
sqlite注入  
  
  
  
框架注入：  
java：  
spring框架注入  
struts2框架注入  
python：  
django框架注入  
php：  
thinkphp框架注入  
asp：  
  
  
  
  
os shell 注入：  
  
  
  
  
组件注入：  
  
  
  
  
反序列化注入：  
  
  
  
  
  
  
