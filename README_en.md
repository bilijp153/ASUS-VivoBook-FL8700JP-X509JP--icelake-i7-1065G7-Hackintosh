

[![](https://img.shields.io/badge/repositories-Aurora极光-informational?style=flat&logo=github&logoColor=white&color=9debeb)](https://github.com/bilijp153?tab=repositories)
[![img](https://img.shields.io/github/stars/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh.svg?color=ff69b4&label=tarts&logoColor=ff69b4&style=social)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh) [![img](https://img.shields.io/github/followers/bilijp153.svg?label=followers&logoColor=success&style=social)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh) ![img](https://img.shields.io/github/contributors/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh.svg?]) [![img](https://img.shields.io/github/last-commit/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh.svg?)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh)
[![](https://img.shields.io/badge/Telegram-Aurora极光-informational?style=flat&logo=telegram&logoColor=white&color=5fb659)](https://t.me/Aurora_5223)
[![](https://img.shields.io/badge/Twitter-極光-informational?style=flat&logo=twitter&logoColor=white&color=5fb659)](https://twitter.com/Aurora_jp123)



## Table of contents
- [Language Selection(语言选择/語言選擇)](#Languageselection)
- [Real machine pictures](#Realmachinepictures)
- [Download link](#Downloadlink)
- [Configure](#Configure)
- [System compatibility](#Systemcompatibility)
- [What works and what doesn't] (#Whatworksandwhatdoesn't)
- [Hardware Compatibility](#HardwareCompatibility)
- [Post-installation operations](#Post-installationoperations)
- [Bugs](#Bugs)
- [Main Personnel] (#Mainersonnel)


## Language selection   
- [Simplified Chinese Version](README_.md)
- [Traditional Chinese Version](README_Traditional Chinese.md)



## Real machine pictures

![AsusFL8700JP](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/computer4.png)
![AsusFL8700JP](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/computer.png)
![AsusFL8700JP](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/computer2.png)
![AsusFL8700JP](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/computer1.png)


## Download link

[![Download from https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/releases](https://img.shields.io/github/v/release/bilijp153/ASUS-VivoBook-FL8700JP- Hackintosh?label=download)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/releases)

## Configure

| Configuration | Model |
|---------------|----------------------------|
| Processor | i7-1065G7 |
| Graphics | Intel lris Plus Graphics G7 |
| Independent display | MX330 (blocked) |
| Memory | 8GB+4GB DDR4 |
| Hard Disk | Western Digital 512G SSD |
| Sound Card | Realtek ALC256 |
| Wireless LAN | Intel Wireless-AC 9461 |
| Touchpad | ELAN1200 |

## System compatibility

  - Catalina (10.15.7)
  - Big Sur (11.x)
  - Monterey (12.x)
  - Ventura (13.x)


## What works and what doesn't
- [x] Type-C
- [x] USB ports
- [x] Card Reader
- [x] Intel lris Plus Graphics G7
- [x] sound card `ALC256` (alcid=5)
- [x] headphone jack
- [x] microphones
- [x] WiFi
- [X] Bluetooth
- [x] batteries
- [x] trackpad (GPIO interrupt)
- [x] Sleep and Wake
- [x] Ginkgo's Startup Assistant on Windows (additional software download required on Windows)
- [ ] MX330
- [ ] HDMI (The 10th generation processor has been removed from HDMI support by Apple, so it cannot be used)


## Hardware Compatibility

### CPU
This machine is equipped with a 10mm [Intel Core Ice Lake i7-1065G7 Processor] (https://www.intel.cn/content/www/cn/zh/products/sku/196597/intel-core-i71065g7-processor -8m-cache-up-to-3-90-ghz/specifications.html)

### GPU
| **Model** | **Compatibility?** |
| ---------- | ----------------------------- |
| Nvidia | Incompatible |
| Intel Core Graphics | Compatible |

Note: The Intel Core Display ID of this machine is 0x8A5C8083

###BIOS

- `SecureBoot` and `FastBoot` need to be turned off
- The hard disk mode should be changed to `AHCI`
- DVMT should be modified to `64M`

Note: The native NVRAM can be used normally under Mac. Press `Ctrl+Enter` or `Mac Preferences - Startup Disk (System Settings - General - Startup Disk under Ventura) through the OC boot interface to select the default startup disk.

### sound card
This machine is equipped with a sound card `Realtek ALC256`, and has Intel's intelligent sound technology

### LAN and Bluetooth
The network card installed in this machine is [Intel Wireless-AC 9461](https://ark.intel.com/content/www/cn/zh/ark/products/125193/intel-wirelessac-9461.html)
Bluetooth is 5.0

Note: The local network card does not support air transfer


## Post-installation operations

### Change SMBIOS (three codes)
Use the OCAT or OpenCore Configurator (hereafter referred to as the tool) model menu to generate your unique `SMBIOS (three code)` information.
`SMBIOS (three-code)` must be unique, you cannot use the one that exists in this `repository (EFI)`.
Run the tool and select Generate SMBIOS.
Use the table below to select the appropriate model for your hardware.
| Brand | Model |
|---------------|----------------------------|
| Apple | Apple MacBook Pro 16,2 |
| Apple | Apple MacBook Air 9,1 |

Go to Apple Coverage via the tool's Verify Serial Number button and enter the verification code (the serial number is automatically entered).
An "Invalid Serial Number" or "Purchase Date Not Verified" message is required to work. If you get other prompts, you must generate a new SMBIOS (code three) and check again.



## Bugs
1.~~There is a probability of `switching from Windows to Mac OS` when there is no sound on Mac OS (if the `Realtek` driver under `Windows` is the HDA driver that comes with `Windows`, there is no such bug)~~ (Fixed )

2. ~~Sleep~~ (Fixed)

3.~~battery~~ (repaired)

4.~~Nuclear display intermittent boot black screen problem~~ (fixed)

5. ELAN1200 indirect disconnection (belonging to ELAN1200 common problem)





## Main Personnel
   #### Maintainer ©[Aurora](https://github.com/bilijp153), released under [license](./License).
   #### Tester [Ruohan](https://github.com/catlingyun)
   Contributed by [Aurora](https://github.com/ biijp153) written and maintained.
