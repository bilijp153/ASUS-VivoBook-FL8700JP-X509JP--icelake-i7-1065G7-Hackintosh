## MacOS Catalina/Big Sur/Monterey for ASUS VivoBook FL8700JP

[![](https://img.shields.io/badge/存储库-Aurora极光-informational?style=flat&logo=github&logoColor=white&color=9debeb)](https://github.com/bilijp153?tab=repositories)
[![img](https://img.shields.io/github/stars/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh.svg?color=ff69b4&label=点赞&logoColor=ff69b4&style=social)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh) [![img](https://img.shields.io/github/followers/bilijp153.svg?label=粉丝&logoColor=success&style=social)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh) ![img](https://img.shields.io/github/contributors/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh.svg?color=red&label=%E8%B4%A1%E7%8C%AE%E4%BA%BA%E6%95%B0) [![img](https://img.shields.io/github/last-commit/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh.svg?color=orange&label=%E6%9C%80%E8%BF%91%E6%8F%90%E4%BA%A4)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh)
[![](https://img.shields.io/badge/电报-Aurora极光-informational?style=flat&logo=telegram&logoColor=white&color=5fb659)](https://t.me/Aurora_5223)
[![](https://img.shields.io/badge/推特-極光-informational?style=flat&logo=twitter&logoColor=white&color=5fb659)](https://twitter.com/Aurora_jp123)



## English Version: [ASUS-VivoBook-FL8700JP-Hackintosh](README_en.md) 



## 机型图片

![AsusFL8700JP](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/computer.png)
![AsusFL8700JP](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/computer2.png)
![AsusFL8700JP](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/computer1.png)


## 下载地址

[![Download from https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/releases](https://img.shields.io/github/v/release/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh?label=下载)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/releases)

# BIOS设置：

- 关闭`SecureBoot`

- 关闭`FastBoot`

- 硬盘模式修改为`AHCI`

- DVMT修改为`64M`


## 配置：

|    配置       |        型号                 |
|--------------|-----------------------------|
|    处理器     |          i7-1065G7          |
|     核显      |    Intel lris Plus Graphics G7    |
|     独显      |      MX330（已屏蔽）    |
|     内存      |     8GB+4GB DDR4        |
|     硬盘      |       西数 512G SSD        |
|     声卡      |       Realtek ALC256        |
|   无线网卡     |        Intel Wireless-AC 9461      |

|             |                           |
|--------------|-----------------------------|
|   Mac模拟机型     |        MacBookAir 9,1      |
|   支持安装版本（已做测试）     |        Mac OS Catalina 10.15.6 ~ Mac OS Monterey 12.5.1 and Mac OS Ventura 13 Beta 5    |




## 什么工作和不工作
- [x] Type-C
- [x] USB3.0和2.0接口
- [x] 读卡器
- [x] 核显`Intel lris Plus Graphics G7`的硬件加速（独显`MX330`无法驱动已做屏蔽）
- [x] 声卡输出（alcid=5）
- [x] 耳机接口
- [x] 麦克风
- [x] WIFI
- [X] 蓝牙
- [x] 电池
- [x] 触控板（GPIO中断）
- [x] 睡眠和唤醒
- [x] 白果的和win搭配的启动助理（即win可以任务栏Mac启动助理右键选择从Mac启动）
- [ ] HDMI（十代HDMI已被苹果公司去除HDMI支持，故不能使用）


## Bug
1.~~声音有概率`从 Windows 切换到 Mac OS`时 Mac OS 无声音 (` Windows`下的` Realtek`驱动若为` Windows`自带的HDA驱动则无此Bug）~~ （已修复）

2.~~睡眠~~（已修复）

3.~~电池~~ （已修复）

4.~~核显开机黑屏问题~~（已修复）



## 注意事项
下载的EFI请替换其中的三码后再使用，防止出现冲突。   

#### 本机NVRAM在Mac下能正常使用，通过OC引导界面按`Ctrl+Enter`选择默认启动盘。




## 主要人员
   #### 维护人员 ©[Aurora极光](https://github.com/bilijp153)，基于[许可](./许可)发布。
   #### 测试人员  [若涵](https://github.com/catlingyun)
   在贡献者的帮助下，由[Aurora极光](https://github.com/bilijp153)编写和维护。([贡献者](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/graphs/contributors)).
   > GitHub [@Aurora极光](https://github.com/bilijp153) · Twitter [@極光](https://twitter.com/Aurora_jp123) · Telegram Channel [@Aurora 极光](https://t.me/Aurora_5223)

   
