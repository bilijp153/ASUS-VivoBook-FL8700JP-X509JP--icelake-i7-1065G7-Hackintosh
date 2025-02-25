<div align="center">

<img align="center" width="180" src="https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/hackintosh2.png" style="max-width: 100%; height: auto;">
<h1>ASUS VivoBook FL8700JP (X509JP) Hackintosh</h1>

[![GitHub License](https://img.shields.io/github/license/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh?label=License&style=flat-square)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/License)
[![Latest Release](https://img.shields.io/github/v/release/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh?label=Download&style=flat-square)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/releases)
[![OpenCore Version](https://img.shields.io/badge/OpenCore-0.9.7+-blue?style=flat-square)](https://github.com/acidanthera/OpenCorePkg)

![Preview](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/简体1.png)

</div>

---

## 📋 目录
- [📦 配置要求](#-配置要求)
- [✅ 兼容性](#-兼容性)
- [⚙️ 功能状态](#️-功能状态)
- [📥 安装指南](#-安装指南)
- [❓ 常见问题](#-常见问题)
- [📜 更新日志](更新日志.md)
- [🙏 致谢](#-致谢)

---

## 📦 配置要求
| **组件**       | **型号**                         |
|----------------|----------------------------------|
| **处理器**     | Intel Core i7-1065G7 (Ice Lake)  |
| **核显**       | Intel Iris Plus Graphics G7      |
| **内存**       | 12GB DDR4 (8+4)                  |
| **存储**       | Western Digital 512GB SSD        |
| **无线网卡**   | Intel Wireless-AC 9461           |
| **声卡**       | Realtek ALC256                   |

---

## ✅ 兼容性
| **macOS 版本** | **支持状态** |
|----------------|--------------|
| Catalina       | ✅ 10.15.4+   |
| Big Sur        | ✅            |
| Monterey       | ✅            |
| Ventura        | ✅            |
| Sonoma         | ✅            |

---

## ⚙️ 功能状态
| **功能**         | **状态** | **备注**                     |
|------------------|----------|------------------------------|
| 核显加速         | ✅        | 支持4K输出                   |
| 无线网络         | ✅        | 2.4G/5G双频                  |
| 蓝牙             | ✅        | 文件传输支持                 |
| 触控板手势       | ✅        | 多指操作流畅                 |
| 睡眠唤醒         | ✅        | 需设置`standbydelay`         |
| HDMI输出         | ❌        | Ice Lake架构限制             |
| 独立显卡（MX330）| ❌        | 已屏蔽                       |

---

## 📥 安装指南
### 准备工作
1. **BIOS设置**  
   - 关闭 `Secure Boot` 和 `Fast Boot`  
   - 硬盘模式设为 `AHCI`  
   - 调整DVMT为 `64MB`

2. **创建安装盘**  
   ```bash
   # 使用终端命令创建安装盘
   sudo /Applications/Install\ macOS\ Ventura.app/Contents/Resources/createinstallmedia --volume /Volumes/MyVolume
   ```

3. **替换EFI**  
   将本仓库的EFI文件复制到U盘的EFI分区。

### 多系统引导
- **Windows/Mac切换**：在OpenCore引导界面按 `Ctrl+Enter` 设置默认启动项  
- **BootCamp支持**：使用 [brigadier](https://github.com/corpnewt/brigadier) 安装驱动  

---

## ❓ 常见问题
<details>
<summary>Q: HDMI无法使用怎么办？</summary>
A: Ice Lake处理器原生不支持HDMI输出，建议使用Type-C转DP。
</details>

<details>
<summary>Q: 触控板间歇性失灵？</summary>
A: ELAN1200固件问题，暂时可通过重启或睡眠唤醒恢复。
</details>

<details>
<summary>Q: 如何关闭启动音效？</summary>
A: 系统设置 > 声音 > 取消勾选"启动时播放声音"。
</details>

---

## 🙏 致谢
- [OpenCore官方指南](https://dortania.github.io/OpenCore-Install-Guide/)
- [Acidanthera](https://github.com/acidanthera) 提供核心驱动
- [@catlingyun](https://github.com/catlingyun) 参与测试

---

<div align="center">
📧 反馈请提交至 <a href="https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/issues">Issues</a>  
© 2021-2024 Aurora极光 | MIT License
</div>

---