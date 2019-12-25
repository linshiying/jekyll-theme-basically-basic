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
