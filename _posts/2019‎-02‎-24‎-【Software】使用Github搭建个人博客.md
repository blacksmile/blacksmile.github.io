---
layout: post
title: "【Software】使用Github搭建个人博客"
date: 2019‎-02‎-24‎ 21:49
categories: 【Software】
tags:
- Github搭建个人博客
---
**博客模版下载地址**  
<http://jekyllthemes.org/>  
<https://github.com/Simpleyyt/jekyll-jacman>  
<https://github.com/codeasashu/hcz-jekyll-blog>  
**一、创建Github仓库**  
先登陆Github账号,如下图新建一个仓库  
![](https://qqadapt.qpic.cn/txdocpic/0/e5cf32394edf46882b1c9fae1658d539/0?_type=png)  
![](https://qqadapt.qpic.cn/txdocpic/0/4e2f615e24af8c7207ec9031a8c592f1/0?_type=png)  
`Repository name就是你的仓库名,这个仓库名必须按(帐户名.github.io)格式来写,到时候访问的地址就是这个了,至于下面的Initialize this repository with a README( 使用 README.md 初始化仓库这将让您可以立刻克隆该仓库到您的电脑。如果您要提交已有的仓库，请忽略这个选项)`  
![](https://qqadapt.qpic.cn/txdocpic/0/909919ccad377b1b025148d2ea576add/0?_type=png)  
**二、将GitHub仓库克隆到本地**  
1.在自己的电脑上找一个目录来作为你本地的仓库,比如我的是”D:\GitHub”,那么就在GitHub文件夹下初始化仓库.  
2.初始化仓库的方式有两种,一种是用git的图形化界面来创建,另一种是用git命令来初始化,这里我使用图形化界面的方式来创建(先下载desktop github然后安装，desktop github新版不支持Windows 32位系统)  
desktop github下载地址  
<https://desktop.github.com/>  
登入到GitHub  
![](https://qqadapt.qpic.cn/txdocpic/0/fa9feae3f48023da8a588c0a775af934/0?_type=png)  
向GitHub提交统计数据可不勾  
![](https://qqadapt.qpic.cn/txdocpic/0/9f65f1e575759f66f54d9ad1d234f239/0?_type=png)  
![](https://qqadapt.qpic.cn/txdocpic/0/fd1f19d24a349dddbf93b660886b8bd8/0?_type=png)  
![](https://qqadapt.qpic.cn/txdocpic/0/bf872756778672d9c7b47097231bd3e9/0?_type=png)  
克隆中等会  
![](https://qqadapt.qpic.cn/txdocpic/0/78bcc1ca652ad1990c9e6ada7e1d70f2/0?_type=png)  
完成  
![](https://qqadapt.qpic.cn/txdocpic/0/00fd4740ddfdcda23df7eaab85d7dff1/0?_type=png)  
**三、将网页传到GitHub上**  
在本地的路径下放入文件  
![](https://qqadapt.qpic.cn/txdocpic/0/b4020eba12429d50e1f1c0c7c517291b/0?_type=png)  
提交备注（给提交的文件添加个摘要信息）  
furst push  
![](https://qqadapt.qpic.cn/txdocpic/0/b293f881f0d22edbb7ab357f6eed9305/0?_type=png)  
2.然后回到网页这刷新下就可以了  
![](https://qqadapt.qpic.cn/txdocpic/0/3ae33b4a96aa2af24004237830c40f3a/0?_type=png)  
**四、浏览自己的网页**  
访问自己上传的网页(点自己的仓库-设置 往下拉)  
![](https://qqadapt.qpic.cn/txdocpic/0/56b3566db2123c1b8b305022ee3fe29c/0?_type=png)  
然后就可以通过GitHub提供的这个网址访问自己的博客了  
![](https://qqadapt.qpic.cn/txdocpic/0/6965e36b15d0dc2d60322430b6e9db41/0?_type=png)  
![](https://qqadapt.qpic.cn/txdocpic/0/8582de71eaa96c50b9c15e5c7e5c6c88/0?_type=png)


**【需要使用Markdown编辑器写博客】**  
第一步:去JekyllThemes下载一个自己喜欢的模板  
第二步:按照之前的步骤把下载好的模板上传到自己的Github仓库中  
第三步:在_posts文件夹中放入自己写好的博客,文件名必须是日期-标题名,例如:2019-01-01-我的第一篇博客  
第四步:上传博客到Github中即可访问自己的博客  
![](https://qqadapt.qpic.cn/txdocpic/0/3b49a3c19deb62a8a60c5e70f7e7703f/0?_type=png)  