<div align="center">

<img align="center" width="100" height="180" src="https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/hackintosh1.png">
<h1>華碩VivoBook FL8700JP (X509JP) 筆記本的黑蘋果</h1>  

 <b> Hackintosh for Asuslaptop VivoBook FL8700JP (X509JP)
   

 
 
[![](https://img.shields.io/badge/存儲庫-Aurora極光-informational?logo=github&logoColor=black&color=9debeb&style=social)](https://github.com/bilijp153?tab=repositories)
[![](https://img.shields.io/badge/存儲庫-若涵-informational?logo=github&logoColor=black&color=9debeb&style=social)](https://github.com/catlingyun)
[![](https://img.shields.io/github/license/bilijp153/ASUS-VivoBook-FL8700JP-icelake-i7-1065G7-Hackintosh?label=許可&style=social)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-i7-1065G7-Hackintosh/blob/main/License)
[![img](https://img.shields.io/github/stars/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh.svg?color=ff69b4&label=點贊&logoColor=ff69b4&style=social)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-i7-1065G7-Hackintosh/stargazers)
[![img](https://img.shields.io/github/followers/bilijp153.svg?label=粉絲&logoColor=success&style=social)](https://github.com/bilijp153?tab=followers)
[![img](https://img.shields.io/github/contributors/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh.svg?logoColor=red&label=貢獻人數&style=social&logo=github)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-i7-1065G7-Hackintosh/graphs/contributors)
[![img](https://img.shields.io/github/last-commit/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh.svg?logoColor=orange&label=最近提交&style=social&logo=github)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-i7-1065G7-Hackintosh/graphs/commit-activity)
[![](https://img.shields.io/badge/嗶哩嗶哩-金俊綿小豆包-informational?logo=bilibili&logoColor=pink&color=5fb659&style=social)](https://space.bilibili.com/329351708?spm_id_from=333.337.0.0)
[![](https://img.shields.io/badge/微博-Aurora極光5431-informational?logo=sinaweibo&color=5fb659&style=social)](https://weibo.com/u/5264002671)
[![](https://img.shields.io/badge/QQ-Aurora極光-informational?logo=tencentqq&color=5fb659&style=social&logoColor=black)](https://qm.qq.com/cgi-bin/qm/qr?k=B2Omg5IKCGWoMNXgMIPmA_AJqEMnMCUb&noverify=0&personal_qrcode_source=3)
[![](https://img.shields.io/badge/Telegram-Aurora極光-informational?logo=telegram&logoColor=blue&color=5fb659&style=social)](https://t.me/Aurora_5223)
[![](https://img.shields.io/badge/Twitter-極光-informational?logo=twitter&logoColor=blue&color=5fb659&style=social)](https://twitter.com/Aurora_jp123)
 
 
   ![AsusFL8700JP](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/繁体1.png)


 </div>

 
 # 📄 目錄
- [語言選擇（語言選擇/Language Selection）](#-語言選擇)
- [注意事項](#-注意事項)
- [配置文件](#-配置文件)
- [實機圖片](#實機圖片)
- [下載地址](#-下載地址)
- [配置](#-配置)
- [系統兼容性](#-系統兼容性)
- [更新日誌](更新日誌.md)
- [什麼工作和不工作](#-什麼工作和不工作)
- [硬件兼容性](#ℹ-硬件兼容性)
- [安裝指南](#-安裝指南)
- [常見問題](#常見問題)
- [主要人員](#-主要人員)
- [感謝](#-感謝)
- [聯繫方式](#-聯繫方式)
- [版權聲明](#-版權聲明)


## 🔎 語言選擇   
- [简体中文版本](README.md) 
- [English Version](README_en.md)

 
## 🤔 注意事項
- 該 EFI 文件僅適用於 ASUS FL8700JP（X509JP） 筆記本，不保證在其他設備上的兼容性。
- 使用本項目時請仔細閱讀使用方法。
- 本項目僅提供黑蘋果 EFI 文件，不包含 macOS 操作系統鏡像文件。
- 在安裝過程中，請確保所有數據已備份，以免意外丟失。
- 本項目僅供學習和研究使用，請勿用於商業用途或其他非法用途 
- 使用本項目可能會對電腦造成一定風險，如果您遇到任何問題，請參考 Hackintosh 社區的相關討論或尋求專業人士的幫助，或在 [Issues](https://github.com/username/repo/issues) 中提出問題我們將盡快與您聯繫解決。

 
## 📦 配置文件

該項目提供的 EFI 配置文件包含以下內容：

``` 
EFI
├── BOOT
│   └── BOOTx64.efi
└── OC
    ├── ACPI
    ├── Kexts
    ├── Drivers
    ├── Resources
    ├── Tools
    ├── config.plist
    └── Opencore.efi
```
 
其中，Boot 裡的 Bootx64.efi 是筆記本 EFI 引導文件；OC 裡的 ACPI 包含了 DSDT、SSDT、UEFI 變量和補丁等文件，Kexts 包含了驅動程序，Drivers 包含了 OpenCore 引導程序，Tools 包含了 OpenCore 的相關工具，Resources 包含了 Opencore 的引導界面主題（圖形界面），config.plist 是 OpenCore 配置文件，Opencore.efi 是 Opencore 引導文件。


## 實機圖片

### 機型圖片
![AsusFL8700JP](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/computer4.png)
![AsusFL8700JP](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/computer.png)
![AsusFL8700JP](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/computer2.png)
![AsusFL8700JP](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/computer1.png)
### 引导界面图片
![AsusFL8700JP](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/EFI.png)
#### 引导界面图标
![AsusFL8700JP](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/icns.png)
## ⬇ 下載地址

[![Download from https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/releases](https://img.shields.io/github/v/release/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh?label=下載)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/releases)


## ⚙ 配置

|    配置       |        型號                 |
 |--------------|-----------------------------|
|    處理器     |          i7-1065G7          |
|     核顯      |    Intel lris Plus Graphics    |
|     獨顯      |      MX330（已屏蔽）    |
|     內存      |     8GB+4GB DDR4        |
|     硬盤      |       西數 512G SSD        |
|     聲卡      |       Realtek ALC256        |
|   無線網卡     |        Intel Wireless-AC 9461      |
|   觸摸板     |        ELAN1200      |
|  OpenCore版本     |          [![](https://img.shields.io/github/v/release/acidanthera/OpenCorePkg?include_prereleases&style=social&label=&logo=apple)](https://github.com/acidanthera/OpenCorePkg/releases)     |


## ✅ 系統兼容性

  - [ ] Mojave和之前的版本 
  - [x] Catalina 
  - [x] Big Sur 
  - [x] Monterey 
  - [x] Ventura 

注:Catalina從10.15.4版本起支持

## ❓ 什麼工作和不工作
- [x] Type-C
- [x] USB接口
- [x] 讀卡器
- [x] Intel lris Plus Graphics
- [x] 聲卡
- [x] 耳機接口
- [x] 麥克風
- [x] WiFi
- [X] 藍牙
- [x] 電池
- [x] 觸控板
- [x] 睡眠和喚醒
- [x] BootCamp
- [ ] MX330
- [ ] HDMI


## ℹ 硬件兼容性

### CPU 
本機搭載的是10mm的[Intel Core Ice Lake i7-1065G7 處理器](https://www.intel.cn/content/www/cn/zh/products/sku/196597/intel-core-i71065g7-processor-8m-cache-up-to-3-90-ghz/specifications.html)



### GPU 
| **型號**  | **兼容性**               |    **HDMI**               |     **DP**     |
| ---------- | -----------------------|---------------------------|----------------|
| Nvidia MX330     | 不兼容        |    -   |        -    |
| Intel lris Plus Graphics G7        | 兼容 |    不支持   |    支持      |

注:本機的Intel 核顯 ID為 0x8A5C0001

   該核顯支持DP但是本機沒有DP接口

   Ice Lake處理器已被蘋果公司去除HDMI支持，故不能使用
   
   ### BIOS

- 需關閉`SecureBoot`和`FastBoot`
- 硬盤模式要修改為`AHCI`
- DVMT要修改為`64M`

注:本機NVRAM在Mac下能正常使用，通過OC引導界面按`Ctrl+Enter`或 `Mac 的偏好設置-啟動磁盤（Ventura下為系統設置-通用-啟動磁盤）`選擇默認啟動盤。

### 🔊 聲卡和麥克風
本機搭載聲卡是`Realtek ALC256`，帶有Intel的智音技術

 ##### 聲卡和麥克風功能
- [x] 播放聲音
- [x] Mac啟動聲音
- [x] 有線耳機
- [x] 麥克風的使用
- [x] 插入耳機時設備的自動切換
- [x] USB音箱
- [x] Windows切換到Mac有聲
- [ ] HDMI聲音

注：要關閉Mac啟動聲音需去系統設置>聲音>啓動時播放聲音
   
   Windows切換到Mac有聲需Windows的聲卡驅動為第三方的驅動或Windows原版驅動

  
   
### ᯤ WiFi和藍牙
- 本機搭載的網卡是[Intel Wireless-AC 9461](https://ark.intel.com/content/www/cn/zh/ark/products/125193/intel-wirelessac-9461.html)
- 藍牙為5.0

##### WiFi和藍牙功能
- [x] WiFi連接（2.4G/5G）
- [x] iPhone和安卓的熱點連接
- [x] Apple Watch解鎖
- [x] 通用控制
- [x] 藍牙連接
- [x] 藍牙文件傳輸
- [ ] 隔空投送


### 🔌 Type-C和USB

##### Type-C和USB功能

- [x] Type-C網口
- [x] 擴展USB和SD卡接口
- [x] USB儲存設備（手機，USB等）
- [x] USB網卡和USB音箱
- [x] USB攝像頭 
- [ ] DP
- [ ] DP to HDMI
- [ ] 顯卡塢
- [ ] 充電

注:本機的Type-C是接在USB接口上而不是PCI接口上，固不支持一些功能


### ⌨️ 觸摸板和鍵盤
本機觸摸板為`ELAN1200`
本機內置鍵盤為`PS2鍵盤`

##### 觸摸板和鍵盤功能
- [x] 多指操作
- [x] 自由滑動
- [x] 流暢滾動
- [x] Mac手勢
- [x] 英文區和數字鍵區的使用
- [x] FN功能的使用
- [x] 鍵盤大寫鍵的開啟燈
- [x] Mac快捷鍵
- [ ] 鍵盤背光（鍵盤不支持）  

注:本機觸摸板存在死機現象，需重啟或睡眠再喚醒解決

FN部分功能鍵為Windows上的軟件專用，固在Mac上無反應


## 🛠 安裝指南

### 更改BIOS設置
該項請看[BIOS](#BIOS)

### 硬盤（固態）設置
- 確認硬盤為GUID格式
- 確認硬盤EFI分區大於400M
- 確認沒有內置其他黑蘋果不支持的固態和機械盤

### 下載和安裝Mac
1. [下載](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/releases)本倉庫中的 EFI 文件。
2. 使用 USB 啟動盤創建工具（推薦balenaEtcher）製作 U 盤啟動盤。
3. 將 EFI 文件夾複製到 U 盤的 EFI 分區中。
4. 進入 BIOS 設置，在 Boot Options 中選擇 U 盤啟動。
5. 進入 OpenCore 引導界面，選擇u盤中的“Install macOS”（安裝 macOS）。
6. 根據安裝嚮導完成安裝。
7. 安裝完成後，將 U 盤中的 EFI 文件夾複製到電腦硬盤的 EFI 分區中。
8. 重新啟動電腦，即可進入 macOS 操作系統。


### 更改SMBIOS（三碼）
- 使用OCAT或OpenCore Configurator（下稱該工具）的機型菜單生成您唯一的`SMBIOS（三碼）`信息。
`SMBIOS（三碼）` 必須是唯一的，您不能使用此`存儲庫(EFI)`中存在的一個。
- 運行該工具並選擇生成 SMBIOS。
- 使用下表為您的硬件選擇合適的型號。

|    品牌       |        型號                 |
|--------------|-----------------------------|
|    Apple     |          Apple MacBook Pro 16,2          |
|    Apple     |          Apple MacBook Air 9,1          |

- 通過該工具的驗證序列號按鈕轉到`蘋果序列號查詢網站`並輸入驗證碼（序列號已自動輸入）。
- 需要“無效序列號”或“未驗證購買日期”消息才算能用。如果你得到是其他提示，必須生成 新的`SMBIOS（三碼）`並再次檢查。

### 使用BootCamp
- 下載[corpnewt](https://github.com/corpnewt)的[brigadier](https://github.com/corpnewt/brigadier)
- 按照提示安裝py
- 完成後程序會自動下載`Windows上的Bootcamp程序`
- 按照提示把下載來的`dmg`打開，把裡面的文件複製到Windows系統盤
- 進入EFI的機型設置`使用OCAT或OpenCore Configurator`打開，修改機型`UpdateSMBIOSMod為Create和開啟SpoofVendor`讓`Windows`認為你是Mac機型
- 重啟進Windows（怎麼進Windows看[BIOS](#BIOS)）
- 安裝Bootcamp程序
- 按照安裝程序提示重啟，然後回`Mac`
- 進入EFI的機型設置`使用OCAT或OpenCore Configurator`打開，修改機型的修改機型`UpdateSMBIOSMod為Custom和關閉SpoofVendor`讓`Windows`不再認為你是Mac機型
- 完成！享受白蘋果方式的啟動吧



## 常見問題

Q: Type-C 插入DP顯示器為啥沒反應？

A: 因為本機的Type-C是接在USB接口上而不是PCI接口上，固不支持一些功能如DP。

Q: 開機有Duang的聲音怎麼辦？

A: 去系統設置>聲音關閉啟動時播放聲音

Q: Windows切換到Mac無聲音怎麼辦？

A:  Windows切換到Mac想要有聲音，需要Windows的聲卡驅動Windows原版驅動及驅動廠商是Microsoft而不是Realtek 

Q: 觸摸板用著用著沒反應了怎麼辦？

A: 本機的觸摸板是ELAN1200，會存在本死機現象，需重啟或睡眠再喚醒解決（是已知bug，暫無辦法修復）

Q: 怎麼設置默認啟動項？

A: 通過OC引導界面按`Ctrl+Enter`或 `Mac 的系統偏好設置-啟動磁盤（Ventura下為系統設置-通用-啟動磁盤）`選擇默認啟動盤。

Q:為什麼HDMI不能使用？

A: 因為本機處理器即Ice Lake處理器已被蘋果公司去除HDMI支持，故不能使用


## 👨 主要人員
   #### 維護人員 ©[Aurora极光](https://github.com/bilijp153)，基於[許可](./License)發布。
   #### 測試人員  [若涵](https://github.com/catlingyun)
   在[貢獻者](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/graphs/contributors)的幫助下，由[Aurora极光](https://github.com/bilijp153)編寫和維護。
   
   
## 🙏 感謝
   - [Acidanthera](https://github.com/acidanthera)--提供的 OpenCore 引導程序和相關 kext
   - [daliansky](https://github.com/daliansky)--提供的相關教程和 EFI ，并和他的的[Hackintosh](https://github.com/daliansky/Hackintosh)--加入我機型引導增加我EFI知名度
   - [corpnewt](https://github.com/corpnewt)的[brigadier](https://github.com/corpnewt/brigadier)--白果啟動方式工具

 
## 📧 聯繫方式

如有問題或建議，歡迎聯繫本項目的作者。

- 郵箱：1551656605@qq.com
- GitHub：https://github.com/bilijp153
- 還可以通過 GitHub 的 [Issues](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-X509JP--icelake-i7-1065G7-Hackintosh/issues)功能與我們聯繫。


## 📄 版權聲明
本項目遵循 MIT 開源協議。您可以自由地使用、修改和分發本項目，但請註明出處並保留原始版權聲明。詳情請參見 [許可證](License) 文件。
