---
layout: post
title: direct from rmd
author: "Andy South"
date: "Thursday, November 20, 2014"
output: md_document
published: true
status: publish
---
 
 
TEST
 

{% highlight r %}
summary(cars)
{% endhighlight %}



{% highlight text %}
##      speed           dist       
##  Min.   : 4.0   Min.   :  2.00  
##  1st Qu.:12.0   1st Qu.: 26.00  
##  Median :15.0   Median : 36.00  
##  Mean   :15.4   Mean   : 42.98  
##  3rd Qu.:19.0   3rd Qu.: 56.00  
##  Max.   :25.0   Max.   :120.00
{% endhighlight %}
 
You can also embed plots, for example:
 
![plot of chunk unnamed-chunk-2](/figures/unnamed-chunk-2-1.png) 
 