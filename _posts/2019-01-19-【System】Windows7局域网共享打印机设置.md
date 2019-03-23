---
layout: post
title: "【System】Windows7局域网共享打印机设置"
date: 2019-01-19 19:48
categories: 【System】
tags:
- Windows 7打印机共享设置
---
Windows7局域网共享打印机设置分两步：  
（不同运营商和不同网段可以利用无线路由器组成局域网进行打印机共享）  

①目标打印机设置（关闭密码保护共享和启动Guest用户、共享打印机选项设置）  
②在其它计算机上添加目标打印机  
**`注意事项：`**  
**`1.路由器或光钎猫接口`**  
**`2.网络状态是否相同`**  
**`3.防火墙`**  
**`4.关于共享之类的设置是否恰当`**  


**一、关闭密码保护共享和启用Guest用户**  
1、开启“网络和共享中心”，选中“更改高级共享设置”。  
2、在“启用网络发现”和“启用文件和打印机共享”前勾选，再保存。  
3、在“密码保护的共享”-“关闭密码保护共享”。  
4、右击“计算机图标”——选择“管理”  
![](http://a4.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/qrhdY.z*frSfFcuZrjiIDj6QRT0OmLzM5dgCvCQT*Ok!/b/dL8AAAAAAAAA&ek=1&kp=1&pt=0&bo=KgIzAQAAAAADEC8!&tl=1&su=0132571249&tm=1553306400&sce=0-12-12&rf=2-9)  

5、在“本地用户和组”中找到“用户”，再找到“Guset”  
![](http://a2.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/VLuy0cxylxbqriNzVZSeDvhCzIUo2payFKxMO53yTeI!/b/dDEBAAAAAAAA&ek=1&kp=1&pt=0&bo=gQJJAQAAAAADEP4!&tl=1&su=0237801057&tm=1553306400&sce=0-12-12&rf=2-9)  

6、右击“Guest”——选择属性——把“账户已禁用”前的勾去掉，点击确定  
![](http://a3.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/lLYHzgeyEZ6lrgIcthh1vq.hlHh2F.XawGKK*wdTBFU!/b/dL4AAAAAAAAA&ek=1&kp=1&pt=0&bo=KgLlAQAAAAADEPk!&tl=1&su=0259013153&tm=1553306400&sce=0-12-12&rf=2-9)  

**目标打印机共享设置（如果同时需要给32、64为系统做共享打印机，两个版本驱动都需要安装）**  
7、“开始”—选择“设备和打印机”  
![](http://a4.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/YjD00Fy.mnyOzarXeco2PEgA6uNv.afiJi4ZMAeMWU0!/b/dFMBAAAAAAAA&ek=1&kp=1&pt=0&bo=mAEAAgAAAAADEK4!&tl=1&su=0148658705&tm=1553306400&sce=0-12-12&rf=2-9)  

8、选中目标打印机（前提是打印机已正确安装），单击鼠标右键打开菜单，选择“打印机属性”  
![](http://a4.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/y8ZQgzXNFqCZIV5pGSAc7TyrwLVcgsqngLjHg7WRJqU!/b/dDcBAAAAAAAA&ek=1&kp=1&pt=0&bo=KgLhAQAAAAADIM0!&tl=1&su=090298161&tm=1553306400&sce=0-12-12&rf=2-9)  

9、 选择“共享”选项卡，选中“共享这台打印机”并设置共享名，然后确定。  
![](http://a3.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/QJPuEfgfHgYDUNoMbpSxSK6fubcZtlA7sdfBTrdUdMM!/b/dL4AAAAAAAAA&ek=1&kp=1&pt=0&bo=KgLdAQAAAAADEME!&tl=1&su=0190120097&tm=1553306400&sce=0-12-12&rf=2-9)  

**二、在其它计算机添加目标打印机**  

1、 打开“资源管理器”，在地址栏输入\共享打印机的IP地址， 例如：\\192.168.1.4  
![](http://a3.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/uQX508UBl1Arns.LvOk05qIFReBZsKsh8Le9P0WH.gw!/b/dL4AAAAAAAAA&ek=1&kp=1&pt=0&bo=KgIdAQAAAAADEAE!&tl=1&su=0122010721&tm=1553306400&sce=0-12-12&rf=2-9)  

注：有些 XP 系统可能一些策略没有打开，会出现不能正常访问的情况，可试着做如下的处理：  
1） 在组策略中设置，安全策略。开始--运行--gpedit.msc--计算机配置--windows 设置--安全设置--本地策略--“用户权力指派”，双击右边的“从网络访问此计算机”，保证其中有 Everyone， 再双击左边的“拒绝从网络访问此计算机”，保证其是空的。  
2）选择左边的“本地策略”-“安全选项”  
a.确认右边的“网络访问：本地帐户的共享与安全模式”为“经典”；  
b.确认右边的“ Microsoft 网络客户：为通讯启用数字签名（总是）”为“已停用”；  
c.确认右边的“ Microsoft 网络客户：为通讯启用数字签名（如果服务器允许）”为“已启用”；  
d.确认右边的“ Microsoft 网络服务器：为通讯启用数字签名（总是）”为“已停用”；  
e.确认右边的“ Microsoft 网络服务器：为通讯启用数字签名（如果服务器允许）”为“已启用”。  

2、 选中共享打印机， 单击鼠标右键打开快显菜单，选择“连接”， 进行安装。  
![](http://a3.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/ayJ4fOKYcjYwlh1YVUqSrAWyLLzPswXgmld00CDNGcM!/b/dL4AAAAAAAAA&ek=1&kp=1&pt=0&bo=KgJwAQAAAAADEGw!&tl=1&su=058591153&tm=1553306400&sce=0-12-12&rf=2-9)  

3、“控制面板”-“硬件和声音”-“设备和打印机”，选择刚装好的打印机， 单击鼠标右键，选择“打印机属性”，单击“打印测试页”， 正常打印， 说明安装成功。  
![](http://a1.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/J3nyNT1V6qjpGNTlefQDWjAQaFpjPRNMGZcQ9QCcu2g!/b/dFQBAAAAAAAA&ek=1&kp=1&pt=0&bo=JAISAgAAAAADEAM!&tl=1&su=078400817&tm=1553306400&sce=0-12-12&rf=2-9)  
![](http://a4.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/*zyOXddAGWu6.3kjM2QLw3df1AMjHaim5VT*nACptO4!/b/dL8AAAAAAAAA&ek=1&kp=1&pt=0&bo=KgLaAQAAAAADEMY!&tl=1&su=091155473&tm=1553306400&sce=0-12-12&rf=2-9)  