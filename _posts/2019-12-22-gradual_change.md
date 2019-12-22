---
layout: page
title: 学习使用CSS3制作渐变背景，让你的个人简历背景变得亮眼不再是梦
excerpt_separator: "<!--more-->"
categories:
    - 学习笔记
---  
使用CSS制作渐变背景，让你的网页背景变得更加美观  
<!--more-->  
##  使用CSS3制作渐变背景
##### 线性渐变语法  
```  
linear-gradient { 
background: linear-gradient(0deg, red, blue); }  
```  
第一个参数表示 从哪里开始(默认是 top), 有:top/ right/ bottom/ left，还可以用度数表示,第二个和第三个参数不限于两个，可以自己决定，组合为更好看的渐变色  
  
##### 两种渐变形状  
渐变形状有两种：圆（cicle）和椭圆（ellipse）
```  
#grad {
  background-image: radial-gradient(circle, red, yellow, green);
}  
```  
  
##### 重复的渐变  
- 重复的径向渐变：
repeating-radial-gradient() 函数用于重复径向渐变：  
```  
#grad {
  background-image: repeating-radial-gradient(red, yellow 10%, green 15%);
}  
```  
- 重复的线性渐变：  
repeating-linear-gradient() 函数用于重复线性渐变  
```  
#grad {
  background-image: repeating-linear-gradient(red, yellow 10%, green 20%);
}  
```  

  
##### 使用多个颜色结点  
带有多个颜色结点的从上到下的线性渐变：  
```  
#grad {
  background-image: linear-gradient(red, yellow, green);
}  
```  
  
##### 使用透明度（transparent）  
CSS3 渐变也支持透明度（transparent），可用于创建减弱变淡的效果。
为了添加透明度，我们使用 rgba() 函数来定义颜色结点。rgba() 函数中的最后一个参数可以是从 0 到 1 的值，它定义了颜色的透明度：0 表示完全透明，1 表示完全不透明。  
从左到右的线性渐变，带有透明度：  
```  
#grad {
  background-image: linear-gradient(to right, rgba(255,0,0,0), rgba(255,0,0,1));
}  
``` 