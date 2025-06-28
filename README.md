<div align="center">
  <img src="./机型效果图/hackintosh2.png#gh-light-mode-only" width="180" alt="Hackintosh Logo">
  <img src="./机型效果图/hackintosh2-1.png#gh-dark-mode-only" width="180" alt="Hackintosh Logo">
  <h1>华硕 VivoBook FL8700JP 黑苹果</h1>
  <p>让 Windows 笔记本成功运行 macOS</p>
</div>

---

## 📌 快速导航([繁體中文](README_繁體中文.md))([English](README_en.md))

|[🌟 项目亮点](#-项目亮点) |[🚩 项目概览](#-项目概览) |[📸 实机展示](#-实机展示)|[💻 硬件兼容性](#-硬件兼容性) |
|------------------|------------------|----------------------------|----------------------------|
|[🖥️ 系统支持](#️-系统支持)|[⚙️ 安装指南](#️-安装指南) |[🛠️ 高级配置](#-高级配置) |[❓ 常见问题](#-常见问题) |
|[⚠️ 注意事项](#️-注意事项)|[🌟 贡献与支持](#️-贡献与支持) |[📮 问题反馈](#-问题反馈) |[🙏 致谢](#-致谢) |
---

## 🌟 项目亮点
- ✅ **完美兼容**：Catalina ~ Sequoia 全版本支持  
- 🖥 **硬件优化**：核显/声卡/网卡深度适配  
- 🚀 **性能调优**：原生CPU电源管理 + 智能睿频
- 🔋 **电源优化**： 原生电源管理 + 原生休眠支持 
- 🛠 **持续维护**：时不时更新 EFI 与问题修复  

---

## 🚩 项目概览
### 配置文件结构
```bash
EFI/                         # EFI 引导文文件夹
├── BOOT/                    # Boot 引导文文件夹
│   └── BOOTx64.efi          # UEFI 引导文件
└── OC/                      # OpenCore 引导文文件夹
    ├── ACPI/                # DSDT/SSDT 补丁
    ├── Kexts/               # 核心驱动
    ├── Drivers/             # OpenCore 驱动
    ├── config.plist         # 主配置文件
    └── ...                  # 其他资源文件
└── ...                      # 其他系统引导文件夹


```
### 注意事项
- **仅适配 ASUS FL8700JP (X509JP) 机型**，其他设备不保证兼容性。
- **不包含 macOS 镜像**，需自行准备安装文件。
- 安装前请备份数据，**操作风险自负**。
- 本项目遵循 [MIT 许可证](License)，禁止商业用途。

### [↩️ 返回快速导航](#-快速导航繁體中文english)

---

## 📸 实机展示
<div align="center">
  <img src="https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/computer1.png" width="45%">
  <img src="https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/computer2.png" width="45%">
</div>

---

## 💻 硬件兼容性
| 组件         | 型号                      | 状态     | 备注                     |
|--------------|---------------------------|----------|--------------------------|
| **处理器**   | Intel i7-1065G7           | ✅ 正常工作 | Ice Lake 架构           |
| **核显**     | Intel Iris Plus G7        | ⚠️ 部分支持 | 不支持HDMI 显示           |
| **独显**     | NVIDIA MX330              | ❌ 未支持  | 已屏蔽                  |
| **声卡**     | Realtek ALC256            | ✅ 正常工作 | 支持外设接入自动切换       |
| **无线网卡** | Intel Wireless-AC 9461    | ✅ 部分支持 | 不支持隔空投送等原生功能         |
| **触控板**   | ELAN1200                  | ⚠️ 部分支持 | 偶发无响应（需重启）   |
| **Type-C**   | -                         | ✅ 部分支持 | 不支持DP显示和雷电功能   |

---

## 🖥️ 系统支持
| 系统版本       | 兼容性 | 最低支持版本        |
|----------------|--------|---------------------|
| Catalina | ✅      | 10.15.4            |
| Big Sur        | ✅      | 11.0               |
| Monterey       | ✅      | 12.0               |
| Ventura        | ✅      | 13.0               |
| Sonoma         | ✅      | 14.0               |
| Sequoia        | ✅      | 15.0               |

### [↩️ 返回快速导航](#-快速导航繁體中文english)

---

## ⚙️ 安装指南
### 1. BIOS 设置

1. (Secure Boot) ➔ 关闭 (Disabled)
2. 快速启动(Fast Boot) ➔ 关闭 (Disabled)
3. DVMT 预分配(DVMT Pre-Allocated) ➔ 64M


### 2. 安装步骤

1. 下载Mac OS 镜像 ➔ 推荐使用[黑果小兵的部落阁](https://blog.daliansky.net/)
2. 制作 Mac OS 安装盘 ➔ 推荐使用 [BalenaEtcher](https://www.balena.io/etcher/)
3. [**下载**](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/releases)EFI 文件 ➔ 解压至 USB 驱动器替换原有EFI文件夹
4. 下载[SSDTTime](https://github.com/corpnewt/SSDTTime)按照提示提取本机SSDT,找到提取出来的SSDT文件夹，把里面的**FACP.aml**重命名为**SSDT-FACP.aml**替换**EFI/OC/ACPI**里的**SSDT-FACP.aml**
5. 调整启动顺序 ➔ 从 USB 启动
6. 运行 OpenCore ➔ 选择 "Install macOS XXX"
7. 多次重启后进入Mac开箱界面
8. 完成设置后 ➔ 迁移 EFI 至本机固态EFI分区并移除U盘



### 3. SMBIOS 配置

1. 使用 **OpenCore Configurator**或者[**OCAuxiliaryTools**](https://github.com/ic005k/OCAuxiliaryTools)打开**config**
2. 修改机型为**MacBookPro16,2**
3. 生成有效 **SystemSerialNumber** 并于 Apple [查看保障信息](https://checkcoverage.apple.com/)验证
4. 保存**config**文件并重启

---

## 🛠️ 高级配置

💻 BootCamp 双系统配置

1. 访问 [**brigadier**](https://github.com/corpnewt/brigadier)下载所需文件
2. 解压后运行其中的**commamd**文件并按照提示要求操作
3. 把生成的**dmg**文件打开复制其中的两个文件夹到Windows系统盘符
4. 使用 **OpenCore Configurator**或者[**OCAuxiliaryTools**](https://github.com/ic005k/OCAuxiliaryTools)修改**config**里面的**pl**项目中的**updateSMBIOSMod**为**Create**并保存重启
5. **OpenCore**界面选择**Windows**来启动到Windows
6. 打开复制到Windows盘符的其中交**BootCamp**的文件夹里面的**Setup.exe**并按提示安装软件
7. 安装完成后按照提示重启电脑
8. 回到Mac使用 **OpenCore Configurator**或者[**OCAuxiliaryTools**](https://github.com/ic005k/OCAuxiliaryTools)修改**config**里面的**pl**项目中的**updateSMBIOSMod**为**Custom**并保存重启


### [↩️ 返回快速导航](#-快速导航繁體中文english)

---

## ❓ 常见问题
<details>
  <summary><b>Q: 开机有“咚”声如何关闭？</b></summary>
  前往 系统设置 ➔ 声音 关闭「启动时播放声音」。
</details>

<details>
  <summary><b>Q: 触控板偶发失灵？</b></summary>
  暂时需重启或睡眠唤醒恢复，此为 ELAN1200 驱动已知问题。
</details>

<details>
  <summary><b>Q: 如何切换默认系统？</b></summary>
  OpenCore 界面按 Ctrl+Enter 或「系统设置」➔「启动磁盘」。
</details>

---

## ⚠️ 注意事项
1. 开箱界面里提示登录AppleID时必须先**跳过**后续在**系统设置**中登录
2. 必须生成**唯一三码**且验证验证序列号状态显示 **"无效序列号"**
3. 完成后就可以尝试注册并登录你的AppleID

---

## 🌟 贡献与支持
| 角色 | 贡献者 |
|------|--------|
| 维护 |  [极光呆呆脑](https://github.com/bilijp153) |
| 测试 |  [若涵](https://github.com/catlingyun) |

---

## 📮 问题反馈
提交至 [GitHub Issues](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/issues) 或联系：  
📧 **邮箱**: 1551656605@qq.com 

<a href="https://space.bilibili.com/329351708">
    <img src="https://img.shields.io/badge/哔哩哔哩-极光呆呆脑-FF69B4?logo=bilibili" alt="Bilibili">
  </a>
  <a href="https://weibo.com/u/5264002671">
    <img src="https://img.shields.io/badge/新浪微博-草莓小极光-1DA1F2?logo=sinaweibo" alt="sinaweibo">
  </a>
  <a href="https://qm.qq.com/cgi-bin/qm/qr?k=B2Omg5IKCGWoMNXgMIPmA_AJqEMnMCUb&noverify=0&personal_qrcode_source=3">
    <img src="https://img.shields.io/badge/腾讯QQ-极光呆呆脑-26A5E4?logo=QQ" alt="QQ">
  </a>

---

## 🙏 致谢
- [OpenCore 官方指南](https://dortania.github.io/OpenCore-Install-Guide/)
- [Acidanthera](https://github.com/acidanthera) 驱动开发团队
- [laobamac](https://github.com/laobamac) OCLP-Mod开发者

### [↩️ 返回快速导航](#-快速导航繁體中文english)

---

<div align="center">
  
本项目基于[MIT 许可证](License)开源  

© 2021-2025 极光呆呆脑 保留所有权利
</div>

