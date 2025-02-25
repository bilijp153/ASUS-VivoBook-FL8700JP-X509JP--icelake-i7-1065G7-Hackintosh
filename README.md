<div align="center">
  <img src="https://img.shields.io/badge/Hackintosh-Professional-blue?style=for-the-badge&logo=apple" alt="Hackintosh"/>
  <h1>ASUS VivoBook FL8700JP/X509JP Hackintosh</h1>
  <p>Intel Ice Lake i7-1065G7 | macOS Ventura/Sonoma</p>
 
  ![Platform](https://img.shields.io/badge/macOS-13/14-9cf?style=flat-square)
  ![OC](https://img.shields.io/badge/OpenCore-0.9.8-cyan?style=flat-square)
  ![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)
</div>
 
<div align="center">
  <img src="https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-X509JP--icelake-i7-1065G7-Hackintosh/raw/main/Images/ShowCase.png" width="80%" alt="Showcase"/>
</div>
 
## 📋 目录导航 
- [硬件配置](#-硬件配置)
- [兼容性状态](#-兼容性状态)
- [安装指南](#-安装指南)
- [重要提示](#-重要提示)
- [更新日志](#-更新日志)
- [致谢与协议](#-致谢与协议)
 
---
 
## 🖥️ 硬件配置 
| 组件         | 型号                          |
|--------------|-------------------------------|
| 处理器       | Intel Core i7-1065G7 (Ice Lake) |
| 内存         | 16GB DDR4 2666MHz             |
| 存储         | WD SN530 512GB NVMe           |
| 显示屏       | 17.3" 1920x1080 IPS           |
| 无线网卡     | Intel AX201                   |
 
---
 
## ✅ 兼容性状态 
### 核心功能 
| 功能         | 状态 | 备注                  |
|--------------|------|-----------------------|
| 显卡加速     | ✅   | Metal 3 支持          |
| 声音输出     | ✅   | 内置扬声器/耳机       |
| 电源管理     | ✅   | 原生电源控制          |
| USB端口      | ✅   | 全类型映射            |
| 摄像头       | ✅   | 720p HD               |
 
### 无线功能 
| 功能         | 状态 | 备注                  |
|--------------|------|-----------------------|
| WiFi         | ✅   | AX201 驱动正常        |
| 蓝牙         | ✅   | 文件传输/外设支持     |
| 隔空投送     | ❌   | 需更换网卡            |
 
---
 
## 🔧 安装指南 
<details>
<summary><strong>点击查看详细安装步骤</strong></summary>
 
1. **BIOS设置**
   ```bash 
   Advanced → Graphics Configuration → DVMT Pre-Allocated → 64M 
 
驱动准备
使用OpenCore Configurator配置PlatformInfo
确保SMBIOS选择MacBookPro16,2
安装后优化
 
sudo pmset autopoweroff 0 
sudo pmset powernap 0 
 
 
## ⚠️ 重要提示
需要禁用BIOS中的 Secure Boot 
推荐使用HIDPI缩放工具优化显示效果
系统更新前请先验证OpenCore兼容性
 
## 📅 更新日志
2025.02.25
升级OpenCore至0.9.8正式版
修复USB-C接口唤醒问题
优化电池电量显示算法
 
## 📜 致谢与协议
特别感谢 Acidanthera 团队的开源贡献
本项目遵循 MIT License
免责声明：Hackintosh安装存在风险，作者不对任何硬件损坏负责
