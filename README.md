<div align="center">
  <img src="https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/hackintosh2.png" width="180" alt="Hackintosh">
  <h1>ASUS VivoBook FL8700JP (X509JP) 黑苹果项目</h1>

  [![OpenCore 0.9.7](https://img.shields.io/badge/OpenCore-0.9.7-0066CC?logo=apple&logoColor=white)](https://github.com/acidanthera/OpenCorePkg)
  [![macOS Catalina→Sonoma](https://img.shields.io/badge/macOS-Catalina→Sonoma-9999FF?logo=apple&logoColor=white)](https://www.apple.com/macos)
  [![License MIT](https://img.shields.io/badge/License-MIT-00AA00)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/blob/main/License)
  [![Last Commit](https://img.shields.io/github/last-commit/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh?color=FF9900)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/commits)
</div>

---

## 📖 目录
- [✅ 功能状态](#-功能状态)
- [⚙️ 硬件配置](#️-硬件配置)
- [📥 安装指南](#-安装指南)
- [❓ 常见问题](#-常见问题)
- [📸 实机效果](#-实机效果)
- [📜 版权声明](#-版权声明)

---

## ✅ 功能状态
| **功能模块**       | **状态** | **详细说明**                     |
|--------------------|----------|----------------------------------|
| **核显加速**       | ✔️ 正常  | Intel Iris Plus G7 完整驱动      |
| **WiFi/蓝牙**      | ✔️ 正常  | 支持通用控制/Apple Watch解锁      |
| **触控板手势**     | ✔️ 正常  | 支持多指操作和Mac原生手势         |
| **电池管理**       | ✔️ 正常  | 电量显示/充电状态                 |
| **Type-C接口**     | ✔️ 正常  | 支持USB设备/扩展坞（视频输出除外） |
| **HDMI输出**       | ❌ 不可用 | Ice Lake架构限制                 |
| **键盘背光**       | ❌ 不可用 | 硬件不支持                       |

---

## ⚙️ 硬件配置
| **组件**           | **型号**                                |
|---------------------|-----------------------------------------|
| 处理器              | Intel Core i7-1065G7 (Ice Lake, 10nm)   |
| 核显                | Intel Iris Plus Graphics G7 (64 EU)     |
| 无线网卡            | Intel Wireless-AC 9461 (160MHz)         |
| 触控板              | ELAN1200 (I2C协议)                      |
| 声卡                | Realtek ALC256 (Layout-id: 11)          |
| 硬盘                | 西部数据 SN550 512GB NVMe SSD           |

---

## 📥 安装指南
### BIOS关键设置
```bash
1. 关闭 Secure Boot
2. 禁用 Fast Boot
3. 硬盘模式设为 AHCI
4. DVMT预分配调整为 64MB
```

### EFI部署流程
```bash
# 使用Etcher写入macOS镜像到U盘
dd if=Install_macOS_Sonoma.dmg of=/dev/diskX bs=1m

# 挂载EFI分区并替换文件
diskutil mount disk0s1
cp -R EFI /Volumes/EFI/
```

### SMBIOS生成规则
| 推荐机型          | 标识符       | 验证要求                     |
|-------------------|--------------|------------------------------|
| MacBookPro16,2    | J680         | 序列号状态需显示「未验证」    |
| MacBookAir9,1     | J413         | 不可使用已注册的购买日期      |

---

## ❓ 常见问题
<details>
<summary><strong>Q: 安装时卡在「苹果Logo」界面？</strong></summary>

1. 检查BIOS中DVMT是否设置为64MB  
2. 尝试添加引导参数 `-v keepsyms=1` 查看错误日志  
3. 移除第三方SSDT补丁测试
</details>

<details>
<summary><strong>Q: Windows/macOS双系统时间不同步？</strong></summary>

在Windows中执行：
```regedit
reg add HKLM\SYSTEM\CurrentControlSet\Control\TimeZoneInformation /v RealTimeIsUniversal /t REG_DWORD /d 1
```
</details>

---

## 📸 实机效果
<div align="center">
  <img src="https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/blob/main/机型效果图/computer.png" width="45%">
  <img src="https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/blob/main/机型效果图/computer1.png" width="45%">
  <img src="https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/blob/main/机型效果图/computer2.png" width="45%">
  <img src="https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/blob/main/机型效果图/computer4.png" width="45%">
</div>

---

## 📜 版权声明
**MIT License**  
允许自由使用/修改/分发，但必须包含原始许可声明。  
完整协议见 [LICENSE](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/blob/main/License)

> © 2021-2024 [Aurora极光](https://github.com/bilijp153) | 由[若涵](https://github.com/catlingyun)提供测试支持
```

---
