---
title: "Wii Themes"
---

{% include toc title="Tabel de Conținut" %}

This guide is intended to be the last you will ever need when it comes to theming on the Wii, not only providing instructions for the Wii Menu through MyMenuifyMod, but also with themes on WiiFlow Lite, USB Loader GX, and The Homebrew Channel. Additionally, forwarders are covered.

DO NOT CONTINUE WITH THIS GUIDE UNLESS YOU HAVE ADEQUATE BRICK PROTECTION, SPECIFICALLY [BOOTMII](bootmii) AND [PRIILOADER](priiloader)!
{: .notice--danger}

MyMenuifyMod has built in safety features to prevent from installing bad or corrupt Wii Menu themes, so please opt to use it instead of other theme installation homebrew.
{: .notice--warning}

Do not use any other version of ThemeMii than the one linked here, as ThemeMii Mod allows you to make a theme for Wii Menu version 4.3, other versions may not.
{: .notice--warning}

### Wii Menu Theming

Only install themes on your Wii that have been formatted specifically for its version and current region. Installing themes from the wrong version or region on your Wii will cause a [brick](bricks#theme-brick). This tutorial will tell you how to create a .csm file that is safe to install.
{: .notice--danger}

Before proceeding, it helps to know the difference between .MYM and .CSM as file formats when used in Wii Menu theming. While the MYM is made by the theme creator which can then be shared around, the CSM is the result from building a MYM into a system menu. In other words, MYM mainly just holds assets - the actual system menu itself that needs to be installed comes seperate.
{: .notice--info}

#### Theme Sources

+ [Wii Theme Team Creations](https://gbatemp.net/threads/wii-theme-team-creations.260327/) (.mym file distribution)
+ [Wii Theme Google Drive](https://drive.google.com/drive/folders/1H8bKkZa5Nwy7tBmDvKEVXhoZStucpUr3) (.mym file distribution)
+ [GBAtemp Other Files for Wii](https://gbatemp.net/download/categories/other-files.166/) (.mym file distribution)
+ [Wii Themer](http://www.wiithemer.org/) (online theme builder for specific versions and regions, ready to install .csm themes)

#### Instrumente necesare

* A modded Wii
* An SD card or USB device
* A Windows/macOS/Linux PC with an Internet connection
* [MyMenuifyMod](https://oscwii.org/library/app/mymenuifymod)
* [ThemeMii Mod](/assets/files/New_ThemeMii_MOD.zip)

#### Building a Theme

If you don't want to go through the hassle of using an external program to build a theme, you can also download a prebuilt theme from Wii Themer and skip to [Theme Installation](themes#theme-installation).

1. Once you download the theme you want and double-check that you have the right one for your system menu version and region, extract the .zip file for ThemeMii Mod and open the application.
1. Go to `Tools` > `Download Base App` > `Version of your Wii Menu` > `Region of your Wii Menu`.
1. A dialog box will pop-up asking you to enter in a value to create a key. Enter what it says, and it will create a key that will be used to decrypt the Wii Menu contents from Nintendo's servers.
1. A file selection box will ask you where to save the .app file (that is the Wii Menu content file that it downloaded). Save it to the directory where ThemeMii is in.
1. Go to `File` > `Open`, then browse for where your .mym file is.
1. Press `Create csm`, then browse for a directory you want to save the theme in. Give it a moment to build the theme.
1. A dialog box will pop up asking you if you want to save the .mym. Press `No`.

#### Theme Installation

1. Install MyMenuifyMod.
1. Create a new directory on your SD card or USB device called `modthemes` if it does not already exist.
1. Copy the theme file to the storage medium under the `modthemes` directory.
1. Put the storage medium in your Wii and boot it up.
1. Go into MyMenuifyMod, and acknowledge the disclaimer. It will ask what IOS you want to use in the app. Select `IOS58`.

    If you get `Exception DSI occured!`, press RESET on your Wii and try again.
    {: .notice--info}

1. Select your storage medium, and you should now see a selection of your themes.

    ![](/images/themes/mym-theme-selection.png)

1. Select the theme you would like to install. If it is signed, MyMenuifyMod will indicate it to you, otherwise it will warn you. Be absolutely sure at this point that you have downloaded the correct theme for your system menu version and region.
1. Install the theme.
1. Reboot into the Wii Menu, and see if the theme successfully installed. If all goes well, you will have a result similar to the below!

    ![](/images/themes/themed-wii-menu.png)

### WiiFlow Lite Theming

Unfortunately, because of the codebase difference between the original WiiFlow and the newer WiiFlow Lite, themes are sparse - in fact, only one theme could be found that confidently works on the newer version. The instructions for installing that theme are below.

#### Instrumente necesare

* A modded Wii
* An SD card or USB device
* [WiiFlow Lite](wii-loaders#wiiflow-lite)
* A Linux/macOS/Windows PC with an Internet connection
* [Rhapsodii Shima](https://gbatemp.net/threads/rhapsodii-shima-5-4.555062/)

#### Instrucțiuni

1. Have the storage device that holds WiiFlow Lite connected to your PC.
1. Download the Rhapsodii Shima archive, either version of the theme works and can be installed side-by-side with no issues.
1. Extract and copy the `wiiflow` folder to the root of your storage device, merge all folders and overwrite all files when requested.
1. Follow the theme setup and theme configuration instructions in `installation.txt`. Enjoy the theme!

### USB Loader GX Theming

#### Instrumente necesare

* A modded Wii
* An SD card or USB device
* [USB Loader GX](wii-loaders#usb-loader-gx)
* A Linux/macOS/Windows PC with an Internet connection
* A [theme](https://gbatemp.net/threads/dark-wii-usb-loader-gx-themes.584493/), this link contains an assortment of dark themes

#### Instrucțiuni

1. Download a theme `.zip` file from the website linked above, or anywhere else you can get a proper theme.
1. Unpack the `.zip` file's contents into the `apps\usbloader_gx` directory on the storage device where you installed USB Loader GX.
1. Put the storage medium in your Wii and boot it up.
1. Start USB Loader GX, go to the `Settings` menu, and then go to `Theme Menu`.
1. Open the theme and install it.

### Homebrew Channel Theming

#### Instrumente necesare

* A modded Wii
* An SD card or USB device
* A Linux/macOS/Windows PC with an internet connection
* A [theme](https://wiibrew.org/wiki/Homebrew_Channel/Themes) from WiiBrew

#### Instrucțiuni

1. Download a theme `.zip` file from the website linked above.

    ![](/images/themes/homebrew-channel-example-theme.png)

1. Paste the `.zip` into the `apps` folder on your storage device where you load homebrew.

    ![](/images/themes/homebrew-channel-paste-zip.png)

1. Extract the contents of the `.zip` into the `apps` folder, and delete the archive.

    ![](/images/themes/homebrew-channel-extract-theme.png)

1. Reinsert the storage device into your Wii and enter the Homebrew Channel.
1. The theme you just installed can be loaded in the same way that you access a standard app.

    ![](/images/themes/homebrew-channel-load-theme.png)

1. The theme should now be loaded, enjoy!

    ![](/images/themes/homebrew-channel-theme-done.png)

### App Forwarders

App forwarders can add a bit of extra flair to your Wii Menu - but be careful with them as bad forwarders can cause a [banner brick](bricks#banner-brick). Generally, you can find forwarders on places like [GBAtemp](https://gbatemp.net/threads/wii-forwarder-repository.588781/) for popular apps such as emulators. Since forwarders come in a .WAD format, the process of installing them is as simple as normal usage with [YAWM ModMii Edition](yawmme).


[Click aici pentru a reveni la indexul site-ului.](site-navigation)
{: .notice--info}
