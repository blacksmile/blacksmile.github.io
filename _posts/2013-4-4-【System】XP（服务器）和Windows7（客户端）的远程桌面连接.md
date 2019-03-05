---
layout: post
title: "【System】XP（服务器）和Windows7（客户端）的远程桌面连接"
date: 2013-4-4 15:18
categories: 【System】
tags:
- XP系统
- Win 7系统
- 远程桌面
---
XP（服务器）和Windows7（客户端）的远程桌面连接：  
1. 设置服务器和客服端的IP：  
![](http://a1.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/b3IGWtrRBEU9mSPuo4PBl6ClesfMmV0WyO1Pg55YsHg!/b/dKjixr5*MQAA&ek=1&kp=1&pt=0&bo=KwKeAQAAAAABAJE!&t=5&tl=3&su=0124164129&tm=1551704400&sce=0-12-12&rf=2-9)  
![](http://a2.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/mE1qAChHnpgygUlhompmPu0A.TNOG40dhZcQar1k9S0!/b/dNXIu8EFEAAA&ek=1&kp=1&pt=0&bo=KgKgAQAAAAABAK4!&t=5&tl=3&su=015050417&tm=1551704400&sce=0-12-12&rf=2-9)  

<!-- more -->

设置完IP后，互相Ping下  
![](http://a2.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/3QtbrkPkG3U.kty31JYTDblZ7KVxZmldZ5M.QqJfuXA!/b/dKFpXL9KMAAA&ek=1&kp=1&pt=0&bo=IANYAgAAAAABAF4!&t=5&tl=3&su=0182224193&tm=1551704400&sce=0-12-12&rf=2-9)  
![](http://a1.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/pTTayfeKyEHU7ngU69ueeo0pciT3CuxNgPMykPKuHYM!/b/dETjw77TMQAA&ek=1&kp=1&pt=0&bo=IANYAgAAAAABAF4!&t=5&tl=3&su=0219914929&tm=1551704400&sce=0-12-12&rf=2-9)  
都可以通！  
Ping 不通其主要原因是Windows7“网络发现”所依赖的服务没有启用，或者被禁用；  
“网络发现”所依赖的服务如下：  
Function Discovery Resource Publication  
SSDP Discovery  
UPnP Device Host  
启动这三个服务后，“网络发现”就可以正常使用了；（“计算机”右键“管理”或者“服务”里）  
![](http://a4.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/PPA6JPjlN1v0NEdRJ49oQwYn8Hmz4VmcBn3UJ9ZzXRE!/b/dDEulcC.HgAA&ek=1&kp=1&pt=0&bo=IANYAgAAAAABAF4!&t=5&tl=3&su=085814001&tm=1551704400&sce=0-12-12&rf=2-9)  
2. 启用远程桌面  
![](http://a2.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/G1Z4crkz89nJDT3oWIqqFfvpQ6Nl938cmVMOqoCQFk0!/b/dL3XV7*CMQAA&ek=1&kp=1&pt=0&bo=KwKfAQAAAAABAJA!&t=5&tl=3&su=0267994641&tm=1551704400&sce=0-12-12&rf=2-9)  
![](http://a2.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/s5Ljgq.4VWiNQZv2Bg.czHcXT83Arm6vt7F*s2h6f3E!/b/dHxQw8EDEAAA&ek=1&kp=1&pt=0&bo=IANYAgAAAAABAF4!&t=5&tl=3&su=08215249&tm=1551704400&sce=0-12-12&rf=2-9)  
查下是否开启了远程桌面3389的端口，如果没有“我的电脑”右键→“服务”，把Remote Desktop开头的服务都开启。  
![](http://a1.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/PTp*VEZ3NU8mc31CGRG.Tnhj8*feTUAVe9PH5bLlYkw!/b/dP3RLcEZGAAA&ek=1&kp=1&pt=0&bo=LAKgAQAAAAABAKg!&t=5&tl=3&su=0240337313&tm=1551704400&sce=0-12-12&rf=2-9)  
![](http://a3.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/5hTDJB*Ox5d5Poa19306dez9HhmXABNQxbx*Mnx*tY0!/b/dAUQ.L.YHgAA&ek=1&kp=1&pt=0&bo=IANYAgAAAAABAF4!&t=5&tl=3&su=0212824801&tm=1551704400&sce=0-12-12&rf=2-9)  
3. 在服务器端添加个有密码的账户（或者是在公司里用的账户）  
![](http://a1.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/kdrLtd.PQA3olssmn5Ht6zILmkA9Lh8QpqOz5FJQ.0w!/b/dC2.vb7tMQAA&ek=1&kp=1&pt=0&bo=KwKfAQAAAAABAJA!&t=5&tl=3&su=0109799681&tm=1551704400&sce=0-12-12&rf=2-9)  
4. 在服务器端里的远程桌面把这个账户添加  
![](http://a2.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/y652UeTdVsymfjWP3Gu6lbzP.4phMZtzpwIoXvz5kdo!/b/dK5vXL*kLwAA&ek=1&kp=1&pt=0&bo=KwKfAQAAAAABAJA!&t=5&tl=3&su=088265745&tm=1551704400&sce=0-12-12&rf=2-9)  
5. 测试：在客户端上，“运行”输入MSTSC  
![](http://a4.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/yfQ.Uin0viOiIm1RDbsR2HQ99qlTVHFWrdOC2mWsr6Q!/b/dEkMj8CTHgAA&ek=1&kp=1&pt=0&bo=IANYAgAAAAABAF4!&t=5&tl=3&su=0187646097&tm=1551704400&sce=0-12-12&rf=2-9)  
![](http://a4.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/baDGAhBrnCBMsjbpdbnPiDYkXm6G.CMo3loRtXH7TrI!/b/dM4vj8CaHgAA&ek=1&kp=1&pt=0&bo=IANYAgAAAAABAF4!&t=5&tl=3&su=050283649&tm=1551704400&sce=0-12-12&rf=2-9)  
![](http://a1.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/XYCo5UMRD4RMZqa*7Mh9w4YA.Br.vKnKebpEqmkooX4!/b/dCRsxb7RMQAA&ek=1&kp=1&pt=0&bo=IANYAgAAAAABAF4!&tl=3&su=04141585&tm=1551704400&sce=0-12-12&rf=2-9)  
成功