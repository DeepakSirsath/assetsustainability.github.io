---
title: Motors@Work kW Ratio - Power Based
layout: helpfile
categories: ['my-motors']
permalink: kw-ratio-power-based/
sequence: 1
tags:
- my-motors
---
## kW Ratio - Power Based

The first option Motors@Work uses to calculate [motor load](/motor-load) is kw Ratio - Power Based.

When using the kW ratio - power based method, the motor load is determined with the following
formula

{% highlight java%}
(powerDraw/((motorSize.746)/(motor.efficiency/100)))100
{% endhighlight %}
