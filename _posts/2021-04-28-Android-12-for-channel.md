---
layout: post
title: Android 12 for channel (moto g7 play)
preview: Android 12 is going to be the next major version of Android. Learn how to install Developer Preview 2 on your Moto g7 Play with this guide.
author: Amy
---

> * I'm not responsible for bricked devices, dead SD cards, thermonuclear war, or you getting fired because the alarm app failed (like it did for me...).
> * YOU are choosing to make these modifications, and if you point the finger at me for messing up your device, I will laugh at you.
> * Your warranty will be void if you tamper with any part of your device / software.

#### Android 12 is going to be the next major version of Android. Learn how to install on your Moto g7 Play with this guide.

## Features
* The latest and greatest from Android
* Experience in development features with an optional Magisk module
* Multi-language support

## Bugs
* Randomised MAC

## Downloads
* [SGSI by Erfan](https://mirrors.lolinet.com/firmware/gsi/Pixel/Pixel-AB-S-20210318-ErfanGSI.img-0247.7z)
* [Internal storage fix](https://github.com/00p513-dev/ErfanGSIs-channel/releases/tag/internal-fix)
* [TWRP](https://eu.dl.twrp.me/channel/)

For Android 12 Extensions:
* [Magisk](https://github.com/topjohnwu/Magisk/releases/tag/v22.1)
* [Android 12 Extensions module](https://github.com/kdrag0n/android12-extensions/releases/tag/v2.0.2)


## Installation
1. Download all files above. Then proceed to the next steps.
2. [Repartition your phone](http://www.amygrace.tk/2021/03/04/repartition-channel.html)
3. Extract the 7z SGSI archive
4. Run `fastboot flash system Pixel-AB-S-20210318-ErfanGSI.img` to install the system image. This cannot be done in official TWRP due to it not knowing about the repartition!
5. Format data (`fastboot -w` works)
6. Reboot to TWRP with `fastboot boot twrp-3.5.2_10-0-channel.img`
7. Flash the Internal Storage fix
8. Reboot to system and apply [the GMS fix](http://www.amygrace.tk/2021/03/04/fix-gms-ports.html)
9. Enjoy Android 12!

## Halp my wifi no work halp amy maam
When connecting, click "Advanced", "Use Device MAC" instead of random

## Android 12 Extensions
1. Download Magisk and install in TWRP
2. Open Magisk app and install "Riru", "Riru - LSPosed" and the Android 12 Extensions module. Reboot after installation.
3. Wait for LSPosed to appear in app drawer, then enable the Android 12 Extensions Xposed module. You will need to enable for SystemUI, so you may have to show system apps.
4. Reboot and open Android 12 Extensions. Everything *should* be working now :)

<br>
