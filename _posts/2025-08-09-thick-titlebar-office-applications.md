---
layout: post
title: "Microsoft Office 365 Thick Window Title Bar Issue"
date: 2025-08-09
---

My Microsoft Office 365 suit of applications, e.g. Word, Excel, PowerPoint, etc. show a thick title bar, which is outrageous to say the least. Take a look at the screenshot below.

![Thick Window Title Bar in Microsoft Office 365](/assets/images/2025-08-09-thick-titlebar-office-applications/microsoft-office-thick-title-bar.webp 'Thick Window Title Bar in Microsoft Office 365')

It's hideous. Looks aweful. 

I tried many things and at last found a solution in the [Microsoft Tech Community website](https://techcommunity.microsoft.com/discussions/microsoft-365/thick-window-title-bar-in-office-365-applications/2980542/replies/4158320){:target="_blank"}, posted by a user named **Rashid_Mehmood**. This worked for me. 

It's a registry hack. Just copy the code below in a text editor, maybe use the default windows notepad, and save it as `.reg` file format, e.g. office.reg

```
Windows Registry Editor Version 5.00

[HKEY_CURRENT_USER\SOFTWARE\Microsoft\Office\16.0\Common\ExperimentConfigs\ExternalFeatureOverrides\powerpoint]
"Microsoft.Office.UXPlatform.FluentSVRefresh"="false"
"Microsoft.Office.UXPlatform.FluentSVRibbonOptionsMenu"="false"
"Microsoft.Office.UXPlatform.RibbonTouchOptimization"="false"

[HKEY_CURRENT_USER\SOFTWARE\Microsoft\Office\16.0\Common\ExperimentConfigs\ExternalFeatureOverrides\excel]
"Microsoft.Office.UXPlatform.FluentSVRefresh"="false"
"Microsoft.Office.UXPlatform.FluentSVRibbonOptionsMenu"="false"
"Microsoft.Office.UXPlatform.RibbonTouchOptimization"="false"

[HKEY_CURRENT_USER\SOFTWARE\Microsoft\Office\16.0\Common\ExperimentConfigs\ExternalFeatureOverrides\word]
"Microsoft.Office.UXPlatform.FluentSVRefresh"="false"
"Microsoft.Office.UXPlatform.FluentSVRibbonOptionsMenu"="false"
"Microsoft.Office.UXPlatform.RibbonTouchOptimization"="false"
```  

After saving the file, double click on it. This would change the relevant registry and will give you back the sane regular titlebar.

Hope this works for you.