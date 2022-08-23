# MacOS Catalina/Big Sur/Monterey for ASUS VivoBook FL8700JP

[![img](https://img.shields.io/github/stars/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh.svg?color=ff69b4&label=tarts&logoColor=ff69b4&style=social)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh) [![img](https://img.shields.io/github/followers/bilijp153.svg?label=followers&logoColor=success&style=social)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh) ![img](https://img.shields.io/github/contributors/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh.svg?]) [![img](https://img.shields.io/github/last-commit/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh.svg?)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh)

## 中文版本: [ASUS-VivoBook-FL8700JP-Hackintosh](README.md) 

## Download

[![Download from https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/releases](https://img.shields.io/github/v/release/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh?label=Download)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/releases)

# BIOS settings:
- Close ` SecureBoot`
- Close ` FastBoot`
- Hard disk mode changed to ` AHCI`
- Modify DVMT to ` 64M`
## 1、 Configuration:
|Configuration | model|
|--------------|-----------------------------|
|Processor | i7-1065g7|
|Core display | Intel lris plus graphics G7|
|Unique display | mx330 (shielded)|
|Memory | 8GB + 4GB DDR4|
|Hard disk | Western Digital 512g SSD|
|Sound card | Realtek ALC256|
|Wireless network card | Intel wireless-ac 9461|

|             |                           |
|--------------|-----------------------------|
|Mac analog model | MacBookAir 9,1|
|Supported installed version (tested) | Mac OS Catalina 10.15.6 ~ Mac OS Monterey 12.5.1 and Mac OS Ventura 13 Beta 5|
## 2、 Normal operation
1. Type-C、USB3. 0, 2.0 interface and card reader (The tenth generation HDMI has been removed from HDMI support by Apple, so it cannot be used)
2. Hardware acceleration of core display `Intel lris plus graphics G7` (the independent display `mx330` cannot drive and has been shielded)
3. Sound card output (alcid = 5)
4. Headphone connector
5. Microphone
6. WiFi / Bluetooth
7. Battery
8. Touch panel（GPIO interrupt）
9. Sleep and wake up
10. Ginkgo's startup assistant with win (that is, win can right-click the Mac startup assistant in the taskbar and choose to start from Mac)

## 3、 Bug
1. The probability of sound is that there is no sound in Mac OS when switching from windows to Mac OS (`Realtek`driver under `windows` does not have this bug if it is HDA driver built by `windows`)

2. ~~sleep~~ (repaired)

3. ~~battery~~ (repaired)

4. ~~Black screen problem of nuclear display startup~~ (repaired)

## 4、 Precautions
Please replace the three codes before using the downloaded EFI to prevent conflicts.

## 5、 The native NVRAM can be used normally under the Mac. Press `Ctrl + enter` to select the default startup disk through the OC boot interface.
