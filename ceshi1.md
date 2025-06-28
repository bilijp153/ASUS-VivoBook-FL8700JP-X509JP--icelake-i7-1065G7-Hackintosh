# 🍎 华硕 VivoBook FL8700JP 黑苹果项目 - 完美运行 macOS

<div align="center">
  <img src="./机型效果图/hackintosh2.png#gh-light-mode-only" width="180" alt="Hackintosh Logo">
  <img src="./机型效果图/hackintosh2-1.png#gh-dark-mode-only" width="180" alt="Hackintosh Logo">
  <h1>让 Windows 笔记本完美运行 macOS</h1>
  <p>为华硕 VivoBook FL8700JP (X509JP) 定制的黑苹果解决方案</p>
  
  <div class="badges">
    <img src="https://img.shields.io/badge/OpenCore-1.0.4-blue?style=for-the-badge&logo=apple" alt="OpenCore">
    <img src="https://img.shields.io/badge/macOS-Catalina→Sequoia-green?style=for-the-badge&logo=apple" alt="macOS Support">
    <img src="https://img.shields.io/badge/License-MIT-lightgrey?style=for-the-badge" alt="License">
    <img src="https://img.shields.io/badge/Status-Active-brightgreen?style=for-the-badge" alt="Status">
  </div>
</div>

---

## 🚀 项目亮点概览

<div class="features-grid">
  <div class="feature-card">
    <div class="icon">💯</div>
    <h3>全版本支持</h3>
    <p>Catalina 到 Sequoia 全兼容</p>
  </div>
  
  <div class="feature-card">
    <div class="icon">⚡</div>
    <h3>极致性能</h3>
    <p>原生电源管理 + 智能睿频</p>
  </div>
  
  <div class="feature-card">
    <div class="icon">🔋</div>
    <h3>电池优化</h3>
    <p>原生休眠支持 + 高效能耗控制</p>
  </div>
  
  <div class="feature-card">
    <div class="icon">🔧</div>
    <h3>持续维护</h3>
    <p>定期更新优化，修复问题</p>
  </div>
</div>

> "这不是简单的黑苹果安装，而是让您的华硕笔记本获得接近原生 MacBook 的体验"

---

## 📚 目录导航

