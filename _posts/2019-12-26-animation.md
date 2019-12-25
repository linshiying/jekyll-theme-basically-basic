---
layout: page
title: SVG与CSS搭配完成的animation
excerpt_separator: "<!--more-->"
categories:
    - SVG笔记
---  
 标签：SVG CSS animation 
<!--more-->  
   
- 首先看一个会变色方块  
   
<style> 
div
{
	width:100px;
	height:100px;
	background:red;
	animation:myfirst 5s;
	-webkit-animation:myfirst 5s; /* Safari and Chrome */  
	animation-direction:normal;
}

@keyframes myfirst
{
	from {background:red;}
	to {background:yellow;}
}

@-webkit-keyframes myfirst /* Safari and Chrome */
{
	from {background:red;}
	to {background:yellow;}
}
</style>  
 <div></div> 
  
  
  
  
  
  
- 然后是不仅会变色而且还会移动的方块  
<style> 
div
{
	width:100px;
	height:100px;
	background:red;
	position:relative;
	animation-name:myfirst;
	animation-duration:5s;
	animation-timing-function:linear;
	animation-delay:2s;
	animation-iteration-count:infinite;
	animation-direction:alternate;
	animation-play-state:running;
	/* Safari and Chrome: */
	-webkit-animation-name:myfirst;
	-webkit-animation-duration:5s;
	-webkit-animation-timing-function:linear;
	-webkit-animation-delay:2s;
	-webkit-animation-iteration-count:infinite;
	-webkit-animation-direction:alternate;
	-webkit-animation-play-state:running;
}

@keyframes myfirst
{
	0%   {background:red; left:0px; top:0px;}
	25%  {background:yellow; left:200px; top:0px;}
	50%  {background:blue; left:200px; top:200px;}
	75%  {background:green; left:0px; top:200px;}
	100% {background:red; left:0px; top:0px;}
}

@-webkit-keyframes myfirst /* Safari and Chrome */
{
	0%   {background:red; left:0px; top:0px;}
	25%  {background:yellow; left:200px; top:0px;}
	50%  {background:blue; left:200px; top:200px;}
	75%  {background:green; left:0px; top:200px;}
	100% {background:red; left:0px; top:0px;}
}
</style> 
<div></div>