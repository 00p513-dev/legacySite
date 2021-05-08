---
layout: post
title: How to build a custom ROM - Part 2
preview: Many Android ROMs exist, but what if one hasn't been built for your phone? Learn how to build it yourself!
author: Amy
---

> * I'm not responsible for bricked devices, dead SD cards, thermonuclear war, or you getting fired because the alarm app failed (like it did for me...).
> * YOU are choosing to make these modifications, and if you point the finger at me for messing up your device, I will laugh at you.
> * Your warranty will be void if you tamper with any part of your device / software.

<br>

> NEVER EVER USE ROOT UNLESS STATED

#### Many Android ROMs exist, but what if one hasn't been built for your phone? Learn how to build it yourself!

In this post we are covering how to `sync` the ROMs sources.

## Initialising the source

`repo` has many options to setup the ROM sources. Luckily most are not needed. The most basic way of initialising a ROM sources is: `repo init -u ROMMANIFEST -b BRANCH` in an empty directory replacing ROMMANIFEST with the manifest url and BRANCH with the branch you want. For example `repo init -u https://github.com/crdroidandroid/android -b 11.0`

We can also add `--depth=1` to save space and internet bandwidth, as we are only downloading the latest code, and not the entire history of Android. For example our command from earlier would become `repo init -u https://github.com/crdroidandroid/android -b 11.0 --depth=1`

## Syncing the source

This is another command that can be simple, but gets more complicated. All that is needed is `repo sync` however this is very slow. A quicker method would be to add multiple jobs with `-jX` where X is the number of jobs. So our command becomes `repo sync -j10` if we want 10 jobs. But wait? What if something changed and it won't sync anymore? This is why we recommend to do a force sync with `--force-sync`. So now are command becomes `repo sync -j10 --force-sync`.

## Summary

If you made it this far congrats! You have downloaded the source code for the Android ROM you wish to build for the first time! What you should do now is go look at my next tutorial to learn how to get the device specific sources. The commands you learnt today are:

1. `repo init -u ROMMANIFEST -b BRANCH --depth=1` to initialise repo
2. `repo sync -j10 --force-sync` to sync sources

<br>