1. [🌟 核心优势](#-核心优势)
2. [🖥 项目结构](#-项目结构)
3. [📸 效果展示](#-效果展示)
4. [💻 硬件支持](#-硬件支持)
5. [🖥️ 系统兼容](#️-系统兼容)
6. [⚙️ 安装指南](#️-安装指南)
7. [🛠️ 高级配置](#️-高级配置)
8. [❓ 常见问题](#-常见问题)
9. [⚠️ 重要提示](#️-重要提示)
10. [🤝 参与贡献](#-参与贡献)

---

## 🌟 核心优势

### 🚀 全面系统支持
从 Catalina 到 Sequoia 全版本完美运行，提供无缝升级体验

### 🔧 深度硬件优化
- Intel Iris Plus G7 核显完美驱动
- Realtek ALC256 声卡完整支持
- 原生电源管理 + CPU 睿频技术
- USB 端口定制化映射

### 🔋 电池效率提升
- 原生休眠支持
- 智能能耗控制
- 电池状态精确显示
- 低功耗模式优化

### 🛠 持续维护更新
- 定期优化 EFI 配置
- 及时修复已知问题
- 适配最新 macOS 版本
- 社区驱动持续改进

---

## 🖥 项目结构

### 📂 EFI 配置文件结构

```bash
EFI/
├── BOOT/
│   └── BOOTx64.efi              # 引导文件
└── OC/
    ├── ACPI/                    # 系统补丁与修复
    │   ├── SSDT-AWAC.aml        # 时钟控制器修复
    │   ├── SSDT-EC-USBX.aml     # 嵌入式控制器
    │   └── SSDT-PLUG.aml        # CPU电源管理
    ├── Kexts/                   # 核心硬件驱动
    │   ├── Lilu.kext            # 核心插件
    │   ├── VirtualSMC.kext      # 系统管理控制器
    │   ├── WhateverGreen.kext   # 显卡修复
    │   └── AppleALC.kext        # 声卡驱动
    ├── Drivers/                 # OpenCore 引导驱动
    │   ├── OpenRuntime.efi      # 运行时服务
    │   └── HfsPlus.efi          # HFS+文件系统支持
    ├── config.plist             # 主配置文件
    └── Tools/                   # 实用工具集合
```

### ⚠️ 重要说明

<div class="notice">
  <div class="notice-header">专属适配</div>
  <p>仅适用于华硕 FL8700JP (X509JP) 特定机型</p>
</div>

<div class="notice warning">
  <div class="notice-header">系统准备</div>
  <p>需自行获取 macOS 安装镜像</p>
</div>

<div class="notice important">
  <div class="notice-header">风险提示</div>
  <p>操作前请务必备份重要数据</p>
</div>

<div class="notice">
  <div class="notice-header">授权许可</div>
  <p>遵循 <a href="LICENSE">MIT 许可证</a>，禁止商业用途</p>
</div>

---

## 📸 效果展示

<div class="gallery">
  <div class="gallery-item">
    <img src="https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/computer1.png" alt="系统概览">
    <p>系统信息概览</p>
  </div>
  <div class="gallery-item">
    <img src="https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/computer2.png" alt="硬件信息">
    <p>详细硬件信息</p>
  </div>
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
| **蓝牙**     | Intel Bluetooth           | ✅ 完美支持 | 完整功能              |
| **摄像头**   | 720p HD Camera            | ✅ 完美支持 | FaceTime 兼容         |

---

## 🖥️ 系统兼容

| macOS 版本   | 兼容状态 | 最低要求版本 | 备注                  |
|--------------|----------|--------------|-----------------------|
| **Catalina** | ✅ 完美  | 10.15.4      | 完全兼容              |
| **Big Sur**  | ✅ 完美  | 11.0         | 推荐版本              |
| **Monterey** | ✅ 完美  | 12.0         | 最佳性能              |
| **Ventura**  | ✅ 完美  | 13.0         | 完整功能支持          |
| **Sonoma**   | ✅ 完美  | 14.0         | 需最新EFI            |
| **Sequoia**  | ✅ 完美  | 15.0         | 开发者测试版兼容      |

---

## ⚙️ 安装指南

### 准备工作

1. **BIOS 设置**：
   - 禁用 Secure Boot
   - 关闭 Fast Boot
   - 设置 DVMT 预分配为 64M
   - 禁用 CFG Lock（如支持）

2. **安装介质**：
   - 下载 macOS 镜像（推荐[黑果小兵的部落阁](https://blog.daliansky.net/)）
   - 使用 [BalenaEtcher](https://www.balena.io/etcher/) 创建安装U盘

### 安装流程

```plaintext
1. 下载EFI文件      → 2. 提取本机ACPI表 → 3. 替换ACPI文件
       ↓                                      ↓
8. 配置SMBIOS    ← 7. 迁移EFI        ← 6. 安装系统      ← 4. 启动安装
```

### 详细步骤

1. **下载项目文件**  
   访问 [发布页面](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/releases) 下载最新EFI

2. **提取本机 ACPI 表**  
   ```bash
   # 使用 SSDTTime 提取必要文件
   SSDTTime 提取 → FACP.aml → 重命名为 SSDT-FACP.aml
   ```

3. **替换配置文件**  
   将生成的SSDT文件放入 `EFI/OC/ACPI` 目录

4. **启动安装**  
   - 从U盘启动进入 OpenCore
   - 选择 "Install macOS"
   - 按照屏幕提示完成安装

5. **迁移 EFI**  
   安装完成后，使用 [MountEFI](https://github.com/corpnewt/MountEFI) 工具将EFI迁移到系统分区

6. **SMBIOS 配置**  
   ```bash
   1. 使用 OCAuxiliaryTools 编辑 config.plist
   2. 设置机型为 MacBookPro16,2
   3. 生成三码并验证
   ```

---

## 🛠️ 高级配置

### 双系统安装 (BootCamp)

```plaintext
+----------------+     +-----------------+     +-----------------+
| 下载 brigadier | --> | 生成 BootCamp   | --> | 复制到 Windows  |
|                |     | 支持文件        |     | 分区           |
+----------------+     +-----------------+     +-----------------+
                          |                           |
                          v                           v
+----------------+     +-----------------+     +-----------------+
| 修改 config    | <-- | 安装 BootCamp   | <-- | 重启进入 Windows|
| 恢复设置       |     | 驱动            |     |                 |
+----------------+     +-----------------+     +-----------------+
```

1. 从 [brigadier](https://github.com/corpnewt/brigadier) 获取 BootCamp 支持文件
2. 将生成的 BootCamp 文件夹复制到 Windows 系统盘
3. 修改 config.plist:
   ```xml
   <key>PlatformInfo</key>
   <dict>
     <key>updateSMBIOSMode</key>
     <string>Create</string>
   </dict>
   ```
4. 重启进入 Windows 并安装 BootCamp
5. 完成后恢复 updateSMBIOSMode 为 `Custom`

### 性能优化技巧
- 启用 `XCPM` 电源管理
- 调整 `HWP` 参数提升睿频响应
- 使用 `CPUFriend` 定制电源配置
- 禁用不必要的内核扩展

---

## ❓ 常见问题

<details>
<summary><strong>Q: 如何关闭开机时的"咚"声？</strong></summary>
<p>前往"系统设置" → "声音" → 取消勾选"启动时播放声音"</p>
</details>

<details>
<summary><strong>Q: 触控板偶尔无响应怎么办？</strong></summary>
<p>这是 ELAN1200 驱动的已知问题，暂时可通过以下方法解决：</p>
<ul>
  <li>重启系统</li>
  <li>进入睡眠模式后唤醒</li>
  <li>使用终端命令: <code>sudo killall AppleMultitouchDriver</code></li>
</ul>
</details>

<details>
<summary><strong>Q: 如何更改默认启动系统？</strong></summary>
<p>两种方法：</p>
<ol>
  <li>在 OpenCore 启动界面按 <code>Ctrl+Enter</code> 设置默认启动项</li>
  <li>进入 macOS 后通过"系统设置" → "启动磁盘"设置</li>
</ol>
</details>

<details>
<summary><strong>Q: 蓝牙设备连接不稳定？</strong></summary>
<p>尝试以下解决方案：</p>
<ul>
  <li>重置蓝牙模块: <code>sudo pkill bluetoothd</code></li>
  <li>更新 <code>IntelBluetoothFirmware</code> 驱动</li>
  <li>检查 USB 映射是否包含蓝牙控制器</li>
</ul>
</details>

---

## ⚠️ 重要提示

1. **首次设置**  
   在初始化界面跳过 Apple ID 登录，完成系统设置后再登录

2. **三码验证**  
   序列号在 [Apple 官网](https://checkcoverage.apple.com/) 应显示"无效序列号"状态

3. **安全登录**  
   完成上述步骤后再登录您的 Apple ID，避免账户异常

4. **系统更新**  
   每次进行 macOS 系统更新前：
   - 备份当前 EFI 分区
   - 检查项目更新日志
   - 等待社区确认兼容性

---

## 🤝 参与贡献

### 核心团队

| 角色       | 贡献者                     | 联系方式                |
|------------|----------------------------|-------------------------|
| 项目维护   | [极光呆呆脑](https://github.com/bilijp153) | 1551656605@qq.com      |
| 测试验证   | [若涵](https://github.com/catlingyun)    | catlingyun@example.com |

### 贡献流程

```plaintext
1. Fork 项目仓库         2. 创建特性分支       3. 提交修改
       ↑                         |                      |
       +-------------------------+----------------------+
                                 ↓
                          4. 发起 Pull Request
```

### 反馈渠道
- [提交 Issue](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/issues)
- 发送邮件至: support@hackintosh-fl8700jp.com
- 加入 Telegram 讨论组

---

## 🙏 特别鸣谢

- [OpenCore 官方指南](https://dortania.github.io/OpenCore-Install-Guide/) - 黑苹果安装的黄金标准
- [Acidanthera](https://github.com/acidanthera) - 提供核心驱动开发
- [laobamac](https://github.com/laobamac) - OCLP-Mod 开发者
- [Dortania 社区](https://dortania.github.io) - 技术支持与知识库
- [黑果小兵](https://blog.daliansky.net/) - 优质安装镜像资源

---

<div align="center">
  
📜 **许可证**: [MIT](LICENSE)  
© 2021-2025 极光呆呆脑 - 保留所有权利

> **温馨提示**：本项目仅用于学习和研究目的，使用 macOS 请遵守苹果公司相关协议

</div>

<style>
  .features-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 20px;
    margin: 30px 0;
  }
  
  .feature-card {
    background: linear-gradient(135deg, #f5f7fa 0%, #e4edf5 100%);
    border-radius: 12px;
    padding: 20px;
    text-align: center;
    box-shadow: 0 4px 6px rgba(0,0,0,0.1);
    transition: transform 0.3s ease;
  }
  
  .feature-card:hover {
    transform: translateY(-5px);
  }
  
  .feature-card .icon {
    font-size: 2.5rem;
    margin-bottom: 15px;
  }
  
  .gallery {
    display: flex;
    justify-content: space-around;
    flex-wrap: wrap;
    gap: 20px;
    margin: 30px 0;
  }
  
  .gallery-item {
    flex: 1;
    min-width: 300px;
    text-align: center;
  }
  
  .gallery-item img {
    border-radius: 10px;
    box-shadow: 0 5px 15px rgba(0,0,0,0.1);
    max-width: 100%;
  }
  
  .notice {
    border-left: 4px solid;
    padding: 10px 15px;
    margin: 15px 0;
    border-radius: 0 8px 8px 0;
  }
  
  .notice-header {
    font-weight: bold;
    margin-bottom: 5px;
  }
  
  .notice {
    background-color: #e3f2fd;
    border-color: #2196f3;
  }
  
  .notice.warning {
    background-color: #fff8e1;
    border-color: #ffc107;
  }
  
  .notice.important {
    background-color: #ffebee;
    border-color: #f44336;
  }
  
  .badges {
    margin: 20px 0;
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 10px;
  }
  
  details {
    background: #f8f9fa;
    border-radius: 8px;
    padding: 10px 15px;
    margin-bottom: 10px;
    border: 1px solid #dfe1e5;
  }
  
  details summary {
    font-weight: bold;
    cursor: pointer;
  }
  
  details[open] summary {
    margin-bottom: 10px;
  }
  
  @media (max-width: 768px) {
    .features-grid {
      grid-template-columns: 1fr;
    }
  }
</style>
