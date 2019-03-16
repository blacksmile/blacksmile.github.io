---
layout: post
title: "【前端开发】HTML CSS中常遇到的bug一些注意事项总结"
date: 2014-04-07 22:32:41
categories: 【前端开发】
tags:
- HTML&CSS bug注意事项
---
1、IE6下横向双倍`margin bug` (触发条件：块属性标签；`float`；横向`margin`设置；IE6下。解决办法：css中加入`display:inline`。)  
2、css中公用属性首先声明；如对浏览器对某些标签有默认的`margin`和`padding`值首先声明默认值为0。  
3、css中class类名必须有实际的意义，必须与内容相关；不得用纯数字用于class类名。  
4、IE6下标签嵌套时，如果内层标签float，只有清除内层标签的浮动后外层标签才能被撑开。  
5、清除浮动时用div而不用其它标签清除浮动；  
 `.clear {height:0;clear:both;overflow:hidden;}`  
6、IE6下定义1px的高度或定义小于等于10px的高度；IE6下默认行高是10px，解决办法是：`overflow：hidden / zoom:0.08 / line-height:1px`。  
7、超链接点击过后就不在出现hover样式？解决方法是：改变`css属性的排列顺序L--V--H--A`。  
8、使用群组选择器时，class名之间必须用空格隔开，否则`firefox`将不会读取CSS命令。  
9、a标签中嵌套img时，必须有`a{dispaly:block;}`否则在IE6下将影响布局（即在图片下方多出一部分空白）。  
10、a标签中嵌套img时，img默认会有1px的`border`，需要在CSS中加入`a img {border:none;}`。  
11、a标签中嵌套img时，a标签必须为块属性（即`display:block;`）否则在IE6下图片下方会多出一部分，影响布局。  
12、在进行`position`定位时如果是标签嵌套时定位必须将父标签里的浮动全部清除，子标签的浮动后的CSS样式才能在IE6下被读出。  
13、通过改变后缀名改变图片格式的图片在IE6下读不出，在其他浏览器下将以原来的格式解析图片。  
14、li 中嵌套img  img需要`float`否则在IE6下  img下方会多出一部分  有空隙。  
15、在IE6下使用`position`定位，内标签必须清除浮动，否则定位的标签将无法显示。  
16、未使用`float`浮动时，内层标签的`margin`值撑不开外层标签，而内层标签的`padding`值则可以撑开。  
17、标签嵌套时，如果父子标签均浮动，子标签就不用清除浮动。  
18、logo外层需要用H1标签嵌套。  
19、在后台无法改动css，改动css需要改代码，所以`需要更换的图片使用img标签`。  