---
layout: post
title: "【System】Windows Server 2008 R2虚拟机优化"
date: 2013-09-28 21:21
categories: 【System】
tags:
- VMware虚拟机优化
- Windows Server 2008 R2
---
Windows Server 2008 R2是微软最新的服务器版操作系统,与Windows 7相同的使用了最新的NT6.1内核
Server系统有着更为出色的内存管理等方面的性能,而且对于开发平台的支持也比client系统更加优秀,下面就讲述一下打造个性化的Windows Server 系统,让它适合桌面用户使用.  

首先刚安装完进入系统时,会强制要求修改密码,此处的密码需要符合密码复杂性.即大写字母,小写字母,数字,特殊符号四种字符中必须有三种以上.设置完毕密码之后,可以进入系统.首先就干掉这个密码复杂性.  
打开开始菜单--管理工具--本地安全策略,将其中的账户策略--密码策略下的密码必须符合复杂性要求设置为禁用  
如图  
![](http://hiphotos.baidu.com/enixdq3/pic/item/4371150b42942b14b0351d0c.jpg)  

<!-- more -->

初次进入系统时,可以看到Windows Server 2008 R2的界面依然采用了Windows 2000的经典界面,对于一般用户来说,这个界面有点过时,因此,首先要将界面设置的漂亮些.  
![](http://hiphotos.baidu.com/enixdq3/pic/item/5c7d3c768e7e2431b151b9ed.jpg)  

此时需要做的是,添加管理桌面主题和多媒体等功能的桌面体验功能,如果没有添加此功能,在services里面是找不到themes服务的具体操作为点击任务栏上的服务器管理器,或者右键计算机,选择管理在服务器管理器中,选择添加功能,打开面板之后,普通用户需要添加桌面体验功能,如果是笔记本或者有无线网卡的,可以同时添加无线LAN服务功能  
![](http://hiphotos.baidu.com/enixdq3/pic/item/14370a3c8990462abba1670c.jpg)  

重启之后,就可以使用其他主题了,打开cmd,运行services.msc,将themes服务设置为自动,并启动服务.  
然后右键计算机--属性,选择左上角三个选项中的高级系统设置--高级--性能设置,将视觉效修改为最佳外观  
![](http://hiphotos.baidu.com/enixdq3/pic/item/6ec4020b5502b23594ca6b0c.jpg)  
然后注销,再次登录之后,就可以选择使用其他主题了.此时系统的界面已经与Windows 7基本一致(只缺少侧边栏,个人不喜欢用,就没有添加)  
![](http://hiphotos.baidu.com/enixdq3/pic/item/25a52618408d206f42a9ad02.jpg)  

接下来需要优化的是部分系统方面的设置了  
首先,登录时需要按CTRL+ALT+DEL很让人不爽,去掉它  
开始菜单--管理工具--本地安全策略--本地策略--安全选项中的交互登录模式,无需按CTRL+ALT+DEL,启用起来  
![](http://hiphotos.baidu.com/enixdq3/pic/item/50cef208a471e7e53ac7630c.jpg)  

还有烦人的关机理由也去掉  
打开命令行,输入gpedit.msc进入组策略  
将计算机配置--管理模版--系统下的显示"关机事件跟踪程序"禁用  
![](http://hiphotos.baidu.com/enixdq3/pic/item/2521f7d8279ac00610df9b02.jpg)  

现在开机和关机都顺畅了,最后需要优化的是部分程序默认设置  
将处理器优先设置为程序和将DEP修改为仅系统  
右键计算机--属性--高级系统设置--高级--性能设置--高级--处理器计划修改为程序  
![](http://hiphotos.baidu.com/enixdq3/pic/item/9c2e098386115b956d811901.jpg)  

右键计算机--属性--高级系统设置--高级--性能设置--高级--数据执行保护修改为仅为基本windows程序和服务启用  
![](http://hiphotos.baidu.com/enixdq3/pic/item/16f1b43e9547ecc655e72301.jpg)  

重启之后就可以了  
最后一个要设置的是IE的ESC设置  
打开服务器管理器,找到安全信息--配置IE ESC  
![](http://hiphotos.baidu.com/enixdq3/pic/item/ad7b331fc99f6a354034170c.jpg)  

将IE ESC设置为禁用  
![](http://hiphotos.baidu.com/enixdq3/pic/item/b4a0dac3e02b121fe4dd3b01.jpg)  

至此所有初级设置全部完毕,你的Windows Server 2008 R2系统完全可以当做Windows 7桌面版系统使用  
![](http://hiphotos.baidu.com/enixdq3/pic/item/881f5b1aa05f6ad0ae513301.jpg)  
接下来就完全可以按照个人的使用习惯配置适合自己的开始菜单,任务栏等.