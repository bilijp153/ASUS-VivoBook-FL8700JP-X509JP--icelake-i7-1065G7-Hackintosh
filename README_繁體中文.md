[![](https://img.shields.io/badge/儲存庫-Aurora极光-informational?style=flat&logo=github&logoColor=white&color=9debeb)](https://github.com/bilijp153?tab=repositories)
[![img](https://img.shields.io/github/stars/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh.svg?color=ff69b4&label=點贊&logoColor=ff69b4&style=social)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh) [![img](https://img.shields.io/github/followers/bilijp153.svg?label=粉絲&logoColor=success&style=social)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh) ![img](https://img.shields.io/github/contributors/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh.svg?color=red&label=貢獻人數) [![img](https://img.shields.io/github/last-commit/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh.svg?color=orange&label=最近提交)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh)
[![](https://img.shields.io/badge/電報-Aurora极光-informational?style=flat&logo=telegram&logoColor=white&color=5fb659)](https://t.me/Aurora_5223)
[![](https://img.shields.io/badge/推特-極光-informational?style=flat&logo=twitter&logoColor=white&color=5fb659)](https://twitter.com/Aurora_jp123)

## 目錄
- [語言選擇（语言选择/Language Selection）](#語言選擇)
- [實機圖片](#實機圖片)
- [下載地址](#下載地址)
- [配置](#配置)
- [系統兼容性](#系統兼容性)
- [更新日誌](更新日誌.md)
- [什麼工作和不工作](#什麼工作和不工作)
- [硬件兼容性](#硬件兼容性)
- [安裝前操作](#安裝前操作)
- [安裝後操作](#安裝後操作)
- [Bug](#Bug)
- [主要人員](#主要人員)
- [感謝](#感謝)


## 語言選擇   
- [簡體中文版本](README.md) 
- [English Version](README_en.md)


## 實機圖片

![AsusFL8700JP](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/computer4.png)
![AsusFL8700JP](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/computer.png)
![AsusFL8700JP](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/computer2.png)
![AsusFL8700JP](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/computer1.png)


## 下載地址

[![Download from https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/releases](https://img.shields.io/github/v/release/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh?label=下載)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/releases)

## 配置

|    配置       |        型號                 |
|--------------|-----------------------------|
|    處理器     |          i7-1065G7          |
|     核顯      |    Intel lris Plus Graphics G7    |
|     獨顯      |      MX330（已屏蔽）    |
|     內存      |     8GB+4GB DDR4        |
|     硬盤      |       西數 512G SSD        |
|     聲卡      |       Realtek ALC256        |
|   無線網卡     |        Intel Wireless-AC 9461      |
|   觸摸板     |        ELAN1200      |

## 系統兼容性

  - Catalina (10.15.7)
  - Big Sur (11.x)
  - Monterey (12.x)
  - Ventura (13.x)


## 什麼工作和不工作
- [x] Type-C
- [x] USB接口
- [x] 讀卡器
- [x] Intel lris Plus Graphics G7
- [x] 聲卡`ALC256`（alcid=5）
- [x] 耳機接口
- [x] 麥克風
- [x] WiFi
- [X] 藍牙
- [x] 電池
- [x] 觸控板（GPIO中斷）
- [x] 睡眠和喚醒
- [x] 白果的Windows上的啟動助理（Windows上需下載額外軟件）
- [ ] MX330
- [ ] HDMI（十代處理器已被蘋果公司去除HDMI支持，故不能使用）


## 硬件兼容性

### CPU
本機搭載的是10mm的[Intel Core Ice Lake i7-1065G7 處理器](https://www.intel.cn/content/www/cn/zh/products/sku/196597/intel-core-i71065g7-processor-8m-cache-up-to-3-90-ghz/specifications.html)

### GPU
| **型號**  | **兼容性**               |
| ---------- | ----------------------------- |
| Nvidia     | 不兼容        |
| Intel 核顯        | 兼容 |

注：本機的Intel 核顯 ID為 0x8A5C8083

### BIOS

- 需關閉`SecureBoot`和`FastBoot`
- 硬盤模式要修改為`AHCI`
- DVMT要修改為`64M`

注：本機NVRAM在Mac下能正常使用，通過OC引導界面按`Ctrl+Enter`或 `Mac 的偏好設置-啟動磁盤（Ventura下為系統設置-通用-啟動磁盤）`選擇默認啟動盤。

### 聲卡
本機搭載聲卡是`Realtek ALC256`，且擁有Intel的智音技術

### 網卡和藍牙
- 本機搭載的網卡是[Intel Wireless-AC 9461](https://ark.intel.com/content/www/cn/zh/ark/products/125193/intel-wirelessac-9461.html)
- 藍牙為5.0

注：本機網卡不支持隔空傳送


## 安裝前操作

### 更改BIOS設置
該項請看[BIOS](#BIOS)

### 硬盤（固態）設置
- 確認硬盤為GUID格式
- 確認硬盤EFI分區大於400M
- 確認沒有內置其他黑蘋果不支持的固態和機械盤

### 下載和安裝Mac
- [下載](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/releases)EFI
- 去黑[果小兵的部落閣](https://blog.daliansky.net/)下載黑蘋果鏡像(下載的版本請看[系統兼容性](#系統兼容性)）
- 下載balenaEtcher
- 使用至少16G大小的U盤拷錄下載的黑蘋果鏡像
- 把下載的EFI文件複製到硬盤的EFI分區
- 使用軟件（入EasyUEFI）建立剛複製到EFI分區的的EFI引導
- 使用硬盤工具進行分區
- 開機按Esc進入引導選擇菜單，選擇剛創建的EFI引導
- 隨後會進入OpenCore菜單，選擇 Install 那項
- 等待進度條跑滿進入安裝程序
- 進入磁盤工具，選擇剛才分區的那個盤符格式化為APFS後退出回到主界面
- 選擇安裝Mac，按照提示進行安裝
- 多次重啟後出現Mac設置界面
- 完成設置後即可享用Mac

注：設置EFI引導時需選擇BootX64.efi,如果BootX64.efi不行則選擇OC文件夾下的OpenCore.efi


## 安裝後操作

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

### 擁有白蘋果啟動
- 下載[corpnewt](https://github.com/corpnewt)的[brigadier](https://github.com/corpnewt/brigadier)
- 按照提示安裝py
- 完成後程序會自動下載`Windows上的Bootcamp程序`
- 按照提示把下載來的`dmg`打開，把裡面的文件複製到Windows系統盤
- 進入EFI的機型設置`使用OCAT或OpenCore Configurator`打開，修改機型項讓`Windows`認為你是Mac機型
- 重啟進Windows（怎麼進Windows看[BIOS](#BIOS)）
- 安裝Bootcamp程序
- 按照安裝程序提示重啟，然後回`Mac`
- 進入EFI的機型設置`使用OCAT或OpenCore Configurator`打開，修改機型項讓`Windows`不再認為你是Mac機型
- 完成！享受白蘋果方式的啟動吧



## Bug
1.~~聲音有概率`從 Windows 切換到 Mac OS`時 Mac OS 無聲音 (` Windows`下的` Realtek`驅動若為` Windows`自帶的HDA驅動則無此Bug）~~ （已修復）

2.~~睡眠~~（已修復）

3.~~電池~~ （已修復）

4.~~核顯間歇性開機黑屏問題~~（已修復）

5.ELAN1200間接性斷觸（屬於ELAN1200通病）





## 主要人員
   #### 維護人員 ©[Aurora极光](https://github.com/bilijp153)，基於[許可](./License)發布。
   #### 測試人員  [若涵](https://github.com/catlingyun)
   在[貢獻者](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/graphs/contributors)的幫助下，由[Aurora极光](https://github.com/bilijp153)編寫和維護。
   
   
   ## 感謝
   - [黑果小兵的部落閣](https://blog.daliansky.net/)--黑蘋果鏡像下載網站
   - [corpnewt](https://github.com/corpnewt)的[brigadier](https://github.com/corpnewt/brigadier)--白果啟動方式工具
   
