---
title: Motors@Work Voltage Compensated Amps Ratio
layout: helpfile
categories: ['my-motors']
permalink: voltage-compensated-amps-ratio/
sequence: 1
tags:
- my-motors
---
## Voltage Compensated Amps Ratio

If the [motor load](/motor-load) cannot be determined using kW Ratio – Power based or
kW Ratio – Voltage based Motors@Work will attempt to calculate the motor load
using Voltage Compensated Amps Ratio strategy.

Using voltage compensated amps ratio, the motor load is determined with the following
formula

{% highlight java%}
(averageCurrent/motor.ampsFullLoad) * (averageVoltage/motor.wiredFor.numericValue) * 100
{% endhighlight %}
