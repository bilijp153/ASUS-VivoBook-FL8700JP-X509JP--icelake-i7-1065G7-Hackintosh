<div align="center">

<img align="center" width="100" height="180" src="https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/hackintosh2.png">
<h1>The Hackintosh of ASUS VivoBook FL8700JP (X509JP) notebook</h1>

  <b> Hackintosh for Asuslaptop VivoBook FL8700JP (X509JP)
   

[![](https://img.shields.io/badge/Repository-Aurora極光-informational?logo=github&logoColor=black&color=9debeb&style=social)](https://github.com/bilijp153?tab=repositories)
[![](https://img.shields.io/badge/Repository-若涵-informational?logo=github&logoColor=black&color=9debeb&style=social)](https://github.com/catlingyun)
[![](https://img.shields.io/github/license/bilijp153/ASUS-VivoBook-FL8700JP-icelake-i7-1065G7-Hackintosh?label=許可&style=social)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-i7-1065G7-Hackintosh/blob/main/License)
[![img](https://img.shields.io/github/stars/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh.svg?color=ff69b4&label=點贊&logoColor=ff69b4&style=social)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-i7-1065G7-Hackintosh/stargazers)
[![img](https://img.shields.io/github/followers/bilijp153.svg?label=粉絲&logoColor=success&style=social)](https://github.com/bilijp153?tab=followers)
[![img](https://img.shields.io/github/contributors/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh.svg?logoColor=red&label=Contributors&style=social&logo=github)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-i7-1065G7-Hackintosh/graphs/contributors)
[![img](https://img.shields.io/github/last-commit/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh.svg?logoColor=orange&label=Commit&style=social&logo=github)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-i7-1065G7-Hackintosh/graphs/commit-activity)
[![](https://img.shields.io/badge/Bilibili-金俊綿小豆包-informational?logo=bilibili&logoColor=pink&color=5fb659&style=social)](https://space.bilibili.com/329351708?spm_id_from=333.337.0.0)
[![](https://img.shields.io/badge/SinaWeibo-Aurora極光5431-informational?logo=sinaweibo&color=5fb659&style=social)](https://weibo.com/u/5264002671)
[![](https://img.shields.io/badge/QQ-Aurora極光-informational?logo=tencentqq&color=5fb659&style=social&logoColor=black)](https://qm.qq.com/cgi-bin/qm/qr?k=B2Omg5IKCGWoMNXgMIPmA_AJqEMnMCUb&noverify=0&personal_qrcode_source=3)
[![](https://img.shields.io/badge/Telegram-Aurora極光-informational?logo=telegram&logoColor=blue&color=5fb659&style=social)](https://t.me/Aurora_5223)
[![](https://img.shields.io/badge/Twitter-極光-informational?logo=twitter&logoColor=blue&color=5fb659&style=social)](https://twitter.com/Aurora_jp123)
 
    
![AsusFL8700JP](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/简体1.png)


  </div>

 
  # 📄 Directory
- [Language Selection(Language Selection/Language Selection)](#-Language-Selection)
- [Precautions](#-Precautions)
- [Configuration file](#-Configuration-file)
- [Machine picture](#Machine-picture)
- [Download link](#-Download-link)
- [Configuration](#-Configuration)
- [System Compatibility](#-System-Compatibility)
- [Changelog](Changelog.md)
- [What works and what doesn't](#-What-works-and-what-doesn't)
- [Hardware Compatibility](#ℹ-Hardware-Compatibility)
- [Installation Guide](#-Installation-Guide)
- [Bugs](#-Bugs)
- [Principal Personnel](#-Principal-Personnel)
- [Thanks](#-Thanks)
- [Contact](#-Contact)
- [Copyright Notice](#-Copyright-Notice)


## 🔎 Language selection
- [Traditional Chinese Version](README_繁體中文.md)
- [English Version](README_en.md)

 

## 🤔 Precautions
- This EFI file is only for ASUS FL8700JP (X509JP) notebook, compatibility on other devices is not guaranteed.
- Please read the usage instructions carefully when using this item.
- This project only provides black Apple EFI files, and does not include macOS operating system image files.
- During installation, please make sure all data is backed up to avoid accidental loss.
- This project is for learning and research purposes only, please do not use it for commercial purposes or other illegal purposes
- Using this project may cause certain risks to the computer. If you encounter any problems, please refer to the relevant discussions in the Hackintosh community or seek professional help or in [Issues](https://github.com/username/repo/issues), we will contact you as soon as possible to solve it.

 
## 📦 Configuration file

The EFI configuration file provided by this project contains the following:

```
EFI
├── BOOT
│ └── BOOTx64.efi
└── OC
     ├── ACPI
     ├── Kexts
     ├── Drivers
     ├── Resources
     ├── Tools
     ├── config.plist
     └── Opencore.efi
```
 
Among them, Bootx64.efi in Boot is the notebook EFI boot file; ACPI in OC includes files such as DSDT, SSDT, UEFI variables and patches, Kexts includes drivers, Drivers includes OpenCore bootloader, Tools includes OpenCore related Tools, Resources contains the Opencore boot interface theme (graphical interface), config.plist is the OpenCore configuration file, Opencore.efi is the Opencore boot file.


## Machine picture

### Model picture
![AsusFL8700JP](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/computer4.png)
![AsusFL8700JP](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/computer.png)
![AsusFL8700JP](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/computer2.png)
![AsusFL8700JP](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/computer1.png)
### 引导界面图片
![AsusFL8700JP](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/EFI.png)
#### 引导界面图标
![AsusFL8700JP](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/icns.png)
## ⬇ Download link

[![Download from https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/releases](https://img.shields.io/github/v/release/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh?label=Download)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/releases)

## ⚙ Configuration

| Configuration | Model |
|--------------|-----------------------------|
| Processor | i7-1065G7 |
| Core Graphics | Intel lris Plus Graphics |
| Independent display | MX330 (blocked) |
| Memory | 8GB+4GB DDR4 |
| Hard Disk | Western Digital 512G SSD |
| Sound Card | Realtek ALC256 |
| Wireless Network Card | Intel Wireless-AC 9461 |
| Touchpad | ELAN1200 |
| OpenCore version| [![](https://img.shields.io/github/v/release/acidanthera/OpenCorePkg?include_prereleases&style=social&label=&logo=apple)](https://github.com/acidanthera/OpenCorePkg/releases) |

## ✅ System Compatibility

   - [ ] Mojave and previous versions
   - [x] Catalina
   - [x] Big Sur
   - [x] Monterey
   - [x] Ventura

Note: Catalina supports from version 10.15.4

## ❓ What works and what doesn't
- [x]Type-C
- [x] USB interface
- [x] card reader
- [x] Intel lris Plus Graphics
- [x] sound card
- [x] Headphone jack
- [x] microphone
- [x] WiFi
- [X] Bluetooth
- [x] batteries
- [x] Trackpad
- [x] sleep and wake
- [x] Boot Camp
- [ ] MX330
- [ ] HDMI


## ℹ Hardware Compatibility

### CPU
This machine is equipped with a 10mm [Intel Core Ice Lake i7-1065G7 processor](https://www.intel.cn/content/www/cn/zh/products/sku/196597/intel-core-i71065g7-processor-8m-cache-up-to-3-90-ghz/specifications.html)



### GPU
| **Model** | **Compatibility** | **HDMI** | **DP** |
| ---------- | -----------------------|-------------- -------------|----------------|
| Nvidia MX330 | Not Compatible | - | - |
| Intel lris Plus Graphics G7 | Compatible | Not Supported | Supported |

Note: The Intel core display ID of this machine is 0x8A5C0001

    The core display supports DP but the machine does not have a DP interface

    Ice Lake processors have been removed by Apple for HDMI support, so they cannot be used
   
  
###BIOS

- Need to close `SecureBoot` and `FastBoot`
- The hard disk mode should be changed to `AHCI`
- DVMT should be changed to `64M`

Note: The NVRAM of this machine can be used normally under Mac. Press `Ctrl+Enter` or `Mac Preferences-Startup Disk (under Ventura, it is System Settings-General-Startup Disk)` to select the default startup disk through the OC boot interface.


### 🔊 Sound card and microphone
The sound card equipped with this machine is `Realtek ALC256`, with Intel's Zhiyin technology
##### Sound card and microphone function
- [x] play sound
- [x] Mac startup sound
- [x] Wired headphones
- [x] Microphone use
- [x] Automatic switching of devices when headphones are plugged in
- [x] USB speakers
- [x] Switch Windows to Mac with sound
- [ ] HDMI sound

Note: Mac startup sound needs to go to `config.plist` to enable
   
    Switching from Windows to Mac with sound requires Windows sound card driver to be a third-party driver or Windows original driver

  
   
### ᯤ WiFi and Bluetooth
- The network card equipped with this machine is [Intel Wireless-AC 9461](https://ark.intel.com/content/www/cn/zh/ark/products/125193/intel-wirelessac-9461.html)
- Bluetooth 5.0

##### WiFi and Bluetooth functionality
- [x] WiFi connection (2.4G/5G)
- [x] Hotspot connection for iPhone and Android
- [x] Apple Watch unlocked
- [x] General Controls
- [x] Bluetooth connection
- [x] Bluetooth file transfer
- [ ] AirDrop



### 🔌 Type-C and USB

##### Type-C and USB function

- [x] Type-C network port
- [x] Extended USB and SD card interface
- [x] USB storage device (mobile phone, USB, etc.)
- [x] USB network card and USB speakers
- [x] USB camera
- [ ] DP
- [ ] DP to HDMI
- [ ] Graphics dock
- [ ] Charge

Note: The Type-C of this machine is connected to the USB interface instead of the PCI interface, which does not support some functions


### ⌨️ Touchpad and Keyboard
The native touchpad is `ELAN1200`
The built-in keyboard of this machine is `PS2 keyboard`

##### Touchpad and Keyboard Functions
- [x] Multi-finger operation
- [x] Free Swipe
- [x] smooth scrolling
- [x] Mac Gestures
- [x] Use of English locale and numeric keypad
- [x] Use of FN function
- [x] Turn on light for keyboard caps key
- [x] Mac shortcut keys
- [ ] keyboard backlight (keyboard not supported)

Note: The touchpad of this machine has a crash phenomenon, which needs to be restarted or sleep and wake up to solve it

Some function keys of FN are dedicated to the software on Windows, and there is no response on Mac.



## 🛠 Installation Guide

### Change BIOS settings
For this item, please see [BIOS](#BIOS)

### Hard disk (solid state) settings
- Confirm that the hard disk is in GUID format
- Confirm that the hard disk EFI partition is larger than 400M
- Confirm that there are no built-in solid-state and mechanical disks that are not supported by other black apples

### Download and Install for Mac
1. [Download](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/releases) the EFI file in this repository.
2. Use a USB boot disk creation tool (balenaEtcher is recommended) to create a USB boot disk.
3. Copy the EFI folder to the EFI partition of the USB flash drive.
4. Enter the BIOS setup, select the USB flash drive to boot in Boot Options.
5. Enter the OpenCore boot interface, select "Install macOS" in the USB flash drive (install macOS).
6. Follow the installation wizard to complete the installation.
7. After the installation is complete, copy the EFI folder in the U disk to the EFI partition of the computer hard disk.
8. Restart the computer to enter the macOS operating system.


### Change SMBIOS (three codes)
- Use the model menu of OCAT or OpenCore Configurator (hereinafter referred to as the tool) to generate your unique `SMBIOS (three codes)` information.
The `SMBIOS (three codes)` must be unique, you cannot use the one present in this `repository (EFI)`.
- Run the tool and select Generate SMBIOS.
- Use the table below to select the appropriate model for your hardware.

| Brand | Model |
|--------------|-----------------------------|
| Apple | Apple MacBook Pro 16,2 |
| Apple | Apple MacBook Air 9,1 |

- Go to the `Apple Serial Number Lookup Website` via the tool's Verify Serial Number button and enter the verification code (the serial number has been entered automatically).
- Requires "Invalid serial number" or "Purchase date not verified" messages to work. If you get other prompts, you must generate a new `SMBIOS (three codes)` and check again.

### Using Boot Camp
- Download [brigadier](https://github.com/corpnewt/brigadier) from [corpnewt](https://github.com/corpnewt)
- Follow the prompts to install py
- After completion the program will automatically download the `Bootcamp program on Windows`
- Follow the prompts to open the downloaded `dmg`, and copy the files inside to the Windows system disk
- Enter the EFI model setting `Use OCAT or OpenCore Configurator` to open, modify the model `UpdateSMBIOSMod to Create and enable SpoofVendor` to let `Windows` think you are a Mac model
- Restart into Windows (see [BIOS](#BIOS) for how to enter Windows)
- Install the Bootcamp program
- Follow the installer prompts to restart, then go back to `Mac`
- Enter the EFI model setting `use OCAT or OpenCore Configurator` to open, modify the model `UpdateSMBIOSMod to Custom and close SpoofVendor` so that `Windows` no longer thinks you are a Mac model
- Finish! Enjoy the white apple way to boot



## ❗ Bugs
1.~~There is a possibility that Mac OS will have no sound when switching from Windows to Mac OS. )

2. ~~sleep~~ (fixed)

3.~~Battery~~ (Repaired)

4.~~Intermittent power-on black screen problem of nuclear display~~(Fixed)

5. ELAN1200 indirect disconnection (belongs to ELAN1200 common fault)


## 👨 Principal Personnel
   #### Maintainer ©[Aurora极光](https://github.com/bilijp153)，released based on[License](./License).
   #### Tester  [若涵](https://github.com/catlingyun)
   With the help of[貢獻者](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/graphs/contributors)，by[Aurora极光](https://github.com/bilijp153)written and maintained.
   
   
## 🙏 Thanks
    
  - [daliansky blog](https://blog.daliansky.net/)--A Hackintosh blog web
    
  - [corpnewt](https://github.com/corpnewt) [brigadier](https://github.com/corpnewt/brigadier)--Real Mac Boot Tool 
    
  - [daliansky](https://github.com/daliansky) [Hackintosh](https://github.com/daliansky/Hackintosh)--Join my model guide to increase my EFI popularity
  
## 📧 Contact

If you have any questions or suggestions, please feel free to contact the author of this project.

- Email: 1551656605@qq.com
- GitHub: https://github.com/bilijp153
- You can also contact us through GitHub's [Issues](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-X509JP--icelake-i7-1065G7-Hackintosh/issues) function.


## 📄 Copyright Notice
This project follows the MIT open source license. You are free to use, modify and distribute this project, but please acknowledge the source and retain the original copyright notice. See the [License](License) file for details.
