---
title: Motors@Work kW Ratio - Voltage Based
layout: helpfile
categories: ['my-motors']
permalink: kw-ratio-voltage-based/
sequence: 1
tags:
- my-motors
---
## kW Ratio - Voltage Based

If the [motor load](/motor-load) cannot be determined using kW Ratio – Power based method,
Motors@Work will attempt to calculate it using the kw Ratio - Voltage Based method.

When using the kW ratio - voltage based method, the motor load is determined with the following
formula

{% highlight java%}
((averageVoltageaverageCurrent(powerFactor/100)0.001732) / ((motor.motorSize.numericValue.746)/(motor.efficiency/100)))*100
{% endhighlight %}
