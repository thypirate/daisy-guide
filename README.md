# Installing custom Kernel on Xiaomi Mi A2 Lite (Daisy) Android 10 

## Prerequisites

* Android SDK tools: https://developer.android.com/studio/releases/platform-tools
* Offain's TWRP image: https://androidfilehost.com/?fid=1395089523397933315
* Offain's TWRP zip: https://androidfilehost.com/?fid=1395089523397933316
* Official Daisy firmware: https://c.mi.com/oc/miuidownload/detail?device=1700354


## Introduction

This is a simple how to install a custom kernel on ```Xiaomi Mi A2 Lite``` Android 10 device also known by the codename ```Daisy```.

Also installing a custom rom involves somewhat similar approach too as you can see in following [this repo](https://github.com/tkchn/daisyinstall).

This repo is based on [this](https://c.mi.com/thread-2975053-1-0.html) thread on Mi Community by user [OS herdz](https://c.mi.com/space-uid-1891219999.html).
 
 
## Installing

First things first, you need to enable developer options.

To enable developer options just go to Settings > About phone > tap on Build number 7 times and you are done, developer options is now enabled.

1 - Unlock Bootloader, go to Settings > System > Developer options > tap on OEM unlocking and also make sure to turn on USB debugging which you can easily find it by scrolling down a bit.

2 - Assuming that you've downloaded all the prerequisites files, copy the twrp.img inside adb folder.

3 - Put your device in fastboot mode by pressing volume down button + power button.

4 - Connect your device to your PC and open a terminal or cmd (if you are using windows) in your adb folder. Type the following command ```fastboot boot twrp.img```.

5 - In Twrp hit install button and search your kernel.

6 - After installing make sure to wipe dalvik before rebooting.

7 - After rebooting you can go Setting > About phone > Android version > and voila you can see that the new kernel has been successfully installed.
