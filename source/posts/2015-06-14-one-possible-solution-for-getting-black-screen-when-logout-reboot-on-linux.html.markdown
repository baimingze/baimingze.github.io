---
layout: post
title: One possible solution for getting black screen when logout/reboot on Linux
date: 2015-06-14 11:09 BST
tags:
---

I have recently installed Fedora 22(KDE spin) on my laptop(ThinkPad T440, with the Inetel HD graphic card).

After I logged in the system, everything was fine with the plasma desktop.

But when I try to logout/reboot(either from KDE or konsole),  I got a black screen, no text, no cursor, just the fan's working noise, telling me that the computer was still working at some level. By the way, the Ctrl+Alt+F1/F2...got no response neither.

I have reset the runlevel to 3 and then try to use "startx", then I got a black screen on start! Even through I can logged in to KDE at runlevel 5 before.

After doing google, I got some ideas from the other's posts. And I found a way can help me to get rid of the black screen. 

The main idea is remove the "nomodeset" from boot. Here is my way indetail:

1. backup

```
cp /boot/grub2/grub.cfg /boot/grub2/grub.cfg.bak
cp /etc/default/grub /etc/default/grub.bak
```

2. remove "nomodeset" from these files with your editor

3. enjoy yourself



