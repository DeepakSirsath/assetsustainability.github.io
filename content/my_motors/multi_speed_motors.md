---
title: Motors@Work Multi-Speed Motors
layout: helpfile
categories: ['my-motors']
permalink: multi-speed-motors/
sequence: 1
tags:
- my-motors
---
## Multi-Speed Motors

Motors@Work allows entry of multi-speed motors.

By default, a motor is considered a single speed motor and allows one entry for
synchronous speed, size, full load speed, full load amperage, and efficiency.

To designate a motor as multi-speed, click the change button next to the single speed
setting on the the motor entry screen.  Changing a motor to multi-speed allows
entry of multiple speeds, sizes, amperages and efficiencies.

Once a motor is designated as multi-speed, Motors@Work will use the appropriate
speed setting for [motor measurement](/motor-measurement) calculations by determining
the average of the amperages entered.

Motors@Work calculates the maximum amperage for each speed using the full load speed
time the service factor for the motor.  If the service factor for the motor is
empty, Motors@Work automatically uses the industry standard service factor of 1.15
to determine the maximum amperage.

Motors@Work will find the lowest setting for which the entered amperage is less
than the maximum amperage and use that setting as the basis for Voltage Compensated Slip
motor load calculations.
