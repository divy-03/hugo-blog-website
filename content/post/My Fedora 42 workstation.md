---
title: My Fedora + Hyprland
description: My fedora 42 workstation installation

date: 2025-09-14T20:12:52+08:00
lastmod: 2025-09-14T20:12:52+08:00
tags:
  - hyprland
  - linux
categories:
  - linux
---

## Why I switched
I was getting frustrated by windows continuous usage of so much memory after only opening few browser tabs and 1 or 2 VS Code windows. 
Windows started to lag after 90% of RAM usage but my [[Hyprland]] only use about 70% of RAM after using more windows than that of windows. 
## How I installed
I remember that in my 2nd year my roommate was using mint so, first I tried installing Linux mint distro. I was following a youtube tutorial step by step, but ended up maybe corrupting my USB drive which I was using to boot into Linux Mint. I booted once into Mint but without installing it first I switched to Windows once and then was never able to boot into Mint again. 
So the Mint story ends here. 

After failing once, I didn't let it go. I then watched another fedora installation tutorial and installed it successfully in dual boot with another USB drive. I still have windows but I hate it when for some reason I've to boot into bcz it's so freaking slow.
## Linux Experience
Fedora 42 workstation comes with wayland and its comparatively modern, faster and secure than the traditional X11 which comes with Mint. 

After installing Fedora, I explored the default GNOME, tried a few extensions, tweaked some keyboard shortcuts and installed few packages. I was exploring the default fedora but then I came across my friend's [[Dotfiles]], he recently installed Arch + [[Hyprland]] with Omarchy script which deletes everything on your system and installs Arch linux. 

Now you might think what are these things Arch, Hyprland and all so here is a basic overview of how our machine runs applications: 
- Basically an app doesn't directly talk to hardware, they talk to kernel (Linux).
- Then the apps display the content via monitors and here the mediator is Display server which can be X11/Wayland. 
- And hyprland, i3 are compositer/windows managers they arrange windows on your screen. 
- But GNOME is a complete Desktop environment like one which Windows provide. 

So I had GNOME as default on my machine, but I was curious about [[Hyprland]]. And to my surprise fedora uses wayland and it supports [[Hyprland]], so I decided to give it a try. 
After installing it for the first time and loggin into it, I was like...what is this. The wallpaper was ugly, there was some warning at the top and that's it. 

So after reading about it, I understood how it works and that you have to configure **everything** according to it. This process is called ricing. So now I started learning about it more and added few things you can read at [[My Hyprland Rice]]. I'm still at it but it already looks & feel better. 

For now that's all about my Linux Fedora 42!