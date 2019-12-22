---
layout: page
title: 只用几行CSS代码就改变内容的显示方式！  
excerpt_separator: "<!--more-->"
categories:
    - 网站设计
---   

神奇的媒体查询，unbelieveable! 仅仅需要几行代码就可以改变内容的显示方式！  
---   
  
<!--more-->  
## 什么是媒体查询？  
利用媒体查询，可以根据设备的能力应用特定的CSS样式。比如，根据视口宽度、屏幕宽高比和朝向（水平或垂直）  
媒体查询包含媒体类型和零个或多个检测媒体特性的表达式。Width、height和color都是可用于媒体查询的特性。使用媒体查询，可以不必修改内容本身，而让网页适配不同的设备。[参考资料]（http://www.w3.org/TR/css3-mediaqueries/)  
  
## 媒体查询语句结构  
媒体查询语句一般由media type+一到多个CSS属性判断组成，而多个CSS属性判断可以用关键字and连接：  
```  
@media screen and (min-width:1024px) and (max-width:1280px){
	body{font-size:medium;}
}  
```  
其中media type可以省略，属性值也可以为空：  
```
@media (color:4){}
@media (color){}  
```  
而针对多个媒体类型的CSS规则，可以用逗号来隔开：  
```  
@media handheld and (min-width:360px),screen and (min-width:480px){
body{font-size:large;}
}  
```  
```  
@media screen and (min-width:800px),print and (min-width:7in){
body{font-size:small;}
}  
```  
  
## 总结
CSS 3的媒体查询是一个十分强大且便利的工具，它的存在为我们在不同的设备下实现丰富的界面提供了一便利的方法，我相信随着移动互联网的快速发展，media queries也会很好发挥自己的作用。