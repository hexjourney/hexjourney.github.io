---
layout: post
title: "The Beginning"
date: 2020-03-01 13:00:00 -0000
categories: Kali
---
## HYPER-V and KALI
I like to work with VM's when possible, and one of my favourites hypervisor to work with is Hyper-V. It's just handy.. preinstalled with windows, it works out of the box, simple enough for me. One of the downsides is that it doesn't work that smooth for Linux as it does for Windows.

Firt things first. Change the resolution.

```
sudo vim /etc/default/grub
```
Search and change the corresponding line to:
```
GRUB_CMDLINE_LINUX_DEFAULT=”quiet splash video=hyperv_fb:1920×1080″
```
Then in the terminal
```
sudo update-grub
```
And that's it.

Now, that's a fast solution. But if you'd like to go a little bit farther just follow the link from the Kali guys and install the Guest Tools. Doing that you will have clipboard sharing between host and VM as well as window resizing. (this last bit still doesn't work for me)

[Installing Hyper-V Enhanced Session Mode (Guest Tools)](https://www.kali.org/docs/virtualization/install-hyper-v-guest-enhanced-session-mode/)
