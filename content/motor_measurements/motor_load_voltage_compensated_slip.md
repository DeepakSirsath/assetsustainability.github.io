---
title: Motors@Work Voltage Compensated Slip
layout: helpfile
categories: ['my-motors']
permalink: voltage-compensated-slip/
sequence: 1
tags:
- my-motors
---
## Voltage Compensated Slip

If the load on a motor cannot be determined using kW Ratio – Power based,
kW Ratio – Voltage based, or Voltage Compensated Amps Ratio strategies,
Motors@Work will attempt to calculate the motor load using Voltage Compensated
Slip.

Using voltage compensated slip, the motor load is determined with the following
formula

{% highlight java%}
((motor.synchronousSpeed.numericValue - measuredSpeed ) / ((motor.synchronousSpeed.numericValue - motor.speedFullLoad) * Math.pow((motor.wiredFor.numericValue/averageVoltage),2)))*100
{% endhighlight %}
