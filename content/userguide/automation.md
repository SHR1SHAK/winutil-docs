---
title: Automation
weight: 7
---

* Some features are available through automation. This allows you to save your config file, pass it to Winutil, walk away and come back to a finished system. Here is how you can set it up currently with Winutil >24.01.15

* On the Install Tab, click "Get Installed", this will get all installed apps **supported by Winutil** on the system.
![GetInstalled](/images/Get-Installed-Dark.png#only-dark#gh-dark-mode-only)
![GetInstalled](/images/Get-Installed-Light.png#only-light#gh-light-mode-only)

* Click on the Settings cog in the upper right corner and choose Export. Choose file file and location; this will export the setting file.
![SettingsExport](/images/Settings-Export-Dark.png#only-dark#gh-dark-mode-only)
![SettingsExport](/images/Settings-Export-Light.png#only-light#gh-light-mode-only)

* Copy this file to a USB or somewhere you can use it after Windows installation.

> [!TIP]
> Use the Microwin tab to create a custom Windows image & install the Windows image.

* On any supported Windows machine, open PowerShell **as Admin** and run the following command to automatically apply tweaks and install apps from the config file.
    ```ps1
    iex "& { $(irm https://christitus.com/win) } -Config [path-to-your-config] -Run"
    ```
* Have a cup of coffee! Come back when it's done.
