# Opencore-Vivobook-A409JA
Complete OpenCore Bootloader File for Asus Vivobook A409JA i3-1005G1

To do an installation of macOS Big Sur/Monterey on your laptop, you have to pick a separate file for macOS Big Sur/Monterey recovery image that can be obtained through OpenCore Dortania Guide on https://dortania.github.io/OpenCore-Install-Guide/installer-guide/winblows-install.html

But if you have installed one, and have somekind of buggy performance or having problems with graphics acceleration on Intel UHD G1 GPU, this is a file for you. But make sure that you change the Serial ID and System UUID. 

What things works with this file?
- Keyboard
- Trackpad
- Brightness and Volume key
- USB Camera
- Audio (Stereo and Mic available, but no Audio Jack audio)
- WiFi Networking and Bluetooth (Buggy Bluetooth Audio on a TWS Earphone, No AirDrop AirPlay Handoff etc)
- Siri is working perfectly well
- Sleep works perfectly well (NEW)
- On Catalina and above, DRM is broken, I have to wait for next WhateverGreen patch update.
- AppleTV+ is not working with broken DRM, so do Amazon Prime Video and Netflix I guess.
- Full graphics acceleration.
- Battery indicators correctly shown.
- Direct Booting, no bootpicker, suitable for users who wants a quicker boot (without dual-booting) without the need to have a checkpoint on boot picker. (Please press ALT in case you're dual-booting or change Misc > Boot > ShowPicker (True).

Notice!
For Intel Wireless users, please change your itlwm kext depending on what version of macOS you're about to install. 
Please edit some parts in PlatformInfo > Generic > Serials before using the EFI.


Format your USB to FAT32 for installation media USB (if you're using recovery image method).
It's good to always test it using a USB, DO NOT DIRECTLY PUT IT INTO YOUR EFI FOLDER IN CASE OF INCOMPATIBILITY.
