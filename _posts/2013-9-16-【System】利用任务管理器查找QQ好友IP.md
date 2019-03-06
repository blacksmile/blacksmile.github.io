---
layout: post
title: "【System】利用任务管理器查找QQ好友IP"
date: 2013-9-16 08:31
categories: 【System】
tags:
- 任务管理器
- QQ
---
有一些第三方版本的QQ或者插件可以显示好友IP地址，但Windows7系统自带的资源监视器中，就能很方便的看到QQ好友的IP地址。  
1、首先，打开“任务管理器”，然后在“性能”标签中点击“资源监视器”。  
![](http://a3.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/rjbjGUTshFQW*ZWcaLKMP5aIrOPGDaOBV8WkhLm2SLQ!/b/dHqgtsShAgAA&ek=1&kp=1&pt=0&bo=oAGrAQAAAAADAC4!&tl=1&su=084873617&tm=1551880800&sce=0-12-12&rf=2-9)  

<!-- more -->

2、打开资源监视器，切换到“网络”标签，然后在“网络活动的进程”中勾选“QQ.exe”。  
![](http://a2.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/AHKONiYpYbBXlP97coXmpmXw90aHoTsbPFV9YQXzM*0!/b/dF5CJ8TNGgAA&ek=1&kp=1&pt=0&bo=JANWAgAAAAADAFY!&tl=1&su=05420801&tm=1551880800&sce=0-12-12&rf=2-9)  

3、选好之后，可以在下方的“TCP连接”中看到所有QQ.exe进程的详细信息，筛选出来的QQ进程有好几个。  
![](http://a1.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/Th26DSXGSBvgGtGNqKwobh.yQuaF.bUojTVAdARNEf4!/b/dDeFi8MlGQAA&ek=1&kp=1&pt=0&bo=JANWAgAAAAADAFY!&tl=1&su=0128440769&tm=1551880800&sce=0-12-12&rf=2-9)  

4、用鼠标右键点击标示该列名称的位置，然后点击“选择列”，勾选其中的“发送”，让这一项的数据也显示在列表中。  
![](http://a1.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/LMSadOp5MY6oM4Q.IbsiOg8TQD9v4DOTdAocx1o8VCI!/b/dE*9icMkGQAA&ek=1&kp=1&pt=0&bo=QwEvAQAAAAADAEk!&tl=1&su=0215326513&tm=1551880800&sce=0-12-12&rf=2-9)  

5、和你要查询IP地址的好友随便说一句话，再去查看“发送”列中有数据变化的进程，该进程的“远程地址”就是这位好友的IP地址了！  
![](http://a3.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/bczMlyoJ3plNpfM6bT5z4B2OCHx7Abcy4cI9hlkklwY!/b/dP5FvsShAgAA&ek=1&kp=1&pt=0&bo=pgNWAgAAAAADANQ!&tl=1&su=085733361&tm=1551880800&sce=0-12-12&rf=2-9)  