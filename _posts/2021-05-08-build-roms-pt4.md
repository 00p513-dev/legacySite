---
layout: post
title: How to build a custom ROM - Part 4
preview: Many Android ROMs exist, but what if one hasn't been built for your phone? Learn how to build it yourself!
author: Amy
---

> * I'm not responsible for bricked devices, dead SD cards, thermonuclear war, or you getting fired because the alarm app failed (like it did for me...).
> * YOU are choosing to make these modifications, and if you point the finger at me for messing up your device, I will laugh at you.
> * Your warranty will be void if you tamper with any part of your device / software.

<br>

> NEVER EVER USE ROOT UNLESS STATED

#### Many Android ROMs exist, but what if one hasn't been built for your phone? Learn how to build it yourself!

In this post we are covering how to do the build. You should have completed all previous tutorials.

## Setting up the environment

Make sure you are in the top directory and run `. build/envsetup.sh`. This will setup the environment ready for building android, and give you access to other commands you will need. 

## Starting the build

1. Run `lunch rom_codename-userdebug`. This tells the build system which device you wish to build for.
2. Run `mka bacon`. This is the final build! This command takes around 6 hours to complete on my own computer, speed varies based on specs. If you get an error such as `Target "bacon" not found` check your ROMs documentation for which command you need to use.
3. Get help! If the build failed ask in the "Android Builders Help" group on telegram for assistance. Make sure you follow the error template.

## Testing the build

If your build completed successfully, you now have to flash it to your phone! The flashable zip should be in `out/target/product/CODENAME`.

## Summary

If you made it this far congrats! You have built an entire ROM! You can now upload this to [Sourceforge](https://sourceforge.net), [AndroidFileHost](https://androidfilehost.com), or anywhere you choose and share on [XDA](https://forum.xda-developers.com) or [Telegram](https://telegram.org). Commands learnt this post:

1. `. build/envsetup.sh` to initialise the environment.
2. `lunch rom_codename-userdebug` to tell the build system which device you wish to build for.
3. `mka bacon` to build the final package.

<br>
