## MacOS Catalina/Big Sur/Monterey for ASUS VivoBook FL8700JP

[![img](https://img.shields.io/github/stars/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh.svg?color=ff69b4&label=%E7%82%B9%E8%B5%9E&logoColor=ff69b4&style=social)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh) [![img](https://img.shields.io/github/followers/bilijp153.svg?label=粉丝&logoColor=success&style=social)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh) ![img](https://img.shields.io/github/contributors/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh.svg?color=red&label=%E8%B4%A1%E7%8C%AE%E4%BA%BA%E6%95%B0) [![img](https://img.shields.io/github/last-commit/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh.svg?color=orange&label=%E6%9C%80%E8%BF%91%E6%8F%90%E4%BA%A4)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh)

## English Version: [ASUS-VivoBook-FL8700JP-Hackintosh](README_en.md) 

## 下载地址

[![Download from https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/releases](https://img.shields.io/github/v/release/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh?label=下载)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/releases)

# BIOS设置：

- 关闭`SecureBoot`

- 关闭`FastBoot`

- 硬盘模式修改为`AHCI`

- DVMT修改为`64M`


## 一、配置：

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
|   Mac模拟机型     |        MacBookPro 16,2      |
|   支持安装版本（已做测试）     |        Mac OS Catalina 10.15.7（19H2) ~ Mac OS  Monterey 12.3.1    |




## 二、正常工作
1. Type-C、USB3.0，2.0接口和读卡器（HDMI暂不能使用）
2. 核显`Intel lris Plus Graphics G7`的硬件加速（独显`MX330`无法驱动已做屏蔽）
3. 声卡输出（alcid=5）
4. 耳机接口
5. 麦克风
6. WIFI/蓝牙
7. 电池
8. 触控板
9. 睡眠和唤醒



## 三、Bug
1.声音有概率`从 Windows 切换到 Mac OS`时 Mac OS 无声音 (` Windows`下的` Realtek`驱动若为` Windows`自带的HDA驱动则无此Bug）

2.~~睡眠~~（已修复）

3.~~电池~~ （已修复）

4.~~核显开机黑屏问题~~（已修复）



## 四、注意事项
1.下载的EFI请替换其中的三码后再使用，防止出现冲突。   

2.如存在安装最新系统存在停留在还剩15分钟可先安装 `Mac OS Catalina 10.15.7（19H2)`然后再使用系统更新升级到最新系统

3.使用 EFI for 19H2版本的升级到 12.x 需去引导文件 `config.plist`里的Kernel开启`BlueToolFixup.kext`并关闭`IntelBluetoothInjector.kext`以确保 12.x 的蓝牙能够正常使用

4.从10.15.7升级至12.x需先在10.15.7安装完在Mac所需使用App后再升级12.x

## 五、本机NVRAM在Mac下能正常使用，通过OC引导界面开机按`Ctrl+Enter`选择默认启动盘。
