# MacOS Catalina/Big Sur/Monterey for ASUS VivoBook FL8700JP

[![](https://img.shields.io/badge/repositories-Aurora极光-informational?style=flat&logo=github&logoColor=white&color=9debeb)](https://github.com/bilijp153?tab=repositories)
[![img](https://img.shields.io/github/stars/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh.svg?color=ff69b4&label=tarts&logoColor=ff69b4&style=social)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh) [![img](https://img.shields.io/github/followers/bilijp153.svg?label=followers&logoColor=success&style=social)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh) ![img](https://img.shields.io/github/contributors/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh.svg?]) [![img](https://img.shields.io/github/last-commit/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh.svg?)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh)
[![](https://img.shields.io/badge/Telegram-Aurora极光-informational?style=flat&logo=telegram&logoColor=white&color=5fb659)](https://t.me/Aurora_5223)
[![](https://img.shields.io/badge/Twitter-極光-informational?style=flat&logo=twitter&logoColor=white&color=5fb659)](https://twitter.com/Aurora_jp123)



## [中文版本](README.md) 
## [繁體中文版本](README_繁體中文.md) 



## Model picture

![AsusFL8700JP](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/computer4.png)
![AsusFL8700JP](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/computer.png)
![AsusFL8700JP](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/computer2.png)
![AsusFL8700JP](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/computer1.png)

## Download

[![Download from https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/releases](https://img.shields.io/github/v/release/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh?label=Download)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/releases)

# BIOS settings:
- Close ` SecureBoot`
- Close ` FastBoot`
- Hard disk mode changed to ` AHCI`
- Modify DVMT to ` 64M`
## Configuration:
|Configuration | Model|
|--------------|-----------------------------|
|Processor | i7-1065G7|
|Core display | Intel lris Plus Graphics G7|
|Unique display | MX330 (shielded)|
|Memory | 8GB + 4GB DDR4|
|Hard disk | Western Digital 512G SSD|
|Sound card | Realtek ALC256|
|Wireless network card | Intel wireless-ac 9461|
|   Touchpad     |        ELAN1200      |

|             |                           |
|--------------|-----------------------------|
|Mac analog model | MacBookAir 9,1|
|Supported installed version (tested) | Mac OS Catalina 10.15.6 ~ Mac OS Monterey 12.5.1 and Mac OS Ventura 13 Beta 5|
## What works and what doesn't
- [x] Type-C
- [x] USB3.0 and 2.0
- [x] Card Reader
- [x] Intel lris Plus Graphics G7
- [ ] MX330
- [x] sound card `ALC256` (alcid=5)
- [x] headphone jack
- [x] microphones
- [x] WiFi
- [X] Bluetooth
- [x] battery
- [x] trackpad (GPIO interrupt)
- [x] Sleep and Wake
- [x] Boot Assistant on Windows in the real MacBook (additional software download required on Windows)
- [ ] HDMI (10th generation CPU has been removed from HDMI support by Apple, so it cannot be used)

## Bug
1. ~~There is a probability of `switching from Windows to Mac OS`, Mac OS has no sound (If the `Realtek` driver under `Windows` is the HDA driver that comes with `Windows`, there is no such bug)~~ (Fixed)

2. ~~sleep~~ (Fixed)

3. ~~battery~~ (Fixed)

4. ~~Intermittent boot black screen problem~~ (Fixed)

5. ELAN1200 indirect disconnection (belonging to ELAN1200 common problem)

## Precautions
Please replace the three codes before using the downloaded EFI to prevent conflicts.

#### To install Black Apple, please confirm that the sound card driver on `Windows` is the `official default` or the now popular third-party `Dolby driver`

#### The native NVRAM can be used normally under the Mac. Press `Ctrl + enter` to select the default startup disk through the OC boot interface.


## Maintainer
#### Maintenance personnel ©[Aurora极光](https://github.com/bilijp153)，Released under the [License](./License) .<br>
#### Testers                [若涵](https://github.com/catlingyun)
Authored and maintained by [Aurora极光](https://github.com/bilijp153) with help from contributors ([Contributors]([https://github.com/Miracle-Sakuno/Asus-VivoBook-X509FB-Hackintosh/graphs/contributors](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/graphs/contributors))).

   > GitHub [@Aurora极光](https://github.com/bilijp153) · Twitter [@極光](https://twitter.com/Aurora_jp123) · Telegram Channel [@Aurora 极光](https://t.me/Aurora_5223)
