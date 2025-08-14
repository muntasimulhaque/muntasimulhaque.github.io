---
layout: post
title: "Write Bangla on Debian/Devuan/Ubuntu/Mint Xfce"
date: 2025-08-14
---

You can write Bangla on Debian or Debian based distros, e.g. Devuan, Ubuntu, Mint, etc., Xfce edition using the IBus input method.

For this, you need to install some packages using the following command:

```
apt install ibus ibus-m17n m17n-db ibus-gtk
```

This would install the required packages for writing Bangla on any Debian or Debian-based system. 

Now you have to add the IBus daemon into the startup items so that IBus autostarts with the desktop.

On the Xfce desktop, open the **Session and Startup** application from the Applications Menu. Then go to the `Application Autostart` tab and click on the `Add` button from the lower left. 

Add the following info into the dialog prompt:

```
Name: IBus daemon
Description: Start the IBus daemon when Xfce starts
Command: /usr/bin/ibus-daemon -d
```

You can write anything into the **Name** and **Description** text boxes. But the **Command** has to be exactly as I put here and the rests don't matter.

Then click on **OK** button to save it and then close the Session and Startup application.

Now all you have got to do is reboot the system. 

After a reboot, you should see the IBus input method icon on the Xfce panel. Right-click on it and select **Preferences**. This would open the IBus Preferences.

Now I go to the **Input Method** tab and click on the **Add** button.

Click on the more button and scroll-down until you see Bengali. Click on it and select `unijoy (m17n)` from there. This would add the unijoy keyboard layout into IBus input method. 

I like unijoy for I’m used to the Bijoy keyboard layout and this unijoy keyboard in similar to Bijoy. 

You can choose other keyboard layout to your liking from the list.

Now go to the **General** tab of IBus Preferences and click on the 3-dot button of the Next input method. Uncheck **Super** key from Modifiers and check the **Control** key instead. And then click on the Apply button. Then click on the OK button and finally close the IBus Preferences.

This changes the keyboard toggle shortcut for switching Engish keyboard and Bangla unijoy keyboard with `Ctrl+Space`. That means whenever you press **Ctrl** and **Space** keys together, it toggles between English and Bangla keyboard. 

Alternatively, you can just select the desired input method from the IBus input method icon in the Xfce panel to chnage the keyboard layout. 

For me though, I just prefer the keyboard shortcut as I don’t have to lift my hand from the keyboard.

Hope it helps.