---
layout: page
title: SVG渐变加移动
excerpt_separator: "<!--more-->"
categories:
    - SVG笔记  
tags:
  - svg
---  
 leywords:渐变，移动
<!--more-->  
  
##### 颜色渐变的方块  
<head>
  <meta charset="UTF-8">
<style> 
.stal
{
width:100px;
height:100px;
background:white;
animation:stal 5s;
animation-iteration-count: infinite;
}

@keyframes stal
{
from {background:white;}
to {background:yellow;}
}



</style>
</head>
<body>

<div class="stal"></div>
</body>  
  
  
    
	  
  
  
##### 颜色渐变且移动的方块  
<head>
  <meta charset="UTF-8">
<style> 
div
.kry
{
width:100px;
height:100px;
background:red;
position:relative;
animation:kry 5s linear 2s infinite alternate;
}

@keyframes kry
{
0%   {background:red; left:0px; top:0px;}
100%  {background:green; left:200px; top:0px;}
}
</style>
</head>
<body>
<div class="kry">我是个方块</div>

</body>  
  
  
  
  
  
  
  
  
  
  
  
---  
在 CSS 中，background-position 属性是 可动画化（animatable） 的。
Internet Explorer 10、Firefox 和 Opera 支持 CSS 动画。
Safari 和 Chrome 通过带有前缀 -webkit-，支持 CSS 动画  
  
  增加animation动画效果并设置好position即可实现移动  
      
   
  
#### 关于animation（动画） 属性：  
- 语法  
animation: name duration timing-function delay iteration-count direction fill-mode play-state;  
- 值  
1.animation-name：指定要绑定到选择器的关键帧的名称  
2.animation-duration：动画指定需要多少秒或毫秒完成  
3.animation-timing-function：设置动画将如何完成一个周期  
4.animation-delay：设置动画在启动前的延迟间隔。  
5.animation-iteration-count：定义动画的播放次数。  
6.animation-direction：指定是否应该轮流反向播放动画。  
7.animation-fill-mode：规定当动画不播放时（当动画完成时，或当动画有一个延迟未开始播放时），要应用到元素的样式。  
8.animation-play-state：指定动画是否正在运行或已暂停。  
9.initial：设置属性为其默认值。  
10.inherit：从父元素继承属性。  


