---
layout: post
title: "【Software】搭建个人博客"
date: 2019-02-24 21:57
categories: 【Software】
tags:
- 搭建个人博客
---
**博客模版下载地址**  
<http://jekyllthemes.org/>  
<https://github.com/Simpleyyt/jekyll-jacman>  
<https://github.com/codeasashu/hcz-jekyll-blog>  

**一、创建Github仓库**  
先登陆Github账号,如下图新建一个仓库  
![](http://r.photo.store.qq.com/psb?/57f6398e-db93-428d-8871-6d2527ad188f/tmAY1*Uz4Bv*DCDMg1UA5prkQdNhvbSqzH8eGixu4KY!/o/dDYBAAAAAAAA&ek=1&kp=1&pt=0&bo=qwJsAasCbAEDEDU!&tl=1&su=044720545&tm=1553403600&sce=0-12-12&rf=2-9)  
![](http://r.photo.store.qq.com/psb?/57f6398e-db93-428d-8871-6d2527ad188f/Gwbkp2XqrxRugyLAEdRooXO7La.eGhpfI96OgryK66I!/o/dDYBAAAAAAAA&ek=1&kp=1&pt=0&bo=egJSAXoCUgEDEDU!&tl=1&su=028536049&tm=1553403600&sce=0-12-12&rf=2-9)  
`Repository name就是你的仓库名,这个仓库名必须按(帐户名.github.io)格式来写,到时候访问的地址就是这个了,至于下面的Initialize this repository with a README( 使用 README.md 初始化仓库这将让您可以立刻克隆该仓库到您的电脑。如果您要提交已有的仓库，请忽略这个选项)`  
![](http://r.photo.store.qq.com/psb?/57f6398e-db93-428d-8871-6d2527ad188f/qa0AWqGcOyEpRRovsf6vNPtYdYhTmPWtZvhdyobwfl8!/o/dL4AAAAAAAAA&ek=1&kp=1&pt=0&bo=VgXYAlYF2AIDIAU!&tl=1&su=021208833&tm=1553403600&sce=0-12-12&rf=2-9)  

**二、将GitHub仓库克隆到本地**  
1.在自己的电脑上找一个目录来作为你本地的仓库,比如我的是”D:\GitHub”,那么就在GitHub文件夹下初始化仓库.  
2.初始化仓库的方式有两种,一种是用git的图形化界面来创建,另一种是用git命令来初始化,这里我使用图形化界面的方式来创建(先下载desktop github然后安装，desktop github新版不支持Windows 32位系统)  
desktop github下载地址  
<https://desktop.github.com/>  
登入到GitHub  
![](http://r.photo.store.qq.com/psb?/57f6398e-db93-428d-8871-6d2527ad188f/vQMvgZ7pfIjDE.MzZsaGcfewu3JSXJO11eJF.nyvPHE!/o/dL8AAAAAAAAA&ek=1&kp=1&pt=0&bo=vwOVAr8DlQIDMBU!&tl=1&su=0182371809&tm=1553403600&sce=0-12-12&rf=2-9)  
向GitHub提交统计数据可不勾  
![](http://r.photo.store.qq.com/psb?/57f6398e-db93-428d-8871-6d2527ad188f/3eP6kBUk7CBSk6SLUf9CZycRKQBf7*5YJEzrxrbq2GI!/o/dFMBAAAAAAAA&ek=1&kp=1&pt=0&bo=wgOVAsIDlQIDMBU!&tl=1&su=0110439745&tm=1553403600&sce=0-12-12&rf=2-9)  
![](http://r.photo.store.qq.com/psb?/57f6398e-db93-428d-8871-6d2527ad188f/HSuIxscKJqTIjyvDtQQnbndT5ui030UeV17KKEkS3TU!/o/dMIAAAAAAAAA&ek=1&kp=1&pt=0&bo=VgXXAlYF1wIDEDU!&tl=1&su=017684945&tm=1553403600&sce=0-12-12&rf=2-9)  
![](http://r.photo.store.qq.com/psb?/57f6398e-db93-428d-8871-6d2527ad188f/rUJA*MjAXmz.RE.GTWNHsJ9HdRrej6ehuqEedjScIAU!/o/dDQBAAAAAAAA&ek=1&kp=1&pt=0&bo=8gSgAvIEoAIDIAU!&tl=1&su=0205845697&tm=1553403600&sce=0-12-12&rf=2-9)  
克隆中等会  
![](http://r.photo.store.qq.com/psb?/57f6398e-db93-428d-8871-6d2527ad188f/EWV5ilSfUz.*MBff6P*t6GbkoRYdM*WDjMZjJ*fRf8g!/o/dL8AAAAAAAAA&ek=1&kp=1&pt=0&bo=VgXYAlYF2AIDEDU!&tl=1&su=0159959169&tm=1553403600&sce=0-12-12&rf=2-9)  
完成  
![](http://r.photo.store.qq.com/psb?/57f6398e-db93-428d-8871-6d2527ad188f/H8bG5Ein8awOph0KkJsylp6qT8Q9XU9MqXj481JdISU!/o/dL8AAAAAAAAA&ek=1&kp=1&pt=0&bo=VgXUAlYF1AIDEDU!&tl=1&su=0230474961&tm=1553403600&sce=0-12-12&rf=2-9)  
**三、将网页传到GitHub上**  
1.在本地的路径下放入文件
![](http://r.photo.store.qq.com/psb?/57f6398e-db93-428d-8871-6d2527ad188f/CyAjfqukp1304o7bIVzBC.rOYddUrXSzAdM23JaVf2U!/o/dL8AAAAAAAAA&ek=1&kp=1&pt=0&bo=2gJcAtoCXAIDEDU!&tl=1&su=0263285937&tm=1553403600&sce=0-12-12&rf=2-9)  
提交备注（给提交的文件添加个摘要信息）  
furst push  
![](http://r.photo.store.qq.com/psb?/57f6398e-db93-428d-8871-6d2527ad188f/pvI3WikkaVH1QgeLzXMEPNVwyCZOTfNe2xhHQyXiqog!/o/dL8AAAAAAAAA&ek=1&kp=1&pt=0&bo=VgXYAlYF2AIDEDU!&tl=1&su=0129619153&tm=1553403600&sce=0-12-12&rf=2-9)  
2.然后回到网页这刷新下就可以了  
![](http://r.photo.store.qq.com/psb?/57f6398e-db93-428d-8871-6d2527ad188f/it7SSmFD0VZwvyDJFYtilXimfk*HRs8d50*T.d*sONM!/o/dDQBAAAAAAAA&ek=1&kp=1&pt=0&bo=VgXUAlYF1AIDEDU!&tl=1&su=0214101793&tm=1553403600&sce=0-12-12&rf=2-9)  
**四、浏览自己的网页**  
访问自己上传的网页(点自己的仓库-设置  往下拉)  
![](http://r.photo.store.qq.com/psb?/57f6398e-db93-428d-8871-6d2527ad188f/2dAtNdcTecMw7gPAjjeNzkxdCQcoWN3UMUZhe9HrjWg!/o/dL8AAAAAAAAA&ek=1&kp=1&pt=0&bo=8QOjAPEDowADEDU!&tl=1&su=0232018353&tm=1553403600&sce=0-12-12&rf=2-9)  
然后就可以通过GitHub提供的这个网址访问自己的博客了  
![](http://r.photo.store.qq.com/psb?/57f6398e-db93-428d-8871-6d2527ad188f/VJ0fICRzY43ZK591.anx8zfW3sMyNS7VLH0C4VtomAY!/o/dFQBAAAAAAAA&ek=1&kp=1&pt=0&bo=wAL7AMAC.wADEDU!&tl=1&su=0268041425&tm=1553403600&sce=0-12-12&rf=2-9)  
![](http://r.photo.store.qq.com/psb?/57f6398e-db93-428d-8871-6d2527ad188f/.DCDzaYjz8f17vCeRiWeAHcC33QOwk4l1K4fGbrk5ak!/o/dL4AAAAAAAAA&ek=1&kp=1&pt=0&bo=VgXaAlYF2gIDEDU!&tl=1&su=0166572849&tm=1553403600&sce=0-12-12&rf=2-9)  


**【需要使用Markdown编辑器写博客】**  
第一步:去JekyllThemes下载一个自己喜欢的模板  
第二步:按照之前的步骤把下载好的模板上传到自己的Github仓库中  
第三步:在_posts文件夹中放入自己写好的博客,文件名必须是日期-标题名,例如:2019-01-01-我的第一篇博客  
第四步:上传博客到Github中即可访问自己的博客  
![](http://r.photo.store.qq.com/psb?/57f6398e-db93-428d-8871-6d2527ad188f/dV0FGUcNRaFWFKAAsldsvxZ7wFjL93nalP5vWHUWa6c!/o/dLkAAAAAAAAA&ek=1&kp=1&pt=0&bo=2wO1AdsDtQEDEDU!&tl=1&su=0119672833&tm=1553403600&sce=0-12-12&rf=2-9)