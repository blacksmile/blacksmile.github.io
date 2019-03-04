---
layout: post
title: "【System】XP和XP的远程桌面连接"
date: 2013-4-3 21:47
categories: 【办公软件应用】
tags:
- 远程桌面
- XP系统
---
XP和XP的远程桌面连接：  
1. 设置服务器和客服端的IP：  
![图片](http://a2.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/hKgwc.tjn*Qkq0VrW3B00imLkO8UOI252wdMJaYU2Gw!/b/dGZUxsHXDwAA&ek=1&kp=1&pt=0&bo=LAKdAQAAAAABAJU!&t=5&tl=3&su=014465905&tm=1551704400&sce=0-12-12&rf=2-9)  
![图片](http://a3.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/ZKsIRGTnO7yapxHuxDmCPmF5LueOa.eVOf0zNivjpvc!/b/dL1*87*VHQAA&ek=1&kp=1&pt=0&bo=KwKhAQAAAAABAK4!&t=5&tl=3&su=0236783201&tm=1551704400&sce=0-12-12&rf=2-9)  
设置完IP后，互相Ping下  
![图片](http://a4.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/ymHaCige0IdNtsTjnbZgjnIdyQ8HhMG3rfF9zALK99s!/b/dK8Sj8CrHgAA&ek=1&kp=1&pt=0&bo=KwKgAQAAAAABAK8!&t=5&tl=3&su=0105577233&tm=1551704400&sce=0-12-12&rf=2-9)  
![图片](http://a2.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/iUOfa0TxWpj1e.mQgKAupblD1lMAW*6a7nt9quPihuk!/b/dNXcWr.MMQAA&ek=1&kp=1&pt=0&bo=KQKiAQAAAAABAK8!&t=5&tl=3&su=0236251425&tm=1551704400&sce=0-12-12&rf=2-9)  
都可以通！  
2. 启用远程桌面  
![图片](http://a4.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/KX9M46hYW3.7Jc09frQ31UzpmLPtZ414VJSKV14Rd1M!/b/dFwEjMCXHgAA&ek=1&kp=1&pt=0&bo=KwKhAQAAAAABAK4!&t=5&tl=3&su=0206418577&tm=1551704400&sce=0-12-12&rf=2-9)  
![图片](http://a2.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/vb4bL9B*LOUNZKqW5bRl5pIAiZVknsZOCs5hSwlhqHU!/b/dMOxvsHcDwAA&ek=1&kp=1&pt=0&bo=LQKhAQAAAAABAKg!&t=5&tl=3&su=0108393761&tm=1551704400&sce=0-12-12&rf=2-9)  
检查下是否开启了远程桌面3389的端口，如果没有“我的电脑”右键→“服务”，把Remote Desktop开头的服务都开启。  
![图片](http://a1.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/307qX*uBRqte4JECwA3psbrBfRg4aX3*5RBjyXCxE3A!/b/dCg*LMH0FwAA&ek=1&kp=1&pt=0&bo=KwKgAQAAAAABAK8!&t=5&tl=3&su=026630769&tm=1551704400&sce=0-12-12&rf=2-9)  
![图片](http://a2.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/fbrnat64e*bGd8y5rS1HHrfZQgZX7Yl77d1mNiPYLkQ!/b/dPtXWb9pMQAA&ek=1&kp=1&pt=0&bo=KwKgAQAAAAABAK8!&t=5&tl=3&su=0202334225&tm=1551704400&sce=0-12-12&rf=2-9)  
3. 在服务器端添加个有密码的账户（或者是在公司里用的账户）  
![图片](http://a4.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/6XxdnfYZYRUqHFoeiI7HYLoa45.w1Q.uEPdDhwAA*w8!/b/dF.Kh8CzHgAA&ek=1&kp=1&pt=0&bo=KwKhAQAAAAABAK4!&t=5&tl=3&su=0145197713&tm=1551704400&sce=0-12-12&rf=2-9)  
4. 在服务器端里的远程桌面把这个账户添加  
![图片](http://a4.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/2zSz.ETa6PRfdFR3M2Au7lFDqQyjnWGY3Rbj3WIPcZw!/b/dJ21kMBcHgAA&ek=1&kp=1&pt=0&bo=KQKfAQAAAAABAJI!&t=5&tl=3&su=0182869905&tm=1551704400&sce=0-12-12&rf=2-9)  
5. 测试：在客户端上，“运行”输入MSTSC  
![图片](http://a3.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/md3IRmpqBCNRw3A8Q9ZUZr.rn8G4PjPcg36mUFw*OZE!/b/dLpl8L*uHQAA&ek=1&kp=1&pt=0&bo=KwKhAQAAAAABAK4!&t=5&tl=3&su=07832753&tm=1551704400&sce=0-12-12&rf=2-9)  
![图片](http://a1.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/Cu9YX.ozgDUiT9dXcFBrnJIUHa1z1xAQKmWPYtnEwSE!/b/dEHAJ8HzFwAA&ek=1&kp=1&pt=0&bo=KgKhAQAAAAABAK8!&t=5&tl=3&su=0115120929&tm=1551704400&sce=0-12-12&rf=2-9)  
![图片](http://a1.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/n1Fi11ioAwFDazOVXJJHe0.dUUPZDEGbX2UK7hyT.0Y!/b/dIS*LcH1FwAA&ek=1&kp=1&pt=0&bo=KgKeAQAAAAABAJA!&tl=3&su=0181439905&tm=1551704400&sce=0-12-12&rf=2-9)  
成功  
---
**其主要原因是“网络发现”所依赖的服务没有启用，或者被禁用；**  

>“网络发现”所依赖的服务如下：  
Function Discovery Resource Publication  
SSDP Discovery  
UPnP Device Host  
启动这三个服务后，“网络发现”就可以正常使用了；