---
title: First RF range test!
date: 2020-07-01
description: Measuring SNR of 250 m link in urban area.
categories:
  - update
  - technical
  - radio
image: https://source.unsplash.com/t3HVjP4xNsg/2000x1322?a=.png
author_staff_member: matthias
---
We used our satellite model to send packets with -10 dBm, which is only 0.0001 watts. In space, we will send with 20 dBm, which is 1000x more powerful.
![SDR Screenshot](/images/mc10dbsmall.jpg)
![Antenna pointing](/images/antennamcsmall.jpg)


We used a commercial off the shelf (COTS) SDR (Signal Defined Radio) from NESDR and our proven high gain ground antenna.
From this 250 m link in urban area, we get around 20 dB of SNR, which will allow us to receive up to 50 dB with 20dBm.
This and coding will allow us enough link budget for long range communications to LEO. 
