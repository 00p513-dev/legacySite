---
layout: post
title: How to build a custom ROM - Part 1
preview: Many Android ROMs exist, but what if one hasn't been built for your phone? Learn how to build it yourself!
author: Amy
---

> * I'm not responsible for bricked devices, dead SD cards, thermonuclear war, or you getting fired because the alarm app failed (like it did for me...).
> * YOU are choosing to make these modifications, and if you point the finger at me for messing up your device, I will laugh at you.
> * Your warranty will be void if you tamper with any part of your device / software.

<br>

> NEVER EVER USE ROOT UNLESS STATED

#### Many Android ROMs exist, but what if one hasn't been built for your phone? Learn how to build it yourself!

In this post we are covering setting up a Ubuntu machine for building Android ROMs. This only has to be done once per machine, and we will be using Ubuntu 20.04.

## Installing necessary packages

1. Open a terminal
2. Run: `sudo apt install bc bison build-essential ccache curl flex g++-multilib gcc-multilib git gnupg gperf imagemagick lib32ncurses5-dev lib32readline-dev lib32z1-dev liblz4-tool libncurses5 libncurses5-dev libsdl1.2-dev libssl-dev libxml2 libxml2-utils lzop pngcrush rsync schedtool squashfs-tools xsltproc zip zlib1g-dev -y`
3. (Only for Ubuntu 18.04 - DO NOT RUN ON 20.04!) Run: `sudo apt install libwxgtk3.0-dev -y`

Packages are now installed and you are ready to proceed to the next section.

## Installing repo

1. Make sure you are in a terminal
2. Run `mkdir -p ~/bin`
3. Run `curl https://storage.googleapis.com/git-repo-downloads/repo > ~/bin/repo`
4. Run `chmod a+x ~/bin/repo`
5. Run `source ~/.profile`

Repo is now setup ready to sync ROM sources.

## Configure git identity

1. Run `git config --global user.email "you@example.com"` replacing with your email address
2. Run `git config --global user.name "Your Name"` replacing with your full name

Git is now ready to go.

<br>
