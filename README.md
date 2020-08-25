# DELL Inspiron 14 5400 2-in-1 laptop EFI

Opencore hackintosh of a Dell 14 5400 2-in-1 notebook

## Dell Specs:

* 10th Generation Intel® Core™ i3-1005G1 Processor
* Windows 10 Home 64bit English
* 4GB,1x4GB,DDR4,3200MHz
* 256GB M.2 PCIe NVMe Solid State Drive

This build is for Catalina 10.15.4 using Opencore 0.6.0.

## What's working

* Wifi and Bluetooth (replaced with Fenvi BCM94352Z, it worked out of the box as advertised on Taobao)


## What's not working

* Integrated RealTek webcam
* Fn keys to control display backlight
* Trackpad
* Backlight
* Audio - Built in and HDMI
* All USB ports including USB-C
* Power management including sleep
* Touchscreen
* SD Card Reader
* HDMI Port
* Fn keys to control volume and keyboard backlight
* Combo jack
* iMessage and FaceTime (plist in repo sanitized.  You'll need to find your own SN)

## BIOS Configuration
Turn off the Secure Boot. That should be all.

## UEFI Variables
In order to run macOS without having to use WhatEverGreen's framebuffer patching and CFG-related booter quirks, it is strongly recommended to modify a few UEFI variables. To do that, you can use the included ModifiedGrub.efi (credits *brainsucker*), which provides the setup_var command.



## Credits
* [acidanthera](https://github.com/acidanthera) for [OpenCore](https://github.com/acidanthera/OpenCorePkg)
* The Dortania crew for their [documentation](https://dortania.github.io/)