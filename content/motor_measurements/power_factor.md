---
title: Motors@Work Motor Measurement - Power Factor
layout: helpfile
categories: ['motor-measurement']
permalink: motor-measurement-power-factor/
sequence: 1
tags:
- motor-measurement
---
## Motor Measurement: Power Factor

Power Factor is a measurement that can be taken by for a motor.

Motors@Work considers low power factor conditions as a priority 1 alert.  Motors@Work always considers the absolute value of the power factor.

###Low Power Factor Settings

####Power Factor Alert Threshold
Override the power factor below which a priority 1 alert occurs.  Specify the value as a percentage (i.e. power factor of .95 = 95% - user would enter 95).  Since Motors@Work always considers the absolute value of the power factor, a reading of -94 would trigger an alert.  A reading of -96 would not (assuming user still has default value of 95 as the threshold).

To change the reading, open the Setup | Settings page.  Find the 'Power Factor Alert Threshold' setting and change as necessary.  The default value is 95 which corresponds to the NEMA recommendation.  A setting of 1 means each low power factor reading creates a priority 1 alert.

####Consecutive Low Power Factor Trigger
Automated readings may produce skewed power factor readings while a motor is
starting up.  For that reason, Motors@Work allows users to set a threshold
for the number of readings that will create a priority 1 alert.

To change the reading, open the Setup | Settings page.  Find the 'Consecutive
Low Power Factor Trigger' setting and change as necessary.  The default value is 1
which means each low power factor reading creates a priority 1 alert.
