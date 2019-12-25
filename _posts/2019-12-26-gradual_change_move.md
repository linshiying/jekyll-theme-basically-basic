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
25%  {background:green; left:200px; top:0px;}
50%  {background:yellow; left:200px; top:200px;}
75%  {background:black; left:0px; top:200px;}
100% {background:red; left:0px; top:0px;}
}
</style>
</head>
<body>
<div class="kry">动起来</div>

</body>
