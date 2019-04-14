---
layout: post
title: "【编程】Sublime Text 使用技巧01"
date: 2016-04-04 23:05
categories: 【编程】
tags:
- Sublime Text
---
　　Sublime Text是开发代码编辑的神器 ，编辑器界面优美，操作速度快速。而且Sublime Text是一款跨平台的编辑器，再也不用为换平台而找不到合适的、熟悉的编辑器担忧了。  
　　Sublime Text 是一款具有代码高亮、语法提示、自动完成且反应快速的编辑器软件，不仅具有华丽的界面，还支持插件扩展机制，用她来写代码，绝对是一种享受。  
　　两个小技巧：选择文字之后，按下 Tab 和 Shift + Tab 可以控制缩进，和 EmEditor 一样，内牛。文件未保存就可以直接退出程序，下次启动会自动恢复。  
![](http://upload.gezila.com/data/20130622/27991371863700.png)  

### 一、在当前项目中，快速搜索文件  
1. 搜索文件  
![](http://upload.gezila.com/data/20130622/46151371863700.png)  
2. 搜索文件小技巧，在输入文件路径的时候，可以/c/u/a/这样的格式匹配来快速找到文件  
![](http://upload.gezila.com/data/20130622/42221371863701.png)  
3. 搜索到了2个结果，可以按上下键来在多个结果中跳转  
![](http://upload.gezila.com/data/20130622/87551371863701.png)  

### 二、添加注释  
1. 添加块注释，类似于`/* */`用这种方法来添加的注释一样。  
先选择要注释的内容，然后按 ctrl + /  
![](http://upload.gezila.com/data/20130622/32961371863701.png)  

2. 添加行注释，把鼠标移到改行的任意位置，按ctrl + /即可  
![](http://upload.gezila.com/data/20130622/93941371863702.png)  
3. 取消单行注释，鼠标位于已经注释的行的任意位置，执行ctrl + /即可  
![](http://upload.gezila.com/data/20130622/32641371863702.png)  
![](http://upload.gezila.com/data/20130622/99301371863702.png)  
4. 取消块注释  
选择要取消的内容，按ctrl + /即可  
![](http://upload.gezila.com/data/20130622/45551371863702.png)  
![](http://upload.gezila.com/data/20130622/72001371863702.png)  
5. 即取消注释和添加注释是逆操作  

### 三、快速跳转到指定的行  
ctrl + g,然后输入行号，enter就行。比如跳转到第五行。 或者ctrl + p,再输入 :  
![](http://upload.gezila.com/data/20130622/22861371863703.png)  

### 四、 搜索函数  
按ctrl + r 或 ctrl + p ,在执行@。 之后填写要搜索的函数名  
![](http://upload.gezila.com/data/20130622/89771371863703.png)  

### 五、 隐藏菜单和显示菜单栏  
1. 隐藏菜单栏：view --> Hide Menu  
![](http://upload.gezila.com/data/20130622/37621371863703.png)  
2. 隐藏菜单栏后，要显示菜单栏：  
这是隐藏之后  
![](http://upload.gezila.com/data/20130622/14711371863703.png)  
3.隐藏之后显示菜单栏 按住Alt 键，菜单栏即会出现。松开后，则菜单栏就会消失。要永久显示则是： 按住Alt 键-->view--> show Menu  
![](http://upload.gezila.com/data/20130622/59761371863704.png)  

### 六、扩展  
Sublime Text是支持插件扩展的，首先，我们需要安装Package Contro，ctrl+\`调出命令行工具，输入  

```
import urllib2,os;pf='Package Control.sublime-package';ipp=sublime.installed_packages_path();os.makedirs(ipp) if not os.path.exists(ipp) else None;open(os.path.join(ipp,pf),'wb').write(urllib2.urlopen('<http://sublime.wbond.net/>'+pf.replace(' ','%20')).read())
```

回车即可。  
点击Preferences→Package Control，显示以下弹窗：  
Package Control Disable Package ：禁用插件  
Package Control enable Package ：启用插件  
Package Control Install Package ：安装插件  
Package Control List Package ：查看已安装插件列表  
Package Control Remove Package ：移除插件  
Package Control Upgrade Package ：升级插件  
![](http://upload.gezila.com/data/20130622/94591371863720.jpg)  
**插件推荐：**  
### 已安装插件列表：  
![](http://upload.gezila.com/data/20130622/83181371863720.jpg)  
Emmet  
前端必备，快速开发HTML/CSS  
![](http://upload.gezila.com/data/20130622/94121371863720.jpg)  
输入 div.wrapper>div.header+div.main+div.footer 按下Tab，立刻变成  
![](http://upload.gezila.com/data/20130622/47581371863720.jpg)  
或者按下ctrl+alt+enter，激发zencoding控制台，可看到整个动态的过程。  
![](http://upload.gezila.com/data/20130622/16651371863721.jpg)  

JsFormat  
格式化js代码，这个插件很有用，我们有时在网上看到某些效果，想查看是怎么实现的，但是代码被压缩过，很难阅读，不用怕，按下ctrl+alt+5(这是我设置的快捷键)，即可让代码还原。  
![](http://upload.gezila.com/data/20130622/43761371863721.jpg)  
![](http://upload.gezila.com/data/20130622/28971371863724.jpg)  

Tag  
格式化标签，让乱七八糟的代码，瞬间整齐清晰。  

BracketHighlighter  
括弧高亮显示  

Clipboard History  
剪切板历史，可以保存多个复制信息，按下ctrl+alt+v，可以选择历史剪切板  
![](http://upload.gezila.com/data/20130622/52591371863724.jpg)  

Goto-CSS-DeclaratioPackage Control  
跳转到css文件该class的声明处，方便修改查看，如图下所示，注意对应的css文件要同时打开才行。  
![](http://upload.gezila.com/data/20130622/44761371863724.jpg)  
![](http://upload.gezila.com/data/20130622/64311371863725.jpg)  

GotoRecent  
打开最近的文件，系统有这个功能，但只能看最近8个，有点不爽，按ctrl+e，选择即可。  
SCSS，支持scss的语法高亮，里面附带了好多CSS Snippet，无论现用或者改造成，都可节省不少时间。  
![](http://upload.gezila.com/data/20130622/99561371863725.jpg)  
还有很多插件，jquery语法提示，jsHint等等。  

### 主要快捷键列表  
　　Ctrl+L 选择整行(按住-继续选择下行)  
　　Ctrl+KK 从光标处删除至行尾  
　　Ctrl+Shift+K 删除整行  
　　Ctrl+Shift+D 复制光标所在整行，插入在该行之前  
　　Ctrl+J 合并行(已选择需要合并的多行时)  
　　Ctrl+KU 改为大写  
　　Ctrl+KL 改为小写  
　　Ctrl+D 选词 (按住-继续选择下个相同的字符串)  
　　Ctrl+M 光标移动至括号内开始或结束的位置  
　　Ctrl+Shift+M 选择括号内的内容(按住-继续选择父括号)  
　　Ctrl+/ 注释整行(如已选择内容，同“Ctrl+Shift+/”效果)  
　　Ctrl+Shift+/ 注释已选择内容  
　　Ctrl+Z 撤销  
　　Ctrl+Y 恢复撤销  
　　Ctrl+M 光标跳至对应的括号  
　　Alt+. 闭合当前标签  
　　Ctrl+Shift+A 选择光标位置父标签对儿  
　　Ctrl+Shift+[ 折叠代码  
　　Ctrl+Shift+] 展开代码  
　　Ctrl+KT 折叠属性  
　　Ctrl+K0 展开所有  
　　Ctrl+U 软撤销  
　　Ctrl+T 词互换  
　　Tab 缩进 自动完成  
　　Shift+Tab 去除缩进  
　　Ctrl+Shift+↑ 与上行互换  
　　Ctrl+Shift+↓ 与下行互换  
　　Ctrl+K Backspace 从光标处删除至行首  
　　Ctrl+Enter 光标后插入行  
　　Ctrl+Shift+Enter 光标前插入行  
　　Ctrl+F2 设置书签  
　　F2 下一个书签  