---
layout: post
title: "Time Mismatch Between Devuan and Windows Dual Boot"
date: 2025-08-05
---

I have Devuan 5.0 Daedalus and Windows 10 dual boot. 

Devuan is basically Debian without systemd. Instead of systemd, it offers sysvinit, or openrc or runit. Anyway, the point is, I was facing time mismatch between Devuan and Windows. 

Time works differently in Windows and Linux. Windows expects BIOS time in Local Time. But Linux expects the BIOS time in UTC. I'm in Dhaka (Bangladesh), which is UTC+6. My BIOS time is set to Bangladeshi Local Time. So, Windows showed me the corrent time, but Devuan added 6 hours extra to it. 

It's not Devuan specific though. It's fundamental to how Linux works. And I faced the same issues with other distros like Ubuntu, Mint, etc. But as they use systemd, I could resolve this issue with a simple command: `timedatectl set-local-rtc true --adjust-system-time`.

But, I can't use `timedatectl` in Devuan Linux as it doesn't have systemd. Instead I can use hwclock or something else. 

I tried using `hwclock` and `date` commands. But neither worked for me. After trying everything, I finally solved it.

Here's what worked for me.

Open a terminal and run:

```
sudo nano /etc/adjtime
```

Usually there might be only three lines in that file and at the last line, if you see `UTC`, replace it with `LOCAL` and save the file.

Now, after this change, execute the following command:

```
sudo hwclock --hctosys --localtime
```

This would set the system clock as per the the hardware clock and ask the system to interpret the hardware clock as local time.

Now, check your system and hardware clock time with the following commands:

```
date
sudo hwclock --show
```

Now, link /etc/localtime with your correct time zone. For me, the command is:

```
sudo ln -sf /usr/share/zoneinfo/Asia/Dhaka /etc/localtime
```

Change the /Asia/Dhaka part with your time zone. To do this, after typing up to `sudo ln -sf /usr/share/zoneinfo/`, press the first letter of your continent name and press the Tab key. This would auto-fill your continent name. Then type in the first couple of letters of your time zone's city name, and you get the idea.

So, this solved the issue for me. I simply rebooted the system, and it worked. Hope it works for you, too.


