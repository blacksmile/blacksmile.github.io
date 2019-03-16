---
layout: post
title: "【前端开发】CSS用text-overflow实现文本标题超出显示省略号“...”"
date: 2014-05-14 08:56:13
categories: 【前端开发】
tags:
- text-overflow
---
**注意：overflow: hidden; text-overflow:ellipsis;white-space:nowrap;一定要一起用**

> 1.一定要给容器定义宽度.
> 2.如果少了overflow: hidden;文字会横向撑到容易的外面
> 3.如果少了white-space:nowrap;文字会把容器的高度往下撑；即使你定义了高度，省略号也不会出现，多余的文字会被裁切掉
> 4.如果少了text-overflow:ellipsis;多余的文字会被裁切掉，就相当于你这样定义text-overflow:clip.
> 如果容器是table，当文字内容过多时，不换行，而是出现...
> 5.一定要给table定义table-layout:fixed;和设置宽width：40px;只有定义了表格的布局算法为fixed，下面td的定义才能起作用。