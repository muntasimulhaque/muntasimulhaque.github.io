---
layout: post
title: '"Unable to install GRUB in /dev/sda" Error During Linux Mint Installation'
date: 2025-04-27
---

I was installing Linux Mint 22.1 Xfce on my Thinkpad X220 laptop which already had Windows 10 installed. At the last moment, the installer failed to install GRUB in /dev/sda and showed the `Unable to install GRUB in /dev/sda` error with the message `Executing 'grub-install /dev/sda' failed. This is a fatal error.`

![Unable to install GRUB in /dev/sda](/assets/images/2025-04-27-unable-to-install-grub/grub-error.png "Unable to install GRUB in /dev/sda")

After going through some posts on Linux Mints forum, I found the solution. The issue was with the UEFI and Legacy boot. 

My Thinkpad X220 is a pretty old laptop. Interestingly it has both UEFI and Legacy boot options. I faced the issue because my Windows 10 was using the Legacy boot option, while Linux Mint was trying to use the UEFI boot option. They both have to use the same option: either UEFI or Legacy. 

The solution was pretty simple. I just had to go to the BIOS by pressing F1 key while booting the laptop. I found 3 options: Both UEFI and Legacy, UEFI only and Legacy only. 

As my Windows 10 was using the Legacy option, to prevent Linux Mint from using the UEFI, I chose the Legacy only mode and saved this change by pressing the F10 key.

After a reboot, when I tried to install Linux Mint again, this time the installation completed successfully without showing any error.

This solved the issue for me.