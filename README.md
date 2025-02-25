<div align="center">
  <img src="https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/hackintosh2.png" width="180" alt="Hackintosh Logo">
  <h1>ASUS VivoBook FL8700JP (X509JP) 黑苹果项目</h1>

  [![OpenCore Version](https://img.shields.io/badge/OpenCore-0.9.7-blue?logo=apple)](https://github.com/acidanthera/OpenCorePkg)
  [![macOS Support](https://img.shields.io/badge/macOS-Catalina→Sonoma-9cf?logo=apple)](https://www.apple.com/macos)
  [![License MIT](https://img.shields.io/badge/License-MIT-green)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/blob/main/License)
  [![Last Commit](https://img.shields.io/github/last-commit/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh?color=orange)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/commits)

  [快速跳转](#-目录) | [下载EFI](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/releases) | [问题反馈](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/issues)
</div>

---

## 🌐 语言选择
- [简体中文](README.md) | [繁體中文](README_繁體中文.md) | [English](README_en.md)

---

## 📌 核心信息
<details>
<summary><strong>✅ 工作状态概览</strong></summary>

| 功能           | 状态 | 备注                  |
|----------------|------|-----------------------|
| 核显加速       | ✔️   | Iris Plus Graphics G7 |
| 声卡/麦克风    | ✔️   | ALC256                |
| WiFi/蓝牙      | ✔️   | Intel AC9461          |
| 触控板手势     | ✔️   | ELAN1200              |
| 睡眠唤醒       | ✔️   | 需终端命令优化        |
| HDMI输出       | ❌   | Ice Lake架构限制      |
| 键盘背光       | ❌   | 硬件不支持            |
</details>

<details>
<summary><strong>⚙️ 硬件配置</strong></summary>

| 组件           | 型号                          |
|----------------|-------------------------------|
| 处理器         | Intel i7-1065G7 (Ice Lake)    |
| 核显           | Intel Iris Plus Graphics G7   |
| 内存           | 12GB DDR4 (8+4)               |
| 存储           | WD 512GB SSD                  |
| 无线网卡       | Intel Wireless-AC 9461        |
| 触控板         | ELAN1200                      |
</details>

---

## 🚀 快速开始
### 安装准备
1. **BIOS设置**  
   - 关闭 `Secure Boot` 和 `Fast Boot`  
   - 硬盘模式设为 `AHCI`  
   - DVMT预分配设置为 `64MB`

2. **下载工具**  
   - [EFI文件](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/releases)  
   - [Etcher](https://www.balena.io/etcher/)（制作启动盘）  

3. **安装步骤**  
   ```bash
   # 1. 将EFI写入U盘EFI分区
   # 2. 从U盘启动进入OpenCore
   # 3. 安装macOS并迁移EFI到系统盘
   ```

---

## 🛠️ 高级配置
### SMBIOS三码生成
使用 [OpenCore Configurator](https://mackie100projects.altervista.org/) 生成唯一的三码：
1. 选择机型：**MacBookPro16,2** 或 **MacBookAir9,1**  
2. 验证序列号状态需显示「无效」或「未验证购买日期」

### BootCamp支持
```bash
# 使用brigadier工具获取驱动
git clone https://github.com/corpnewt/brigadier
python brigadier -m MacBookPro16,2
```

---

## 📸 实机预览
<div align="center">
  <img src="https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/blob/main/机型效果图/computer.png" width="45%">
  <img src="https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/blob/main/机型效果图/computer1.png" width="45%">
</div>

---

## ❓ 常见问题
**Q: HDMI无信号输出？**  
A: Ice Lake处理器原生不支持HDMI，需通过Type-C转接DP。

**Q: 触控板间歇失灵？**  
A: ELAN1200固件问题，暂时通过重启或睡眠唤醒恢复。

**Q: Windows/macOS切换后无声？**  
A: Windows需使用微软官方声卡驱动，禁用Realtek驱动。

---

## 📜 版权声明
本项目基于 [MIT License](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/blob/main/License)，严禁用于商业用途。  
© 2021-2024 [Aurora极光](https://github.com/bilijp153) | [若涵](https://github.com/catlingyun)

[返回顶部](#-目录)
