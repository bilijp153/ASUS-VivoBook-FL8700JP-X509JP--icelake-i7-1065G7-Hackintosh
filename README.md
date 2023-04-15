<div align="center">

<img align="center" width="100" height="180" src="https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/hackintosh2.png">
<h1>华硕VivoBook FL8700JP (X509JP) 笔记本的黑苹果</h1>  

 <b> Hackintosh for Asuslaptop VivoBook FL8700JP (X509JP)
   

 
 
[![](https://img.shields.io/badge/存储库-Aurora极光-informational?logo=github&logoColor=black&color=9debeb&style=social)](https://github.com/bilijp153?tab=repositories)
[![](https://img.shields.io/badge/存储库-若涵-informational?logo=github&logoColor=black&color=9debeb&style=social)](https://github.com/catlingyun)
[![](https://img.shields.io/github/license/bilijp153/ASUS-VivoBook-FL8700JP-icelake-i7-1065G7-Hackintosh?label=许可&style=social)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-i7-1065G7-Hackintosh/blob/main/License)
[![img](https://img.shields.io/github/stars/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh.svg?color=ff69b4&label=点赞&logoColor=ff69b4&style=social)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-i7-1065G7-Hackintosh/stargazers)
[![img](https://img.shields.io/github/followers/bilijp153.svg?label=粉丝&logoColor=success&style=social)](https://github.com/bilijp153?tab=followers)
[![img](https://img.shields.io/github/contributors/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh.svg?logoColor=red&label=贡献人数&style=social&logo=github)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-i7-1065G7-Hackintosh/graphs/contributors)
[![img](https://img.shields.io/github/last-commit/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh.svg?logoColor=orange&label=最近提交&style=social&logo=github)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-i7-1065G7-Hackintosh/graphs/commit-activity)
[![](https://img.shields.io/badge/哔哩哔哩-金俊绵小豆包-informational?logo=bilibili&logoColor=pink&color=5fb659&style=social)](https://space.bilibili.com/329351708?spm_id_from=333.337.0.0)
[![](https://img.shields.io/badge/微博-Aurora極光5431-informational?logo=sinaweibo&color=5fb659&style=social)](https://weibo.com/u/5264002671)
[![](https://img.shields.io/badge/QQ-Aurora极光-informational?logo=tencentqq&color=5fb659&style=social&logoColor=black)](https://qm.qq.com/cgi-bin/qm/qr?k=B2Omg5IKCGWoMNXgMIPmA_AJqEMnMCUb&noverify=0&personal_qrcode_source=3)
[![](https://img.shields.io/badge/电报-Aurora极光-informational?logo=telegram&logoColor=blue&color=5fb659&style=social)](https://t.me/Aurora_5223)
[![](https://img.shields.io/badge/推特-極光-informational?logo=twitter&logoColor=blue&color=5fb659&style=social)](https://twitter.com/Aurora_jp123)
 
   ![AsusFL8700JP](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/简体1.png)

 </div>

 
 # 📄 目录
- [语言选择（語言選擇/Language Selection）](#-语言选择)
- [注意事项](#-注意事项)
- [配置文件](#-配置文件)
- [实机图片](#实机图片)
- [下载地址](#-下载地址)
- [配置](#-配置)
- [系统兼容性](#-系统兼容性)
- [更新日志](更新日志.md)
- [什么工作和不工作](#-什么工作和不工作)
- [硬件兼容性](#ℹ-硬件兼容性)
- [安装指南](#-安装指南)
- [常见问题](#常见问题)
- [主要人员](#-主要人员)
- [感谢](#-感谢)
- [联系方式](#-联系方式)
- [版权声明](#-版权声明)


## 🔎 语言选择   
- [繁體中文版本](README_繁體中文.md) 
- [English Version](README_en.md)

 

## 📢 注意事项
- 该 EFI 文件仅适用于 ASUS FL8700JP（X509JP） 笔记本，不保证在其他设备上的兼容性。
- 使用本项目时请仔细阅读使用方法。
- 本项目仅提供黑苹果 EFI 文件，不包含 macOS 操作系统镜像文件。
- 在安装过程中，请确保所有数据已备份，以免意外丢失。
- 本项目仅供学习和研究使用，请勿用于商业用途或其他非法用途 
- 在安装和使用该系统时，请遵守相关法律法规和知识产权保护规定。
- 使用本项目可能会对电脑造成一定风险，如果您遇到任何问题，请参考 Hackintosh 社区的相关讨论或寻求专业人士的帮助，或在 [Issues](https://github.com/username/repo/issues) 中提出问题我们将尽快与您联系解决。

 
## 📦 配置文件

该项目提供的 EFI 配置文件包含以下内容：

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
 
其中，Boot 里的 Bootx64.efi 是笔记本 EFI 引导文件；OC 里的 ACPI 包含了 DSDT、SSDT、UEFI 变量和补丁等文件，Kexts 包含了驱动程序，Drivers 包含了 OpenCore 引导程序，Tools 包含了 OpenCore 的相关工具，Resources 包含了 Opencore 的引导界面主题（图形界面），config.plist 是 OpenCore 配置文件，Opencore.efi 是 Opencore 引导文件。


## 实机图片

### 机型图片
![AsusFL8700JP](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/computer4.png)
![AsusFL8700JP](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/computer.png)
![AsusFL8700JP](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/computer2.png)
![AsusFL8700JP](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/computer1.png)
### 引导界面图片
![AsusFL8700JP](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/EFI.png)
#### 引导界面图标
![AsusFL8700JP](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/icns.png)
## ⬇ 下载地址

[![Download from https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/releases](https://img.shields.io/github/v/release/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh?label=下载)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/releases)

## ⚙ 配置

|    配置       |        型号                 |
|--------------|-----------------------------|
|    处理器     |          i7-1065G7          |
|     核显      |    Intel lris Plus Graphics    |
|     独显      |      MX330（已屏蔽）    |
|     内存      |     8GB+4GB DDR4        |
|     硬盘      |       西数 512G SSD        |
|     声卡      |       Realtek ALC256        |
|   无线网卡     |        Intel Wireless-AC 9461      |
|   触摸板     |        ELAN1200      |
|  OpenCore版本     |          [![](https://img.shields.io/github/v/release/acidanthera/OpenCorePkg?include_prereleases&style=social&label=&logo=apple)](https://github.com/acidanthera/OpenCorePkg/releases)     |

## ✅ 系统兼容性

  - [ ] Mojave和之前的版本 
  - [x] Catalina 
  - [x] Big Sur 
  - [x] Monterey 
  - [x] Ventura 

注:Catalina从10.15.4版本起支持

## ❓ 什么工作和不工作
- [x] Type-C
- [x] USB接口
- [x] 读卡器
- [x] Intel lris Plus Graphics
- [x] 声卡
- [x] 耳机接口
- [x] 麦克风
- [x] WiFi
- [X] 蓝牙
- [x] 电池
- [x] 触控板
- [x] 睡眠和唤醒
- [x] BootCamp
- [ ] MX330
- [ ] HDMI


## ℹ 硬件兼容性

### CPU 
本机搭载的是10mm的[Intel Core Ice Lake i7-1065G7 处理器](https://www.intel.cn/content/www/cn/zh/products/sku/196597/intel-core-i71065g7-processor-8m-cache-up-to-3-90-ghz/specifications.html)



### GPU 
| **型号**  | **兼容性**               |    **HDMI**               |     **DP**     |
| ---------- | -----------------------|---------------------------|----------------|
| Nvidia MX330     | 不兼容        |    -   |        -    |
| Intel lris Plus Graphics G7        | 兼容 |    不支持   |    支持      |

  
  ### BIOS

- 需关闭`SecureBoot`和`FastBoot`
- 硬盘模式要修改为`AHCI`
- DVMT要修改为`64M`


  ### 🔊 声卡和麦克风
   本机搭载声卡是`Realtek ALC256`，带有Intel的智音技术
  ##### 声卡和麦克风功能
    - [x] 播放声音
    - [x] Mac启动声音
    - [x] 有线耳机
    - [x] 麦克风的使用
    - [x] 插入耳机时设备的自动切换
    - [x] USB音箱
    - [x] Windows切换到Mac有声
    - [ ] HDMI声音

  
   
  ### ᯤ WiFi和蓝牙
   - 本机搭载的网卡是[Intel Wireless-AC 9461](https://ark.intel.com/content/www/cn/zh/ark/products/125193/intel-wirelessac-9461.html)
   - 蓝牙为5.0

  ##### WiFi和蓝牙功能
    - [x] WiFi连接（2.4G/5G）
    - [x] iPhone和安卓的热点连接
    - [x] Apple Watch解锁
    - [x] 通用控制
    - [x] 蓝牙连接
    - [x] 蓝牙文件传输
    - [ ] 隔空投送



 ### 🔌 Type-C和USB

  ##### Type-C和USB功能

    - [x] Type-C网口
    - [x] 扩展USB和SD卡接口
    - [x] USB储存设备（手机，USB等）
    - [x] USB网卡和USB音箱
    - [x] USB摄像头 
    - [ ] DP
    - [ ] DP to HDMI
    - [ ] 显卡坞
    - [ ] 充电



 ### ⌨️ 触摸板和键盘
  本机触摸板为`ELAN1200`
  本机内置键盘为`PS2键盘`

 ##### 触摸板和键盘功能
   - [x] 多指操作
   - [x] 自由滑动
   - [x] 流畅滚动
   - [x] Mac手势
   - [x] 英文区和数字键区的使用
   - [x] FN功能的使用
   - [x] 键盘大写键的开启灯
   - [x] Mac快捷键
   - [ ] 键盘背光 




## 🛠 安装指南

### 更改BIOS设置
该项请看[BIOS](#BIOS)

### 硬盘（固态）设置
- 确认硬盘为GUID格式
- 确认硬盘EFI分区大于400M
- 确认没有内置其他黑苹果不支持的固态和机械盘

### 下载和安装Mac
1. [下载](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/releases)本仓库中的 EFI 文件。
2. 使用 USB 启动盘创建工具（推荐[Etcher](https://www.balena.io/etcher/)）制作 U 盘启动盘。
3. 将 EFI 文件夹复制到 U 盘的 EFI 分区中。
4. 进入 BIOS 设置，在 Boot Options 中选择 U 盘启动。
5. 进入 OpenCore 引导界面，选择u盘中的“Install macOS”（安装 macOS）。
6. 根据安装向导完成安装。
7. 安装完成后，将 U 盘中的 EFI 文件夹复制到电脑硬盘的 EFI 分区中。
8. 重新启动电脑，即可进入 macOS 操作系统。


### 更改SMBIOS（三码）
- 使用OCAT或OpenCore Configurator（下称该工具）的机型菜单生成您唯一的`SMBIOS（三码）`信息。
`SMBIOS（三码）` 必须是唯一的，您不能使用此`存储库(EFI)`中存在的一个。
- 运行该工具并选择生成 SMBIOS。
- 使用下表为您的硬件选择合适的型号。

|    品牌       |        型号                 |
|--------------|-----------------------------|
|    Apple     |          Apple MacBook Pro 16,2          |
|    Apple     |          Apple MacBook Air 9,1          |

- 通过该工具的验证序列号按钮转到`苹果序列号查询网站`并输入验证码（序列号已自动输入）。
- 需要“无效序列号”或“未验证购买日期”消息才算能用。如果你得到是其他提示，必须生成 新的`SMBIOS（三码）`并再次检查。

### 使用BootCamp
- 下载[corpnewt](https://github.com/corpnewt)的[brigadier](https://github.com/corpnewt/brigadier)
- 按照提示安装py
- 完成后程序会自动下载`Windows上的Bootcamp程序`
- 按照提示把下载来的`dmg`打开，把里面的文件复制到Windows系统盘
- 进入EFI的机型设置`使用OCAT或OpenCore Configurator`打开，修改机型`UpdateSMBIOSMod为Create和开启SpoofVendor`让`Windows`认为你是Mac机型
- 重启进Windows（怎么进Windows看[BIOS](#BIOS)）
- 安装Bootcamp程序
- 按照安装程序提示重启，然后回`Mac`
- 进入EFI的机型设置`使用OCAT或OpenCore Configurator`打开，修改机型的修改机型`UpdateSMBIOSMod为Custom和关闭SpoofVendor`让`Windows`不再认为你是Mac机型
- 完成！享受白苹果方式的启动吧

## 常见问题

Q: Type-C 插入DP显示器为啥没反应？

A: 因为本机的Type-C是接在USB接口上而不是PCI接口上，固不支持一些功能如DP。

Q: 开机有Duang的声音怎么办？

A: 去系统设置>声音关闭启动时播放声音

Q: Windows切换到Mac无声音怎么办？

A:  Windows切换到Mac想要有声音，需要Windows的声卡驱动Windows原版驱动及驱动厂商是Microsoft而不是Realtek 

Q: 触摸板用着用着没反应了怎么办？

A: 本机的触摸板是ELAN1200，会存在本死机现象，需重启或睡眠再唤醒解决（是已知bug，暂无办法修复）

Q: 怎么设置默认启动项？

A: 通过OC引导界面按`Ctrl+Enter`或 `Mac 的系统偏好设置>启动磁盘（Ventura下为系统设置>通用>启动磁盘）`选择默认启动盘。

Q:为什么HDMI不能使用？

A: 因为本机处理器即Ice Lake处理器已被苹果公司去除HDMI支持，故不能使用
 
 
## 新功能完成进度
 
  Mac原生睡眠功能 ![Progress](https://progress-bar.dev/28/?cale=300title=Mac原生睡眠功能)

## 👨 主要人员
   #### 维护人员 ©[Aurora极光](https://github.com/bilijp153)，基于[许可](./License)发布。
   #### 测试人员  [若涵](https://github.com/catlingyun)

   
   
## 🙏 致谢
 

  - [dortania/OpenCore-Install-Guide](https://github.com/dortania/OpenCore-Install-Guide)
  - [Acidanthera](https://github.com/acidanthera)
  - [Hackintosh](https://github.com/daliansky/Hackintosh)
  - [brigadier](https://github.com/corpnewt/brigadier)


   
## 📧 联系方式

如有问题或建议，欢迎联系本项目的作者。

- 邮箱：1551656605@qq.com
- GitHub：https://github.com/bilijp153
- 还可以通过 GitHub 的 [Issues](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-X509JP--icelake-i7-1065G7-Hackintosh/issues)功能与我们联系。


## 📄 版权声明
本项目遵循 MIT 开源协议。您可以自由地使用、修改和分发本项目，但请注明出处并保留原始版权声明。详情请参见 [许可证](License) 文件。
 
© 2021-2023 Aurora极光.  All rights reserved.
   

