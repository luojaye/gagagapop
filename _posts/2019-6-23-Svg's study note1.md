---
layout: page
title: svg的学习笔记
excerpt_separator: "<!--more-->"
categories:
  - 学习笔记
---
# SVG
## 何为svg   
<br>  <!--more-->
可缩放矢量图形是基于可扩展标记语言(标准通用标记语言的子集)，用于描述二维矢量图形的一种图形格式。它由万维网联盟制定，是一个开放标准。通过svg可以使画面更加生动活泼，使客户舒心以及具有一定的观赏感。<br> 
一、在网页中使用svg有以下三种方式<br>
1. svg就是一种图像格式，和jpeg，gif，png等位图图像格式有所不同，所以作为svg格式的图片更多的可以被应用到网页上，例如将svg文件设置为<img>元素的src属性，或者是给任意的元素设置背景图像，或者是设置为CSS3的属性border-image。但是这种方式也存在不好的地方，就是浏览器在渲染svg图像的时候，会将svg描述的矢量图像转换成栅格图像用于显示，这就失去了svg的一部分功能，svg是文本描述的图像格式，可能会有一些引用文件，比如其他的图像文件，外部脚本或者是web字体文件，在使用这种方式渲染svg时大多数浏览器会忽略引用文件。<br>2. <object>元素可以将外部的文件嵌入到html中. <br>3. 在网页中嵌入svg，最直接的方式是将svg文件的内容直接写入html文本中，这样在网页中不仅可以显示svg图像，还可以使用脚本控制，用css添加样式，可谓是最好的做法。
二、用文档表示的图像
1.SVG的根元素。svg的根元素有width、height和viewbox属性。它们是针对于在svg的长宽以及视框而规定的属性。width和height可以控制图形的长宽但viewbox可以控制其在网页上的显示视框，定义svg所有形状所需要遵守的坐标规则。例如视框值为 1 10 100 1000视为对矩形左上角和右下角的描述则用于描述左上角的位置前两个值被称为min-x和min-y，而后两个值为右下角对应宽度和高度。<br>
2.命名是由图形编辑程序定义的命名空间（xmlns是XML命名空间的缩写。）<br>3.标题title和描述标签desc增强svg的可读性。g元素可以作为一条绳子将图形所需要的图像进行捆绑，使一个图像完整化。<br>4.svg有path、rect、circle、ellipse、line、polyline和polygon这几种形状元素。
三、使用流行的图像编辑工具和服务创建SVG
1.AI、Bohemian Coding的Sketch、Inkscape以及一些线上免费使用的工具。<br>2.利用svg图标服务。图标网站提供<br> [图标库](http://www.fontawesome.com.cn/faicons/)

