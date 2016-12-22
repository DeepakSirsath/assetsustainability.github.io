---
title: Motors@Work Motor Measurement - Power Factor
layout: helpfile
categories: ['motor-measurement']
permalink: motor-measurement-power-factor/
sequence: 1
tags:
- motor-measurement
---
## Motor Measurement: Power Factor (PF)

Power Factor is the ratio of real power to apparent power for an electrical system.

Motors@Work uses power factor [measurements](/motor-measurement) in load and efficiency analytics.

Motors@Work generated priority 1 alerts for [low power factor](/low-power-factor) conditions.  Motors@Work always considers the absolute value of the power factor.

For motor load calculation, power factor must be greater than 1.  If less than one, Motors@Work considers the reading to be power factor from instrumentation.

###Low Power Factor Settings

#### <a name="PowerFactorAlertThreshold"></a> Power Factor Alert Threshold
Override the power factor below which a priority 1 alert occurs.  Specify the value as a percentage (i.e. power factor of .95 = 95% - user would enter 95).  Since Motors@Work always considers the absolute value of the power factor, a reading of -94 would trigger an alert.  A reading of -96 would not (assuming user still has default value of 95 as the threshold).

To change the reading, open the Setup \| Settings page.  Find the 'Power Factor Alert Threshold' setting and change as necessary.  The default value is 95 which corresponds to the NEMA recommendation.  A setting of 1 means each low power factor reading creates a priority 1 alert.

#### <a name="ConsecutiveLowPowerFactorReadings"></a> Consecutive Low Power Factor Trigger
Automated readings may produce skewed power factor readings while a motor is starting up.  For that reason, Motors@Work allows users to set the number of low readings that will create a priority 1 alert.

To change the reading, open the Setup \| Settings page.  Find the 'Consecutive
Low Power Factor Trigger' setting and change as necessary.  The default value is 1
which means each low power factor reading creates a priority 1 alert.
