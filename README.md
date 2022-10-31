[![](https://img.shields.io/badge/存储库-Aurora极光-informational?style=flat&logo=github&logoColor=white&color=9debeb)](https://github.com/bilijp153?tab=repositories)
[![img](https://img.shields.io/github/stars/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh.svg?color=ff69b4&label=点赞&logoColor=ff69b4&style=social)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh) [![img](https://img.shields.io/github/followers/bilijp153.svg?label=粉丝&logoColor=success&style=social)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh) ![img](https://img.shields.io/github/contributors/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh.svg?color=red&label=%E8%B4%A1%E7%8C%AE%E4%BA%BA%E6%95%B0) [![img](https://img.shields.io/github/last-commit/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh.svg?color=orange&label=%E6%9C%80%E8%BF%91%E6%8F%90%E4%BA%A4)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh)
[![](https://img.shields.io/badge/电报-Aurora极光-informational?style=flat&logo=telegram&logoColor=white&color=5fb659)](https://t.me/Aurora_5223)
[![](https://img.shields.io/badge/推特-極光-informational?style=flat&logo=twitter&logoColor=white&color=5fb659)](https://twitter.com/Aurora_jp123)

## 目录
- [语言选择（語言選擇/Language Selection）](#语言选择)
- [实机图片](#实机图片)
- [下载地址](#下载地址)
- [配置](#配置)
- [系统兼容性](#系统兼容性)
- [更新日志](更新日志.md)
- [什么工作和不工作](#什么工作和不工作)
- [硬件兼容性](#硬件兼容性)
- [安装前操作](#安装前操作)
- [安装后操作](#安装后操作)
- [Bug](#Bug)
- [主要人员](#主要人员)
- [感谢](#感谢)


## 语言选择   
- [繁體中文版本](README_繁體中文.md) 
- [English Version](README_en.md)


## 实机图片

![AsusFL8700JP](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/computer4.png)
![AsusFL8700JP](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/computer.png)
![AsusFL8700JP](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/computer2.png)
![AsusFL8700JP](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/computer1.png)


## 下载地址

[![Download from https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/releases](https://img.shields.io/github/v/release/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh?label=下载)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/releases)

## 配置

|    配置       |        型号                 |
|--------------|-----------------------------|
|    处理器     |          i7-1065G7          |
|     核显      |    Intel lris Plus Graphics G7    |
|     独显      |      MX330（已屏蔽）    |
|     内存      |     8GB+4GB DDR4        |
|     硬盘      |       西数 512G SSD        |
|     声卡      |       Realtek ALC256        |
|   无线网卡     |        Intel Wireless-AC 9461      |
|   触摸板     |        ELAN1200      |

## 系统兼容性

  - Catalina (10.15.7)
  - Big Sur (11.x)
  - Monterey (12.x)
  - Ventura (13.x)


## 什么工作和不工作
- [x] Type-C
- [x] USB接口
- [x] 读卡器
- [x] Intel lris Plus Graphics G7
- [x] 声卡`ALC256`（alcid=5）
- [x] 耳机接口
- [x] 麦克风
- [x] WiFi
- [X] 蓝牙
- [x] 电池
- [x] 触控板（GPIO中断）
- [x] 睡眠和唤醒
- [x] BootCamp
- [ ] MX330
- [ ] HDMI


## 硬件兼容性

### CPU
本机搭载的是10mm的[Intel Core Ice Lake i7-1065G7 处理器](https://www.intel.cn/content/www/cn/zh/products/sku/196597/intel-core-i71065g7-processor-8m-cache-up-to-3-90-ghz/specifications.html)

### GPU
| **型号**  | **兼容性**               |    **HDMI**               |     **DP**     |
| ---------- | -----------------------|---------------------------|----------------|
| Nvidia     | 不兼容        |    -   |        -    |
| Intel 核显        | 兼容 |    不支持   |    支持      |

注：本机的Intel 核显 ID为 0x8A530002
    该核显支持DP但是本机没有DP接口
    Ice Lake处理器已被苹果公司去除HDMI支持，故不能使用

### BIOS

- 需关闭`SecureBoot`和`FastBoot`
- 硬盘模式要修改为`AHCI`
- DVMT要修改为`64M`

注：本机NVRAM在Mac下能正常使用，通过OC引导界面按`Ctrl+Enter`或 `Mac 的偏好设置-启动磁盘（Ventura下为系统设置-通用-启动磁盘）`选择默认启动盘。

### 声卡
本机搭载声卡是`Realtek ALC256`，且拥有Intel的智音技术

### 网卡和蓝牙
- 本机搭载的网卡是[Intel Wireless-AC 9461](https://ark.intel.com/content/www/cn/zh/ark/products/125193/intel-wirelessac-9461.html)
- 蓝牙为5.0

注：本机网卡不支持隔空传送


## 安装前操作

### 更改BIOS设置
该项请看[BIOS](#BIOS)

### 硬盘（固态）设置
- 确认硬盘为GUID格式
- 确认硬盘EFI分区大于400M
- 确认没有内置其他黑苹果不支持的固态和机械盘

### 下载和安装Mac
- [下载](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/releases)EFI
- 去[黑果小兵的部落阁](https://blog.daliansky.net/)下载黑苹果镜像(下载的版本请看[系统兼容性](#系统兼容性)）
- 下载balenaEtcher
- 使用至少16G大小的U盘拷录下载的黑苹果镜像
- 把下载的EFI文件复制到硬盘的EFI分区
- 使用软件（入EasyUEFI）建立刚复制到EFI分区的的EFI引导
- 使用硬盘工具进行分区
- 开机按Esc进入引导选择菜单，选择刚创建的EFI引导
- 随后会进入OpenCore菜单，选择 Install 那项
- 等待进度条跑满进入安装程序
- 进入磁盘工具，选择刚才分区的那个盘符格式化为APFS后退出回到主界面
- 选择安装Mac，按照提示进行安装
- 多次重启后出现Mac设置界面
- 完成设置后即可享用Mac

注：设置EFI引导时需选择BootX64.efi，如果BootX64.efi不行则选择OC文件夹下的OpenCore.efi



## 安装后操作

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

### 拥有白苹果启动
- 下载[corpnewt](https://github.com/corpnewt)的[brigadier](https://github.com/corpnewt/brigadier)
- 按照提示安装py
- 完成后程序会自动下载`Windows上的Bootcamp程序`
- 按照提示把下载来的`dmg`打开，把里面的文件复制到Windows系统盘
- 进入EFI的机型设置`使用OCAT或OpenCore Configurator`打开，修改机型项让`Windows`认为你是Mac机型
- 重启进Windows（怎么进Windows看[BIOS](#BIOS)）
- 安装Bootcamp程序
- 按照安装程序提示重启，然后回`Mac`
- 进入EFI的机型设置`使用OCAT或OpenCore Configurator`打开，修改机型项让`Windows`不再认为你是Mac机型
- 完成！享受白苹果方式的启动吧



## Bug
1.~~声音有概率`从 Windows 切换到 Mac OS`时 Mac OS 无声音 (` Windows`下的` Realtek`驱动若为` Windows`自带的HDA驱动则无此Bug）~~ （已修复）

2.~~睡眠~~（已修复）

3.~~电池~~ （已修复）

4.~~核显间歇性开机黑屏问题~~（已修复）

5.ELAN1200间接性断触（属于ELAN1200通病）


## 主要人员
   #### 维护人员 ©[Aurora极光](https://github.com/bilijp153)，基于[许可](./License)发布。
   #### 测试人员  [若涵](https://github.com/catlingyun)
   在[贡献者](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/graphs/contributors)的帮助下，由[Aurora极光](https://github.com/bilijp153)编写和维护。
   
   
   ## 感谢
   - [黑果小兵的部落阁](https://blog.daliansky.net/)--黑苹果镜像下载网站
   - [corpnewt](https://github.com/corpnewt)的[brigadier](https://github.com/corpnewt/brigadier)--白果启动方式工具
   - [daliansky](https://github.com/daliansky)的[Hackintosh](https://github.com/daliansky/Hackintosh)--加入我机型引导增加我EFI知名度
   
