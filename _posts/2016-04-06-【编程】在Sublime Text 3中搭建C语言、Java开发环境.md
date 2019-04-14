---
layout: post
title: "【编程】在Sublime Text 3中搭建C语言、Java开发环境"
date: 2016-04-06 17:25
categories: 【编程】
tags:
- Sublime Text
---

### 一、在Sublime Text 3中搭建C语言开发环境  
Sublime Text 3的高亮显示代码，非常好用，界面也非常漂亮，Sublime Text 3工具栏有编译项，所以想让它来编译C和C++代码。  
我们用到的C/C++编译器使用的是gcc/g++，所以需要下载安装MinGW。  
1.下载地址  
<http://sourceforge.net/projects/mingw/>  
这个是边下载边安装的，下载完成即安装完成。  
比如我安装在C:\MinGW  

2.设置环境变量。右击我的电脑，点属性->高级->环境变量。（如果里面还有其他的变量，记得要加个分号啊，分号得在英文输入模式下输入的。）  
添加以下  
变量                   值  

```
PATH                  C:\MinGW\bin;
LIBRARY_PATH          C:\MinGW\lib;
C_INCLUDEDE_PATH      C:\MinGW\include;
```

下面就是要判断一下我们的MinGW是否安装成功，直接运行cmd命令行，输入g++ -v  
![](http://a1.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/tSqxr03396Jn.KmueAsiomANySlzGAHZFMFDeiir3nE!/b/dGgAAAAAAAAA&ek=1&kp=1&pt=0&bo=pgK8AQAAAAADADw!&tl=1&su=0179766689&tm=1555232400&sce=0-12-12&rf=2-9)  
显示如上则安装成功。  
因为Sublime Text中已经有了默认的编译器相关配置，所以配置好环境变量后c/c++是直接可以编译运行的，写一个程序测试一下  
![](http://a3.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/1LqgjDcc4DKIDMJhAw9FZZvPF4kxPkf7cJgfS58ud5I!/b/dGYAAAAAAAAA&ek=1&kp=1&pt=0&bo=KAMEAgAAAAADAAg!&tl=1&su=022593441&tm=1555232400&sce=0-12-12&rf=2-9)  
Ctrl+B编译  
![](http://a1.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/fTIypiDyzD3GS1Y6*GH9mu*GPrt0Kc2b8FTgOlX5bFc!/b/dFgBAAAAAAAA&ek=1&kp=1&pt=0&bo=KAMEAgAAAAADAAg!&tl=1&su=049263921&tm=1555232400&sce=0-12-12&rf=2-9)  
Ctrl+Shift+B运行，怎么样是不是很神奇。  
相关问题：  
​     配置好了，开发环境后还有一些问题，如果代码写的正确可以直接编译运行，可是如果代码写错了的话，编译失败会出现以下提示：  
![](http://a1.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/.iHG1aQNuYoH8vFHY5OkVNpides3Jt5M4psA57jJLEI!/b/dGgAAAAAAAAA&ek=1&kp=1&pt=0&bo=KAMEAgAAAAADAAg!&tl=1&su=0101679617&tm=1555232400&sce=0-12-12&rf=2-9)  
它不显示错误的地方，所以还要我们修改以下它默认c/c++编译器的配置文件  
用winrar打开Packages目录下的C++.sublime-package，再用Sublime Text打开里面的C++.sublime-build文件修改如下：  
![](http://a2.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/PST25ppHYvlpd1GPtVKbzmdHn.4SQWzKNR.ciIp8u0s!/b/dFkBAAAAAAAA&ek=1&kp=1&pt=0&bo=KAMEAgAAAAADAAg!&tl=1&su=0187428785&tm=1555232400&sce=0-12-12&rf=2-9)  
现在再来试试，Ctrl+B编译  
![](http://a4.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/HZ6TUYTRcn61uhm5K6mHef1reMJD2x1pGKuTv71QIoY!/b/dFcBAAAAAAAA&ek=1&kp=1&pt=0&bo=KAMEAgAAAAADAAg!&tl=1&su=0145959505&tm=1555232400&sce=0-12-12&rf=2-9)  
如上图说明成功了  
### 二、在Sublime Text 3中搭建Java开发环境  
Sublime Text 3的高亮显示代码，非常好用，界面也非常漂亮，Sublime Text 3工具栏有编译项，所以想让它来编译和运行Java代码  
1.设置Java的PATH环境变量（自行百度）  
2.创建批处理或Bash Shell脚本文件  
新建记事本，输入下面的内容，并保存为`runJava.bat文件`。  

```
@ECHO OFF
   cd %~dp1
​      ECHO Compiling %~nx1.......
​      IF EXIST %~n1.class (
​      DEL %~n1.class
​      )
​      javac %~nx1
​      IF EXIST %~n1.class (
​      ECHO -----------OUTPUT-----------
​      Java %~n1
​      )
```

​然后把runJava.bat批处理文件移动到JDK的bin目录。  
3.在Sublime Text 3编辑器中配置相应的Java构建环境  
用winrar打开Sublime Text 3的Package目录下的Java.sublime-package，用Sublime Text打开里面的JavaC.sublime-build将文件修改为  

```
{
   "shell_cmd": "runJava.bat \"$file\"",
   "file_regex": "^(...*?):([0-9]*):?([0-9]*)",
   "selector": "source.java",
   "encoding":"cp936"
}
```

![](http://a3.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/nu6BsDDrHrRqf4xfNG4MTQZR1FC9mGsRmXwasWhtP3o!/b/dFoBAAAAAAAA&ek=1&kp=1&pt=0&bo=7wLxAQAAAAADADg!&tl=1&su=040995025&tm=1555232400&sce=0-12-12&rf=2-9)  
修改好了保存一下  
​下面写一个java程序测试一下（Ctrl+B编译运行）出现以下结果说明成功了  
![](http://a3.qpic.cn/psb?/57f6398e-db93-428d-8871-6d2527ad188f/*W8eADA7bqbt*VCICgK*eFa*iSXhHnNFZNttVXxIFSQ!/b/dFoBAAAAAAAA&ek=1&kp=1&pt=0&bo=KAMEAgAAAAADAAg!&tl=1&su=0145950097&tm=1555232400&sce=0-12-12&rf=2-9)  
直接将控制台输出结果显示在Sublime Text 3中  

如果不想每次编译文件后，还需要切换窗口点击运行编译生成的exe来查看结果的话。还可以在简单的配置一下，直接将控制台输出的结果显示在ST中，也不需要切换窗口，只需要在调用Ctrl+B编译后再键入Ctrl+Shift+B运行即可。将Sublime Text的Packages目录下的Packages\C++\C++.sublime-build文件修改为：  

复制代码 代码如下:  

```
{
​    "cmd": ["g++", "${file}", "-o", "${file_path}/${file_base_name}"],
​    "file_regex": "^(..[^:]*):([0-9]+):?([0-9]+)?:? (.*)$",
​    "working_dir": "${file_path}",
​    "selector": "source.c, source.c++",
​    "encoding":"cp936",
​    "variants":
​    [
​        {
​            "name": "Run",
​            "cmd": ["${file_path}\\\\${file_base_name}.exe"]
​        }
​    ]
}
```
