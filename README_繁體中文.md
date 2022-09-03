## MacOS Catalina/Big Sur/Monterey for ASUS VivoBook FL8700JP

[![](https://img.shields.io/badge/儲存庫-Aurora极光-informational?style=flat&logo=github&logoColor=white&color=9debeb)](https://github.com/bilijp153?tab=repositories)
[![img](https://img.shields.io/github/stars/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh.svg?color=ff69b4&label=點贊&logoColor=ff69b4&style=social)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh) [![img](https://img.shields.io/github/followers/bilijp153.svg?label=粉絲&logoColor=success&style=social)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh) ![img](https://img.shields.io/github/contributors/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh.svg?color=red&label=貢獻人數) [![img](https://img.shields.io/github/last-commit/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh.svg?color=orange&label=最近提交)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh)
[![](https://img.shields.io/badge/電報-Aurora极光-informational?style=flat&logo=telegram&logoColor=white&color=5fb659)](https://t.me/Aurora_5223)
[![](https://img.shields.io/badge/推特-極光-informational?style=flat&logo=twitter&logoColor=white&color=5fb659)](https://twitter.com/Aurora_jp123)


## [中文版本](README.md)
## [English Version](README_en.md) 



## 機型圖片

![AsusFL8700JP](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/computer4.png)
![AsusFL8700JP](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/computer.png)
![AsusFL8700JP](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/computer2.png)
![AsusFL8700JP](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/computer1.png)


## 下載地址

[![Download from https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/releases](https://img.shields.io/github/v/release/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh?label=下载)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/releases)

# BIOS設置：

- 關閉`SecureBoot`

- 關閉`FastBoot`

- 硬盤模式修改為`AHCI`

- DVMT修改為`64M`


## 配置：

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

|             |                           |
|--------------|-----------------------------|
|   Mac模擬機型     |        MacBookAir 9,1      |
|   支持安裝版本（已做測試）     |        Mac OS Catalina 10.15.6 ~ Mac OS Monterey 12.5.1 and Mac OS Ventura 13 Beta 5    |




## 什麼工作和不工作
- [x] Type-C
- [x] USB3.0和2.0
- [x] 讀卡器
- [x] Intel lris Plus Graphics G7
- [ ] MX330
- [x] 聲卡`ALC256`（alcid=5）
- [x] 耳機接口
- [x] 麥克風
- [x] WiFi
- [X] 藍牙
- [x] 電池
- [x] 觸控板（GPIO中斷）
- [x] 睡眠和喚醒
- [x] 白果的Windows上的啟動助理（Windows上需下載額外軟件）
- [ ] HDMI（十代處理器已被蘋果公司去除HDMI支持，故不能使用）


## Bug
1.~~聲音有概率`從 Windows 切換到 Mac OS`時 Mac OS 無聲音 (` Windows`下的` Realtek`驅動若為` Windows`自帶的HDA驅動則無此Bug）~~ （已修復）

2.~~睡眠~~（已修復）

3.~~電池~~ （已修復）

4.~~核顯間歇性開機黑屏問題~~（已修復）

5.ELAN1200間接性斷觸（屬於ELAN1200通病）



## 注意事項
下載的EFI請替換其中的三碼後再使用，防止出現衝突。

#### 安裝黑蘋果請確認`Windows`上的聲卡驅動為`官方默認`或現在流行的第三方的`Dolby驅動`

#### 本機NVRAM在Mac下能正常使用，通過OC引導界面按`Ctrl+Enter`選擇默認啟動盤。



## 主要人員
   #### 維護人員 ©[Aurora极光](https://github.com/bilijp153)，基於[許可](./License)發布。
   #### 測試人員  [若涵](https://github.com/catlingyun)
   在貢獻者的幫助下，由[Aurora极光](https://github.com/bilijp153)編寫和維護。([貢獻者](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/graphs/contributors)).
   > GitHub [@Aurora极光](https://github.com/bilijp153) · Twitter [@極光](https://twitter.com/Aurora_jp123) · Telegram Channel [@Aurora 极光](https://t.me/Aurora_5223)

   
