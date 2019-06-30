---
layout: page
title: svg的学习笔记
excerpt_separator: "<!--more-->"
categories:
  - 学习笔记
---
## SVG可以通过这几种方式置入网页中<br>
<li>img标签<br>
<li>object标签<br>
<li>设置为背景图像<br>
<li>内联<br>
img标签是直接使用img src=""的形式进行，而object是通过使用<object>标签从而达到目的，通过此方式可以让网页上的Java进行识别。对于设置背景图像进行置入则与插入其余图片格式别无出入，但可以通过css中来进行选择器的调整其格式等。内联则是通过xml的在html中的直接书写应用，可以在内部和外部对svg进行调整。<br>

| | img标签插入 | object标签插入 | 
| ------ | ------ | ------ |
| SMIL动画 | Y | Y |
| 外部css控制| N| *1 |
|内部css控制|Y|Y|
|通过Javascript控制|N|Y|
|缓存|Y|Y|
|SVG内部的媒体查询|Y|Y|
|使用use|N|Y|

| | 内联 | 背景图片 | 
| ------ | ------ | ------ |
| SMIL动画 | Y| Y |
| 外部css控制| Y |N |
|内部css控制|Y|Y|
|通过Javascript控制|Y|N|
|缓存|*2|Y|
|SVG内部的媒体查询|*3|Y|
|使用use|Y|N|
 
* 1 使用object这一标签插入的时候，通过外部样式形式的时候需要在SVG的文件夹内添加。<br>
* 2 通过外部资源引入时，IE浏览器默认不支持。<br>
* 3 内联svg的媒体查询其对象是文档中的大小而不是svg的auto。