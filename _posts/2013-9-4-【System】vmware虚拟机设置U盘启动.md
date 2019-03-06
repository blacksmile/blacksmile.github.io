---
layout: post
title: "【System】vmware虚拟机设置U盘启动"
date: 2013-9-4 16:41
categories: 【System】
tags:
- vmware虚拟机
---

**很多网友都有了可启动的U盘吧，不过，还是很多网友不知道如何设置虚拟机，才能让虚拟机支持U盘启动，下面讲解一下如何设置虚拟机从U盘启动。**  
**温馨提示：应首先插上U盘，然后启动vmware虚拟机，否则设置时会找不到U盘。**  
 **U盘启动盘常用启动方式有USB-ZIP、 USB-HDD 、USB-CDROM几种，根据不同启动方式有不同设置。我这里演示两种方法给大家参考**  
**![](http://a1.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/zXhphH5kPKdbhznUdi3z.ri6IUTEUBWdeAAniyRxeCY!/b/dLB2iMOOFQAA&ek=1&kp=1&pt=0&bo=WAL0AQAAAAABAIg!&t=5&tl=3&su=0221206593&tm=1551790800&sce=0-12-12&rf=2-9)**  

<!-- more -->

**第一种：USB-CDROM启动**  
**1、如果量产成了USB-CDROM,那么在编辑虚拟机设置里面使用物理光驱，不要自动探测，手动选定USB-CDROM盘符，然后虚拟机第一启动选择光驱启动。**  
![](http://a2.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/JO4bj.Dr.nOsGZyuOYfvS6RPqq.fo5e*H69XmjWitwk!/b/dPGtIsRFFwAA&ek=1&kp=1&pt=0&bo=6gFVAQAAAAABAJg!&t=5&tl=3&su=0217006049&tm=1551790800&sce=0-12-12&rf=2-9)  
**2、我将1G的U盘量产成一个USB-CDROM和一个移动磁盘。**  
![](http://a1.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/SfLD4dkmqXO5N0QjRcCfQ*qOeehwQlVPfa6KxVVxs*Y!/b/dE15gsOOFQAA&ek=1&kp=1&pt=0&bo=SAJ9AQAAAAABABE!&tl=3&su=020697089&tm=1551790800&sce=0-12-12&rf=2-9)  
**3、VM需要手动设置USB-CDROM，启动时按F2进入BIOS设置CD-ROM为第一启动，或者按ESC选择CD-ROM第一启动。**  
![](http://a1.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/OoDLVG33iVxWjri*qvczvAJbC5nJ3L6AqT.cfUa6F*8!/b/dLQrkMORFQAA&ek=1&kp=1&pt=0&bo=gwLlAQAAAAABAEI!&tl=3&su=0262154657&tm=1551790800&sce=0-12-12&rf=2-9)  
![](http://a1.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/nqIaDPb3jvUsLV*LqDLrkLYihDu8k76ZInULI.9PKfk!/b/dH3.hsNTFAAA&ek=1&kp=1&pt=0&bo=6gEoAQAAAAABAOU!&t=5&tl=3&su=087164225&tm=1551790800&sce=0-12-12&rf=2-9)  
![](http://a1.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/jBNbNt4FPrFkUNA*1GLLBtt16btdlF0xPuj5bOLRvTE!/b/dBwUjcOQFQAA&ek=1&kp=1&pt=0&bo=6gFzAQAAAAABAL4!&t=5&tl=3&su=0260672369&tm=1551790800&sce=0-12-12&rf=2-9)  
**4、启动后，进入USB-CDROM启动界面，这里安装的是XP SP3操作系统。USB-CDROM设置完毕。**  
![](http://a4.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/BuG4mPGDcV2IoSO2Q30VIblelKu9JeFuGMiwOTYRViI!/b/dOr48sJcGgAA&ek=1&kp=1&pt=0&bo=oAIYAgAAAAABAJ8!&t=5&tl=3&su=065506593&tm=1551790800&sce=0-12-12&rf=2-9)  
**第二种：USB-ZIP或者USB-HDD 启动方式，下面是设置过程：**  
**温馨提示：应首先插上U盘，然后启动vmware虚拟机，否则设置时会找不到U盘。**  
**1、打开虚拟机后，点击“编辑虚拟机设置”（注意，一定要在这个界面编辑，如果进入虚拟机中的操作系统编辑，那么会无法设置成功。）**  
![](http://a1.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/hWYjPc8oa2bxbh1B7IoOOjE7Wk9c3Yi6XnFNyI5En3M!/b/dPiWjsORFQAA&ek=1&kp=1&pt=0&bo=6gFbAQAAAAABAJY!&t=5&tl=3&su=067025025&tm=1551790800&sce=0-12-12&rf=2-9)  
**2、选择【硬盘】点【下一步】**  
![](http://a1.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/A9LAbJqe3c.JwqSGc7ftfxHI..ngRZ*hTal6eY5raNA!/b/dHo1kMOOFQAA&ek=1&kp=1&pt=0&bo=6gGRAQAAAAABAFw!&t=5&tl=3&su=0166502337&tm=1551790800&sce=0-12-12&rf=2-9)  
![](http://a4.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/9qszkTlMQVQOGlFTa.Ao4BFxMNt14904KswpBzEcMaw!/b/dI307MKsGgAA&ek=1&kp=1&pt=0&bo=6gF7AQAAAAABALY!&t=5&tl=3&su=069618449&tm=1551790800&sce=0-12-12&rf=2-9)  
**3、我们这里选择【使用物理磁盘】 然后点下一步**  
![](http://a2.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/TTsT153KFm.cFdBBGLunrK4Sdq6g08cfmUJqBglUewE!/b/dJYcHsRHFwAA&ek=1&kp=1&pt=0&bo=6gGOAQAAAAABAEM!&t=5&tl=3&su=0217298001&tm=1551790800&sce=0-12-12&rf=2-9)  
**4、设置完毕了，我们点击【确定】然后启动虚拟机在BIOS里设置U盘启动就行了。**  
**BIOS设置，如图所示：我们按F2 快捷键**  
![](http://a1.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/PQmrw9XC5P4ZcdX4Iuy0ofwJF4M2l8KBdPDtM.m0fUQ!/b/dCSPi8ORFQAA&ek=1&kp=1&pt=0&bo=6gGcAQAAAAABAFE!&t=5&tl=3&su=078442193&tm=1551790800&sce=0-12-12&rf=2-9)  
**使用键盘方向键 选择【Boot】---->【Hard Drive】回车，通过键盘的【+】设置第一启动为【VMware Virtuanl SCSI Hard Drive (0:0=1)】---->按F10/Y保存刚刚的设置。**  
**5、退出启动后进入USB-ZIP或者USB-HDD，界面如下：**  
![](http://a4.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/BuG4mPGDcV2IoSO2Q30VIblelKu9JeFuGMiwOTYRViI!/b/dOr48sJcGgAA&ek=1&kp=1&pt=0&bo=oAIYAgAAAAABAJ8!&tl=3&su=065506593&tm=1551790800&sce=0-12-12&rf=2-9)