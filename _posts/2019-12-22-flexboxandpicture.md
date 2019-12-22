---
layout: page
title: 学会弹性布局+响应式图片将是成功做成某奇艺频道页面的第一步
excerpt_separator: "<!--more-->"
categories:
    - 平面设计
---  
  
标签：弹性布局。响应式图片  
<!--more-->  
  
## 什么是Flexbox？  
一种当页面需要适应不同的屏幕大小以及设备类型时确保元素拥有恰当的行为的布局方式。
引入弹性盒布局模型的目的是提供一种更加有效的方式来对一个容器中的子元素进行排列、对齐和分配空白空间。  
  
## flexbox的几个特性  
##### 1.flex-direction  
- 语法：  
flex-direction: row | row-reverse | column | column-reverse  

##### 2.justify-content 属性  
- 语法：  
justify-content: flex-start | flex-end | center | space-between | space-around  

##### 3.align-items 属性  
- 语法：  
align-items: flex-start | flex-end | center | baseline | stretch  

##### 4.flex-wrap 属性  
- 语法：  
flex-wrap: nowrap|wrap|wrap-reverse|initial|inherit;  
  
##### 5.align-content 属性  
- 语法：  
align-content: flex-start | flex-end | center | space-between | space-around | stretch  
  
## 响应式图片  
##### <picture> 元素  
HTML5 的 <picture> 元素可以设置多张图片。  
e.g.  
```  
<picture>
  <source srcset="img_smallflower.jpg" media="(max-width: 400px)">
  <source srcset="img_flowers.jpg">
  <img src="img_flowers.jpg" alt="Flowers">
</picture>  
```  
##### 不同设备显示不同图片  
大尺寸图片可以显示在大屏幕上，但在小屏幕上确不能很好显示。我们没有必要在小屏幕上去加载大图片，这样很影响加载速度。所以我们可以使用媒体查询，根据不同的设备显示不同的图片。  
```  
/* For width smaller than 400px: */
body {
    background-image: url('img_smallflower.jpg'); 
}

/* For width 400px and larger: */
@media only screen and (min-width: 400px) {
    body { 
        background-image: url('img_flowers.jpg'); 
    }
}  
```  
掌握好这些语义之后结合RWD就可以制作一个页面频道啦