---
layout: post
title: "'br-connection-profile-unavailable' Error on Devuan 5.0 Daedalus"
date: 2025-08-05
---

While connecting my bluetooth earbuds to my Devuan 5.0 Daedalus Xfce edition, I got the following error:

> br-connection-profile-unavailable

After trying lots of things, executing the following commands one after another worked.

```
apt purge libspa-0.2-modules
apt autoremove
apt install pulseaudio-module-bluetooth libspa-0.2-bluetooth
```  
  
Hope it works for you, too.