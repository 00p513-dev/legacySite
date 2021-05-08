---
layout: post
title: How to build a custom ROM - Part 3
preview: Many Android ROMs exist, but what if one hasn't been built for your phone? Learn how to build it yourself!
author: Amy
---

> * I'm not responsible for bricked devices, dead SD cards, thermonuclear war, or you getting fired because the alarm app failed (like it did for me...).
> * YOU are choosing to make these modifications, and if you point the finger at me for messing up your device, I will laugh at you.
> * Your warranty will be void if you tamper with any part of your device / software.

<br>

> NEVER EVER USE ROOT UNLESS STATED

#### Many Android ROMs exist, but what if one hasn't been built for your phone? Learn how to build it yourself!

In this post we are covering how to download your devices sources. You should have the ROM sources synced already and be in its directory in your terminal.

## Finding the sources

The best places to look are [LineageOS's github](https://github.com/LineageOS/) or [PixelExperience's github](https://github.com/PixelExperience-Devices). If it isn't there ask a ROM maintainer for your phone where they keep their device tree. The git repository you need will likely be labelled in the following format `device_OEM_CODENAME`.

## Downloading the device tree

Make sure you are in the ROMs directory in your terminal. Now run `git clone REPOURL device/OEM/CODENAME -b BRANCH`. Do for all dependencies needed (such as kernel and vendor sources), replacing with the path required by them.

## Adapting to your ROM

Enter the device tree's directory and open the AndroidProducts.mk file. Replace the old ROMs name with the new one, for example `lineage_channel` with `bliss_channel` for bliss. You can find out which name you need by looking at the ROMs official device trees. Now move the `rom_codename.mk` file to match and open it. Do the same here, and make sure you have the right vendor path. Again, look at other device trees for reference. Once this is done we are ready for the build!

## Summary

If you made it this far congrats! You have downloaded the device sources and adapted them for your ROM. What you should do now is go look at my next tutorial for how to build the ROM. The commands you learnt today are:

1. `git clone REPOURL device/OEM/CODENAME -b BRANCH`

<br>
