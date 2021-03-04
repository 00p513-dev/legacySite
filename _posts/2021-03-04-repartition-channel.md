---
layout: post
title: How to repartition your Moto g7 Play
preview: The Moto g7 Play is a great value device, with awesome development capabilities. Sadly the system partition is too small for some images. Learn how to repartition your device with the steps below.
author: Amy
---

> * I'm not responsible for bricked devices, dead SD cards, thermonuclear war, or you getting fired because the alarm app failed (like it did for me...).
> * YOU are choosing to make these modifications, and if you point the finger at me for messing up your device, I will laugh at you.
> * Your warranty will be void if you tamper with any part of your device / software.

#### The Moto g7 Play is a great value device, with awesome development capabilities. Sadly the system partition is too small for some images. Learn how to repartition your device with the steps below.

<br> 

## Downloads
* [LineageOS (recovery and zip)](https://download.lineageos.org/channel)
* [ocean.bin](https://sourceforge.net/amys-roms/files/Moto-GPTs/)

## Installation
1. Download all files above. Then proceed to the next steps.
2. `fastboot flash gpt ocean.bin`
3. `fastboot flash boot lineage-recovery.img` (replace with your image name)
4. Reboot to Lineage recovery and flash LineageOS.
5. Format data
6. Reboot to system and follow setup

<br>
