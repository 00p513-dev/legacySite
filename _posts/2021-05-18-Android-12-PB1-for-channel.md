---
layout: post
title: Android 12 Public Beta 1 for channel (moto g7 play)
preview: Android 12 is going to be the next major version of Android. Learn how to install Public Beta 1 on your Moto g7 Play with this guide.
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
* [GSI by Google - mirrored on my Telegram channel](https://t.me/amyGSI)

For Android 12 Extensions:
* [Magisk](https://github.com/topjohnwu/Magisk/releases/tag/v23.0)
* [Android 12 Extensions module](https://github.com/kdrag0n/android12-extensions/releases/)


## Installation
1. Download all files above. Then proceed to the next steps.
2. [Repartition your phone](http://www.amygrace.tk/2021/03/04/repartition-channel.html)
3. Extract the ZIP archive
4. Run `fastboot flash system system.img` to install the system image. This cannot be done in official TWRP due to it not knowing about the repartition!
5. Format data (`fastboot -w` works)
6. Enjoy Android 12! No other fixes are needed at this time!

## Android 12 Extensions
1. Download Magisk and install in TWRP
2. Open Magisk app and install "Riru", "Riru - LSPosed" and the Android 12 Extensions module. Reboot after installation.
3. Wait for LSPosed to appear in app drawer, then enable the Android 12 Extensions Xposed module. You will need to enable for SystemUI, so you may have to show system apps.
4. Reboot and open Android 12 Extensions. Everything *should* be working now :)

<br>
