# MacOS Catalina/Big Sur/Monterey for ASUS VivoBook FL8700JP

[![](https://img.shields.io/badge/repositories-Aurora极光-informational?style=flat&logo=github&logoColor=white&color=9debeb)](https://github.com/bilijp153?tab=repositories)
[![img](https://img.shields.io/github/stars/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh.svg?color=ff69b4&label=tarts&logoColor=ff69b4&style=social)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh) [![img](https://img.shields.io/github/followers/bilijp153.svg?label=followers&logoColor=success&style=social)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh) ![img](https://img.shields.io/github/contributors/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh.svg?]) [![img](https://img.shields.io/github/last-commit/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh.svg?)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh)
[![](https://img.shields.io/badge/Telegram-Aurora极光-informational?style=flat&logo=telegram&logoColor=white&color=5fb659)](https://t.me/Aurora_5223)
[![](https://img.shields.io/badge/Twitter-極光-informational?style=flat&logo=twitter&logoColor=white&color=5fb659)](https://twitter.com/Aurora_jp123)



## 中文版本: [ASUS-VivoBook-FL8700JP-Hackintosh](README.md) 



## Model picture

![AsusFL8700JP](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/computer.png)
![AsusFL8700JP](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/computer2.png)
![AsusFL8700JP](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/computer1.png)


## Download

[![Download from https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/releases](https://img.shields.io/github/v/release/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh?label=Download)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/releases)

# BIOS settings:
- Close ` SecureBoot`
- Close ` FastBoot`
- Hard disk mode changed to ` AHCI`
- Modify DVMT to ` 64M`
## Configuration:
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
## Normal operation
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

## Bug
1. ~~There is a probability of `switching from Windows to Mac OS`, Mac OS has no sound (If the `Realtek` driver under `Windows` is the HDA driver that comes with `Windows`, there is no such bug)~~ (Fixed)

2. ~~sleep~~ (Fixed)

3. ~~battery~~ (Fixed)

4. ~~Black screen problem of nuclear display startup~~ (Fixed)

## Precautions
Please replace the three codes before using the downloaded EFI to prevent conflicts.

#### The native NVRAM can be used normally under the Mac. Press `Ctrl + enter` to select the default startup disk through the OC boot interface.


## Maintainer
#### Maintenance personnel ©[Aurora极光](https://github.com/bilijp153)，Released under the [License](./License) .<br>
#### Testers                [若涵](https://github.com/catlingyun)
Authored and maintained by [Aurora极光](https://github.com/bilijp153) with help from contributors ([Contributors]([https://github.com/Miracle-Sakuno/Asus-VivoBook-X509FB-Hackintosh/graphs/contributors](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/graphs/contributors))).

   > GitHub [@Aurora极光](https://github.com/bilijp153) · Twitter [@極光](https://twitter.com/Aurora_jp123) · Telegram Channel [@Aurora 极光](https://t.me/Aurora_5223)
