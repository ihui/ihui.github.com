---
layout: post
title: "matlab text function"
description: matlab, text
date: 2013-08-27 22:12
comments: true
categories: programming
---
As you know, it is easy to plot a set of 2D discrete points with matlab *plot* function. I usually do many plots to find data's implication, terrace slop, for example. When the slop changes abruptly at a point,  that point should be found. It's not a easy work when the amount of points is huge without any label. So, the third column (labels) are printed for every point is a good way to look for that point.  
  
The function *text* can be used to print labels for points with a loop as below:  

> for i=1:length(x)  
> 　text(x(i),y(i), num2str(label(i)))  
> end
   
Reference:  
[http://blog.csdn.net/ccxcau/article/details/7362890](http://blog.csdn.net/ccxcau/article/details/7362890)