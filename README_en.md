<div align="center">
  <img src="https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/hackintosh2.png" width="180" alt="Hackintosh Logo">
  <h1>ASUS VivoBook FL8700JP Hackintosh</h1>
  <p>Run macOS on a Windows Laptop</p>
</div>

---

## 📌 Quick Navigation([简体中文](README.md))([繁體中文](README_繁體中文.md))
|[🌟 Project Highlights](#-project-highlights) |[🚩 Project Overview](#-project-overview) |[📸 Gallery](#-gallery)|[💻 Hardware Compatibility](#-hardware-compatibility) |
|------------------|------------------|----------------------------|----------------------------|
|[🖥️ System Support](#️-system-support)|[⚙️ Installation Guide](#️-installation-guide) |[🛠️ Advanced Config](#️-advanced-config) |[❓ FAQ](#-faq) |
|[⚠️ Notes](#️-notes)|[🌟 Contribution & Support](#️-contribution--support) |[📮 Feedback](#-feedback) |[🙏 Acknowledgments](#-acknowledgments) |
---

## 🌟 Project Highlights
- ✅ **Full Compatibility**: Supports macOS Catalina ~ Sequoia  
- 🖥 **Hardware Optimization**: Deep adaptation for iGPU/Audio/Wi-Fi  
- 🚀 **Performance Tuning**: Native CPU power management + Turbo Boost  
- 🔋 **Power Optimization**: Native power management + Sleep support  
- 🛠 **Continuous Maintenance**: Regular EFI updates and bug fixes  

---

## 🚩 Project Overview
### EFI Structure
```bash
EFI/                         # EFI Boot Directory
├── BOOT/                    # Boot Directory
│   └── BOOTx64.efi          # UEFI Boot File
└── OC/                      # OpenCore Directory
    ├── ACPI/                # DSDT/SSDT Patches
    ├── Kexts/               # Core Kexts
    ├── Drivers/             # OpenCore Drivers
    ├── config.plist         # Main Configuration
    └── ...                  # Other Resources
└── ...                      # Other System Directories


```
### Notes
- **Only compatible with ASUS FL8700JP (X509JP)**. Other devices are not guaranteed.  
- **No macOS installer included**. Prepare the installer yourself.  
- Backup data before installation. **Proceed at your own risk**.  
- Licensed under [MIT License](LICENSE). Commercial use prohibited.  

### [↩️ Back to Navigation](#-quick-navigation)

---

## 📸 Gallery
<div align="center">
  <img src="https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/computer1.png" width="45%">
  <img src="https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/computer2.png" width="45%">
</div>

---

## 💻 Hardware Compatibility
| Component      | Model                     | Status    | Notes                     |
|----------------|---------------------------|-----------|---------------------------|
| **CPU**        | Intel i7-1065G7           | ✅ Working | Ice Lake architecture    |
| **iGPU**       | Intel Iris Plus G7        | ⚠️ Partial | HDMI output unsupported  |
| **dGPU**       | NVIDIA MX330              | ❌ Unsupported | Disabled via SSDT      |
| **Audio**      | Realtek ALC256            | ✅ Working | Auto-switch for peripherals |
| **Wi-Fi**      | Intel Wireless-AC 9461    | ✅ Partial | No AirDrop/AirPlay       |
| **Trackpad**   | ELAN1200                  | ⚠️ Partial | Occasional unresponsiveness |
| **Type-C**     | -                         | ⚠️ Partial | No DP/Thunderbolt support |

---

## 🖥️ System Support
| macOS Version  | Compatibility | Minimum Version       |
|----------------|---------------|-----------------------|
| Catalina       | ✅             | 10.15.4              |
| Big Sur        | ✅             | 11.0                 |
| Monterey       | ✅             | 12.0                 |
| Ventura        | ✅             | 13.0                 |
| Sonoma         | ✅             | 14.0                 |
| Sequoia        | ✅             | 15.0                 |

### [↩️ Back to Navigation](#-quick-navigation)

---

## ⚙️ Installation Guide
### 1. BIOS Settings

- **Secure Boot**: Disabled  
- **Fast Boot**: Disabled  
- **DVMT Pre-Allocated**: 64M  

### 2. Installation Steps

1. Download macOS installer ➔ Recommended: [Daliansky's Blog](https://blog.daliansky.net/)  
2. Create macOS installer USB ➔ Use [BalenaEtcher](https://www.balena.io/etcher/)  
3. [**Download**](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/releases) EFI files ➔ Replace the USB's EFI folder  
4. Set USB as first boot device  
5. Boot via OpenCore ➔ Select "Install macOS XXX"  
6. Reboot multiple times until setup completes  
7. Migrate EFI to the internal SSD and remove USB  

### 3. SMBIOS Configuration

1. Use **OpenCore Configurator** or [**OCAuxiliaryTools**](https://github.com/ic005k/OCAuxiliaryTools) to set **SystemProductName** to **MacBookAir9,1** or **MacBookPro16,2** (recommended: MacBookAir9,1)  
2. Generate a valid **SystemSerialNumber** and verify via Apple's [Check Coverage Page](https://checkcoverage.apple.com/)  
3. Save and reboot  

---

## 🛠️ Advanced Config

💻 BootCamp Dual Boot Configuration

1. Download files via [**brigadier**](https://github.com/corpnewt/brigadier)  
2. Run the script and follow prompts to generate a **dmg**  
3. Copy BootCamp folders to the Windows partition  
4. Set **updateSMBIOSMod** to **Create** in `config.plist` and reboot  
5. Select **Windows** in OpenCore  
6. Install BootCamp drivers via `Setup.exe`  
7. Reboot and set **updateSMBIOSMod** back to **Custom**  

### [↩️ Back to Navigation](#-quick-navigation)

---

## ❓ FAQ
<details>
  <summary><b>Q: How to disable the startup "dong" sound?</b></summary>
  Go to System Settings ➔ Sound ➔ Disable "Play sound on startup".
</details>

<details>
  <summary><b>Q: Trackpad occasionally unresponsive?</b></summary>
  Reboot or sleep/wake to fix. Known issue with ELAN1200 drivers.
</details>

<details>
  <summary><b>Q: How to switch default OS?</b></summary>
  Press Ctrl+Enter in OpenCore or set via System Settings ➔ Startup Disk.
</details>

---

## ⚠️ Notes
1. **Skip Apple ID login** during setup and log in later via System Settings.  
2. Generate **unique SMBIOS** and ensure serial shows **"Invalid"** on Apple's site.  
3. Only then attempt Apple ID registration.  

---

## 🌟 Contribution & Support
| Role           | Contributor                |
|----------------|----------------------------|
| Maintainer     | [极光呆呆脑](https://github.com/bilijp153) |
| Tester         | [若涵](https://github.com/catlingyun) |

---

## 📮 Feedback
Submit via [GitHub Issues](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/issues) or contact:  
📧 **Email**: 1551656605@qq.com  

<a href="https://space.bilibili.com/329351708">
    <img src="https://img.shields.io/badge/Bilibili-极光呆呆脑-FF69B4?logo=bilibili" alt="Bilibili">
  </a>
  <a href="https://weibo.com/u/5264002671">
    <img src="https://img.shields.io/badge/Weibo-草莓小极光-1DA1F2?logo=sinaweibo" alt="Weibo">
  </a>
  <a href="https://qm.qq.com/cgi-bin/qm/qr?k=B2Omg5IKCGWoMNXgMIPmA_AJqEMnMCUb&noverify=0&personal_qrcode_source=3">
    <img src="https://img.shields.io/badge/QQ-极光呆呆脑-26A5E4?logo=QQ" alt="QQ">
  </a>

---

## 🙏 Acknowledgments
- [OpenCore Install Guide](https://dortania.github.io/OpenCore-Install-Guide/)  
- [Acidanthera](https://github.com/acidanthera) for kexts and tools  

### [↩️ Back to Navigation](#-quick-navigation)

---

<div align="center">
This project is licensed under [MIT License](LICENSE).  

© 2021-2024 极光呆呆脑. All rights reserved.
</div>
[file content end]
```
