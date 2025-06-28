# 华硕 VivoBook FL8700JP 黑苹果项目

<div align="center">
  <img src="./机型效果图/hackintosh2.png#gh-light-mode-only" width="180" alt="Hackintosh Logo">
  <img src="./机型效果图/hackintosh2-1.png#gh-dark-mode-only" width="180" alt="Hackintosh Logo">
  <h1>让 Windows 笔记本完美运行 macOS</h1>
  <p>为华硕 VivoBook FL8700JP (X509JP) 定制的黑苹果解决方案</p>
  
  ![OpenCore Version](https://img.shields.io/badge/OpenCore-1.0.4-blue)
  ![macOS Support](https://img.shields.io/badge/macOS-Catalina→Sequoia-green)
  ![License](https://img.shields.io/badge/License-MIT-lightgrey)
</div>

---

## 📌 快速导航
| [🌟 核心优势](#-核心优势) | [📸 效果展示](#-效果展示) | [💻 硬件支持](#-硬件支持) |
|--------------------------|--------------------------|--------------------------|
| [🖥️ 系统兼容](#️-系统兼容) | [⚙️ 安装指南](#️-安装指南) | [🛠️ 高级配置](#️-高级配置) |
| [❓ 常见问题](#-常见问题) | [⚠️ 重要提示](#️-重要提示) | [🤝 参与贡献](#-参与贡献) |

---

## 🌟 核心优势
- **全面系统支持**：从 Catalina 到 Sequoia 全版本完美运行
- **深度硬件优化**：核显/声卡/网卡等关键组件完美驱动
- **性能极致发挥**：原生电源管理 + 智能睿频技术
- **电池效率提升**：原生休眠支持 + 高效能耗控制
- **持续维护更新**：定期优化 EFI 配置，修复已知问题

> "这不是简单的黑苹果安装，而是让您的华硕笔记本获得接近原生 MacBook 的体验"

---

## 🖥 项目结构
### EFI 配置文件
```bash
EFI/
├── BOOT/
│   └── BOOTx64.efi
└── OC/
    ├── ACPI/          # 系统补丁与修复
    ├── Kexts/         # 核心硬件驱动
    ├── Drivers/       # OpenCore 引导驱动
    ├── config.plist   # 主配置文件
    └── Tools/         # 实用工具集合
```

### ⚠️ 重要说明
1. **专属适配**：仅适用于华硕 FL8700JP (X509JP) 特定机型
2. **系统准备**：需自行获取 macOS 安装镜像
3. **风险提示**：操作前请务必备份重要数据
4. **授权许可**：遵循 [MIT 许可证](LICENSE)，禁止商业用途

---

## 📸 效果展示
<div align="center">
  <img src="https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/computer1.png" width="45%" alt="系统概览">
  <img src="https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/computer2.png" width="45%" alt="硬件信息">
</div>

---

## 💻 硬件支持
| 组件         | 型号                      | 状态       | 详细说明               |
|--------------|---------------------------|------------|------------------------|
| **处理器**   | Intel i7-1065G7           | ✅ 完美支持 | Ice Lake 架构优化     |
| **核显**     | Intel Iris Plus G7        | ⚠️ 基本支持 | 不支持 HDMI 输出      |
| **独立显卡** | NVIDIA MX330              | ❌ 不支持   | 已在配置中屏蔽        |
| **音频**     | Realtek ALC256            | ✅ 完美支持 | 自动切换输入/输出设备 |
| **无线网络** | Intel Wireless-AC 9461    | ⚠️ 部分支持 | 不支持隔空投送       |
| **触控板**   | ELAN1200                  | ⚠️ 基本支持 | 偶发无响应            |
| **Type-C**   | -                         | ⚠️ 部分支持 | 不支持视频输出        |

---

## 🖥️ 系统兼容
| macOS 版本   | 兼容状态 | 最低要求版本 |
|--------------|----------|--------------|
| Catalina     | ✅ 完美  | 10.15.4      |
| Big Sur      | ✅ 完美  | 11.0         |
| Monterey     | ✅ 完美  | 12.0         |
| Ventura      | ✅ 完美  | 13.0         |
| Sonoma       | ✅ 完美  | 14.0         |
| Sequoia      | ✅ 完美  | 15.0         |

---

## ⚙️ 安装指南
### 准备工作
1. **BIOS 设置**：
   - 禁用 Secure Boot
   - 关闭 Fast Boot
   - 设置 DVMT 预分配为 64M

2. **安装介质**：
   - 下载 macOS 镜像（推荐[黑果小兵的部落阁](https://blog.daliansky.net/)）
   - 使用 [BalenaEtcher](https://www.balena.io/etcher/) 创建安装U盘

### 安装步骤
1. 下载项目 [EFI 文件](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/releases)
2. 使用 [SSDTTime](https://github.com/corpnewt/SSDTTime) 提取本机 ACPI 表
   ```bash
   SSDTTime 提取 → FACP.aml → 重命名为 SSDT-FACP.aml
   ```
3. 替换 EFI/OC/ACPI 中的对应文件
4. 从U盘启动进入 OpenCore
5. 选择 "Install macOS" 开始安装
6. 完成安装后迁移 EFI 到系统分区

### SMBIOS 配置
1. 使用 [OCAuxiliaryTools](https://github.com/ic005k/OCAuxiliaryTools) 编辑 config.plist
2. 设置机型为 **MacBookPro16,2**
3. 生成有效三码并在 [Apple 官网](https://checkcoverage.apple.com/) 验证

---

## 🛠️ 高级配置
### 双系统安装 (BootCamp)
```mermaid
graph LR
A[下载 brigadier] --> B[生成 BootCamp 文件]
B --> C[复制到 Windows 分区]
C --> D[修改 config.plist]
D --> E[安装 BootCamp 驱动]
E --> F[恢复 config 设置]
```

1. 从 [brigadier](https://github.com/corpnewt/brigadier) 获取 BootCamp 支持文件
2. 将生成的 BootCamp 文件夹复制到 Windows 系统盘
3. 修改 config.plist 中 PlatformInfo → updateSMBIOSMode 为 `Create`
4. 重启进入 Windows 并安装 BootCamp
5. 完成后恢复 updateSMBIOSMode 为 `Custom`

---

## ❓ 常见问题
### 开机提示音问题
> **Q: 如何关闭开机时的"咚"声？**  
> 前往"系统设置" → "声音" → 取消勾选"启动时播放声音"

### 触控板问题
> **Q: 触控板偶尔无响应怎么办？**  
> 这是 ELAN1200 驱动的已知问题，暂时可通过重启或睡眠唤醒恢复

### 默认系统设置
> **Q: 如何更改默认启动系统？**  
> 在 OpenCore 界面按 `Ctrl+Enter` 或进入 macOS 后通过"系统设置" → "启动磁盘"设置

---

## ⚠️ 重要提示
1. **首次设置**：在初始化界面跳过 Apple ID 登录，完成系统设置后再登录
2. **三码验证**：序列号在 Apple 官网应显示"无效序列号"状态
3. **安全登录**：完成上述步骤后再登录您的 Apple ID

---

## 🤝 参与贡献
### 核心团队
| 角色       | 贡献者                     | 联系方式                |
|------------|----------------------------|-------------------------|
| 项目维护   | [极光呆呆脑](https://github.com/bilijp153) | 1551656605@qq.com      |
| 测试验证   | [若涵](https://github.com/catlingyun)    |                         |

### 反馈渠道
- [提交 Issue](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/issues)
- 社区支持：
  [![Bilibili](https://img.shields.io/badge/哔哩哔哩-极光呆呆脑-FF69B4?logo=bilibili)](https://space.bilibili.com/329351708)
