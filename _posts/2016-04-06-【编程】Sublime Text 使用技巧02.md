---
layout: post
title: "【编程】Sublime Text 使用技巧 02"
date: 2016-04-06 19:05
categories: 【编程】
tags:
- Sublime Text
---

1. 更改变量名的几种方法  

![](http://qqadapt.qpic.cn/adapt/0/02c77daa-e62a-43dd-904f-97b75294d5d1/800?pt=0&ek=1&kp=1&sce=0-12-12)  

这种情况下该如何快速选中正确的内容？  

第一种方法：  
让Cmd-D (Win: Ctrl-D)只选择同一个变量。  
把光标移到第一个i后面：  
![](http://qqadapt.qpic.cn/adapt/0/a96c6a92-6983-9ee2-255f-216a9247d8d2/800?pt=0&ek=1&kp=1&sce=0-12-12)  
按Cmd-D (Win: Ctrl-D)：  
![](http://qqadapt.qpic.cn/adapt/0/97c1f1dc-6b03-9aa0-3907-808fcd300731/800?pt=0&ek=1&kp=1&sce=0-12-12)  
再按一次：  
![](http://qqadapt.qpic.cn/adapt/0/61afdcaf-dd56-471e-3bab-35505a5717bc/800?pt=0&ek=1&kp=1&sce=0-12-12)  
限制：选取范围中不能有别的同名同类token，如：  
![](http://qqadapt.qpic.cn/adapt/0/0d5f8efd-ac2c-56f6-864f-a41401a42f99/800?pt=0&ek=1&kp=1&sce=0-12-12)  

第二种方法：  
自动选取所有同名同类token。  
把光标移到第一个i后面：  
![](http://qqadapt.qpic.cn/adapt/0/a96c6a92-6983-9ee2-255f-216a9247d8d2/800?pt=0&ek=1&kp=1&sce=0-12-12)  
按Ctrl-Cmd-G (Win: Alt-F3)：  
![](http://qqadapt.qpic.cn/adapt/0/61afdcaf-dd56-471e-3bab-35505a5717bc/800?pt=0&ek=1&kp=1&sce=0-12-12)  
限制：会将别的作用域中的同名同类token都选中，如：  
![](http://qqadapt.qpic.cn/adapt/0/082cf22a-43e5-cec1-e3d5-2c1f74075f23/800?pt=0&ek=1&kp=1&sce=0-12-12)  

第三种方法：  
Cmd-K, Cmd-D (Win: Ctrl-K, Ctrl-D) 跳过选区。  
这个方法能解决所有问题，先把光标移到第一个i后面：  
![](http://qqadapt.qpic.cn/adapt/0/57e4f7d0-7942-2367-9626-e0a2a81745d8/800?pt=0&ek=1&kp=1&sce=0-12-12)  
按Cmd-D (Win: Ctrl-D)：  
![](http://qqadapt.qpic.cn/adapt/0/6b1c2cb6-348d-bcd4-3b7d-664b3c450ce2/800?pt=0&ek=1&kp=1&sce=0-12-12)  
再按一次：  
![](http://qqadapt.qpic.cn/adapt/0/7dee8736-a30c-7653-187d-c16ebef9a607/800?pt=0&ek=1&kp=1&sce=0-12-12)  
这个token我们不想选中，这时候只要分别按 Cmd-K, Cmd-D (Win: Ctrl-K, Ctrl-D) 就可以跳过这个选区：  
![](http://qqadapt.qpic.cn/adapt/0/b3197965-3a4a-b1ba-e64e-159b5d38608e/800?pt=0&ek=1&kp=1&sce=0-12-12)  
这个token也不要，再按一次跳过：  
![](http://qqadapt.qpic.cn/adapt/0/498a1da6-a59c-262f-d797-47d8dc6e8735/800?pt=0&ek=1&kp=1&sce=0-12-12)  
你会发现执行跳过选区后就不再是同名同类的token选择了，不过不要紧，我们继续跳过就好：  
![](http://qqadapt.qpic.cn/adapt/0/14ea040b-011a-67c9-390e-9e7ae59c3a64/800?pt=0&ek=1&kp=1&sce=0-12-12)  
这个token我们要保留，于是只按Cmd-D (Win: Ctrl-D)：  
![](http://qqadapt.qpic.cn/adapt/0/3d0ef6f2-2401-5101-9378-c69ae8a0bf0a/800?pt=0&ek=1&kp=1&sce=0-12-12)  
然后就能正确地重命名了。  

2. 自适应缩进的复制粘贴  
有些情况下我们需要直接复制粘贴一段网上的代码，有些人可能会这样选中原文进行复制：  
![](http://qqadapt.qpic.cn/adapt/0/d90140e5-e488-ea80-9e4e-8109d4a4cdb5/800?pt=0&ek=1&kp=1&sce=0-12-12)  
然后在subl中这样粘贴：  
![](http://qqadapt.qpic.cn/adapt/0/8c0c8783-602f-2404-b21b-bf0006d8e9f5/800?pt=0&ek=1&kp=1&sce=0-12-12)  
但是你会发现粘贴出来的缩进格式完全对不上号：  
![](http://qqadapt.qpic.cn/adapt/0/a01dfd30-bbf7-5b40-bd99-ecdc2607f2f5/800?pt=0&ek=1&kp=1&sce=0-12-12)  
正确的做法如下：  
把目标代码片段的每一个整行都选中，然后进行复制：  
![](http://qqadapt.qpic.cn/adapt/0/55fb1a29-eb60-01df-fd6b-9927b4e1aa94/800?pt=0&ek=1&kp=1&sce=0-12-12)  
在subl中对插入行进行正确的缩进：  
![](http://qqadapt.qpic.cn/adapt/0/dcc29832-d9a8-4319-8e48-fb25ec87a55a/800?pt=0&ek=1&kp=1&sce=0-12-12)  
然后按Cmd-Shift-v (Win: Ctrl-Shift-v) 进行自适应缩进的粘贴：  
![](http://qqadapt.qpic.cn/adapt/0/4231540b-f2cf-34e8-f11a-d464f3840a67/800?pt=0&ek=1&kp=1&sce=0-12-12)  
这样的粘贴方式不但能自适应缩进，还能自动将空格或Tab缩进转换成适应你代码的格式。  

3. 快速创建新文件 (AdvancedNewFile)  
我在使用ANF之前最快的创建新文件的方法是这样的：  
Cmd-n (Win: Ctrl-n) 打开编辑窗格：  
![](http://qqadapt.qpic.cn/adapt/0/c9ca597f-e2c6-538f-df16-984c91a504e1/800?pt=0&ek=1&kp=1&sce=0-12-12)  
然后Cmd-Shift-p (Win: Ctrl-Shift-p) 打开Command Palette，如果我想写ruby代码，我就敲ssru：  
![](http://qqadapt.qpic.cn/adapt/0/feac32fe-ae6b-e6ef-3224-9cc37a8e76b7/800?pt=0&ek=1&kp=1&sce=0-12-12)  
回车后我的文档就变成Ruby语法的了，这个时候保存文件就会自动提供.rb的后缀名：  
![](http://qqadapt.qpic.cn/adapt/0/da4c3fbc-bc15-8f07-9cfc-0333d972c673/800?pt=0&ek=1&kp=1&sce=0-12-12)  
不过这样的流程还是太繁琐了。我推荐安装使用AdvancedNewFile插件代替原有的新建文件功能。  
新的流程如下：  
比如我有这样一个project：  
![](http://qqadapt.qpic.cn/adapt/0/ab6d33af-9494-3da9-0319-16a0b1d27ce2/800?pt=0&ek=1&kp=1&sce=0-12-12)  
我想在script目录下建立一个utils文件夹，然后再在utils里面建立一个API.js文件，我只要按 Cmd-Opt-n (Win: Ctrl-Alt-n) 打开一个路径输入框：  
![](http://qqadapt.qpic.cn/adapt/0/a8f020ab-a1bc-65d9-1572-814316748240/800?pt=0&ek=1&kp=1&sce=0-12-12)  
然后输入script/utils/API.js回车就可以自动创建目录结构以及空文件。由于我们打开了script/app.js文件，我们可以直接输入./utils/API.js创建相对路径的文件结构。另外，对于已存在的目录可以使用Tab补全。创建出来的新文件会自动打开，并且会自动选择相应的语法，没有额外的工作。  

4. 更改HTML标签  
我之前更改HTML标签时要么就用上面更改变量名的方式选中一组标签，要么就手动按着Cmd (Win: Ctrl)不放双击标签的开头和结尾：  
![](http://qqadapt.qpic.cn/adapt/0/9287c71e-d03f-6573-400b-344cd7f63bdb/800?pt=0&ek=1&kp=1&sce=0-12-12)  
但是如果标签中间内容很多，这样的方式会比较费时。Emmet插件提供了一个非常方便的快捷键能够快速选择对应的一组标签名。首先将光标移至标签的开头或结尾：  
![](http://qqadapt.qpic.cn/adapt/0/3a08c4a3-53ce-809d-7e5e-963c6a058685/800?pt=0&ek=1&kp=1&sce=0-12-12)  
然后按Cmd-Shift-K (Win: Ctrl-Shift-') 就能选中这组标签：  
![](http://qqadapt.qpic.cn/adapt/0/3778d561-75b9-67b5-6265-c8ce37cd9d4f/800?pt=0&ek=1&kp=1&sce=0-12-12)  

5. CSS快速键入  
Emmet插件还提供了很多非常方便的CSS Snippets。比方说我们要敲出font-size: 1.8em;其中1.8是根据一个值计算得来的，比如说是3.6/2的结果，我们可以用Emmet进行这种简单的数值计算。  
键入fz3.6/2：  
![](http://qqadapt.qpic.cn/adapt/0/c5582920-2a2d-ea4f-7844-b68a2296ce0b/800?pt=0&ek=1&kp=1&sce=0-12-12)  
按Cmd-Shift-Y (Win: Ctrl-Shift-Y)计算数值：  
![](http://qqadapt.qpic.cn/adapt/0/39b3d0d4-f958-47e3-1c43-c0b2461a00e3/800?pt=0&ek=1&kp=1&sce=0-12-12)  
然后按Tab展开Snippet：  
![](http://qqadapt.qpic.cn/adapt/0/b981ba2c-b367-1177-1130-80362ba327ac/800?pt=0&ek=1&kp=1&sce=0-12-12)  

6. 2空格-4空格缩进快速切换  
我之前用别人代码的时候总是遇到缩进空格数跟我不同的情况，后来我学会一种方法能够处理这样的文件。比如我要将4空格缩进转成2空格缩进，首先将目标代码复制到一个独立的编辑窗口中：  
![](http://qqadapt.qpic.cn/adapt/0/1722bfd7-7d4e-621e-5fcd-61c8dcbf99e4/800?pt=0&ek=1&kp=1&sce=0-12-12)  
然后在编辑器右下角的缩进选项菜单中选择Tab Width: 4：  
![](http://qqadapt.qpic.cn/adapt/0/46ef049a-d67b-7afa-89b4-3945f82d8224/800?pt=0&ek=1&kp=1&sce=0-12-12)  
然后在编辑器右下角的缩进选项菜单中选择Convert Indentation to Tabs：  
![](http://qqadapt.qpic.cn/adapt/0/0b4e093d-368e-0935-5113-92f6b4cd1c2c/800?pt=0&ek=1&kp=1&sce=0-12-12)  
然后在编辑器右下角的缩进选项菜单中选择Tab Width: 2：  
![](http://qqadapt.qpic.cn/adapt/0/69131a1e-ce89-ccb1-3740-aa2947c47e9e/800?pt=0&ek=1&kp=1&sce=0-12-12)  
然后在编辑器右下角的缩进选项菜单中选择Convert Indentation to Spaces：  
![](http://qqadapt.qpic.cn/adapt/0/fc7f9e08-5cd0-1901-fd30-978a852812ea/800?pt=0&ek=1&kp=1&sce=0-12-12)  
然后你的文档就变成2空格缩进的了：  
![](http://qqadapt.qpic.cn/adapt/0/036f6ded-538a-faf8-d247-a51103653f46/800?pt=0&ek=1&kp=1&sce=0-12-12)  
但是这样的方法太过繁琐了不是吗？于是我就写了一个宏脚本，绑定到快捷键上来做这个工作。  
打开这个链接：  
<https://gist.github.com/beaugunderson/8588871>  
把to-2.sublime-macro和to-4.sublime-macro文件下载到你Sublime Text配置目录的Packages/User路径下，然后在编辑器菜单中选择Preferences - Key Bindings - User打开用户快捷键配置文件，把Default (OSX).sublime-keymap中的内容添加到这个文件中。  
然后你就可以用Ctrl-2或Ctrl-4转换文件的缩进空格数了。  

7. 扩展选区  
我非常喜欢Emacs的expand-region插件，ST2提供有类似的Expand Selection to Scope功能，但是不太好用，我建议安装ExpandRegion插件。  
首先把光标移到某个位置：  
![](http://qqadapt.qpic.cn/adapt/0/a6d51331-a38f-bea1-3f7d-75647a5330a6/800?pt=0&ek=1&kp=1&sce=0-12-12)  
然后按一次Cmd-Shift-Space (Win: Ctrl-Shift-Space)会选择当前的最小区域：  
![](http://qqadapt.qpic.cn/adapt/0/a3e166d6-5ea0-6f83-3ebc-a2a3d9ca827b/800?pt=0&ek=1&kp=1&sce=0-12-12)  
再按一次会向外扩展区域：  
![](http://qqadapt.qpic.cn/adapt/0/e07c15d1-a5a1-0398-8555-2a2d9101cd35/800?pt=0&ek=1&kp=1&sce=0-12-12)  
每次按都会不断地向外扩展区域，直到全选为止。  

8. 选区增强插件  
安装 MultiEditUtils 插件。  
这是一个非常强大的选区增强插件，如果你喜欢用复杂的快捷键完成高难度的编辑工作，这个插件可以提供很多方面的支持。  
详细的功能请阅读项目主页：  
[philippotto/Sublime-MultiEditUtils · GitHub](https://link.zhihu.com/?target=https%3A//github.com/philippotto/Sublime-MultiEditUtils)  

9. 代码格式化  
安装 CodeFormatter 和 SublimeAStyleFormatter 插件。使用时在 Command Palette 找 "format" 相关的命令即可。  

10. 颜色高亮  
安装 Color Highlighter，会自动高亮代码中的颜色，在写纯css的时候比较有用。  

11. 语言分析增强  
很多时候有些文件不能被 Sublime Text 准确识别出相应的语言，比如不带後缀名的配置脚本之类。这时可以使用 ApplySyntax 插件，参照默认配置进行调整就能识别这些特殊情况了。  

12. Windows 下输入法支持  
如果遇到输入法的输入栏不在光标位置的问题，可以安装 IMESupport 插件解决。  

13. 忽略依赖目录  
有时候我们要用 Sublime Text 的文件检索功能找到特定的文件，如果项目目录下面有 node_modules、bower_components 之类的文件夹则会影响输出结果，再加上这些文件夹中的文件平时不会去改动，我们可以修改配置把这些目录忽略掉。  

```
"folder_exclude_patterns": [".svn",".git",".hg","CVS","node_modules","bower_components"],
```

`14. 备份/同步 Sublime Text 配置`  
如果你经常在不同的电脑用 Sublime Text，你会希望所有的配置改动都能即时同步。如果你试过直接同步整个 Packages 目录会发现有些插件实际上是有区分系统的，Mac 和 Windows 的会有不同，甚至有些插件会区别主机，直接同步这些插件会造成冲突。  
正确的同步办法在 Package Control 的官网有介绍：  
[Syncing - Package Control](https://link.zhihu.com/?target=https%3A//packagecontrol.io/docs/syncing)  
其实很简单，只对 Packages/Users 目录进行同步，Package Control 就能自行解决平台冲突了。