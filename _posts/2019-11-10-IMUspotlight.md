---
title: Tech Spotlight IMU
date: 2019-11-10
description: Gyro Accelerometer Compass in 3x3 mm
categories:
  - update
  - technical
  - spotlight
  - sensor
image: https://source.unsplash.com/t3HVjP4xNsg/2000x1322?a=.png
author_staff_member: matthias
---
The IMU is a crucial component for attitude determination. We use the new TDK "ICM-20948" Integrated circuit, which has Nine-Axis (Gyro + Accelerometer + Compass).
![Schematic](/images/icmhighlight.png)


With this, we can know our orientation from the magnetic field, ratation information and we hope to even measure acceleration.
TDK claims it is the "World's Lowest Power 9-Axis MEMS MotionTracking Device". Therefore, we drive it with our 1.8V bus. 
Because we do not need the fastest bus, we chose I2C, which also has a low power consumption and the possiblitiy of attaching multiple sensors to the same bus. The used schematic is shown below.
It also shows the deblocking capacitors, a part of the I2C bus and connector and an interrupt connector, which allows to forward interrupts to the main processor.




