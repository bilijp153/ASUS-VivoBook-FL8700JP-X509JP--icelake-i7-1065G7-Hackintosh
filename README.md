<div align="center">
  <img src="https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/hackintosh2.png" width="180" alt="Hackintosh Logo">
  <h1> 华硕 VivoBook FL8700JP 黑苹果项目</h1>
  
  [![GitHub Stars](https://img.shields.io/github/stars/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh?color=ff69b4&style=for-the-badge)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/stargazers)
  [![Latest Release](https://img.shields.io/github/v/release/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh?style=for-the-badge&logo=apple)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/releases)
  [![License](https://img.shields.io/github/license/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh?style=for-the-badge)](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/LICENSE)

  <img src="https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/简体1.png" width="600" alt="Demo">
</div>

---

## 📌 快速导航
| [✨ 特性](#-特性) | [📦 硬件兼容性](#-硬件兼容性) | [⚙️ 安装指南](#️-安装指南) | [❓ 常见问题](#-常见问题) |
|------------------|----------------------------|-------------------------|-------------------------|

---

## ✨ 特性
- ✅ **完美驱动**：核显、声卡、WiFi/蓝牙、触控板、睡眠唤醒  
- 🚫 **已知限制**：独显 MX330 不可用，HDMI 无输出  
- 🌟 **系统支持**：Catalina → Sonoma（推荐 Monterey/Ventura）  
- 📱 **多端优化**：响应式布局，适配手机/平板/电脑  

---

## 📦 硬件兼容性
<table>
  <tr>
    <th>组件</th>
    <th>状态</th>
    <th>备注</th>
  </tr>
  <tr>
    <td>Intel Iris Plus Graphics</td>
    <td>✅ 完美</td>
    <td>支持 4K 输出</td>
  </tr>
  <tr>
    <td>Realtek ALC256 声卡</td>
    <td>✅ 完美</td>
    <td>支持耳机自动切换</td>
  </tr>
  <tr>
    <td>Intel AC9461 无线网卡</td>
    <td>✅ 基本</td>
    <td>不支持隔空投送</td>
  </tr>
  <tr>
    <td>ELAN1200 触控板</td>
    <td>⚠️ 偶发卡顿</td>
    <td>需重启恢复</td>
  </tr>
</table>

---

## ⚙️ 安装指南
### 准备工作
1. **BIOS 设置**  
   - 关闭 `Secure Boot` 和 `Fast Boot`  
   - 硬盘模式设为 `AHCI`  
   - 调整 DVMT 至 `64M`

2. **下载工具**  
   - [EFI 文件](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/releases)  
   - [Etcher](https://www.balena.io/etcher/)（制作启动盘）

### 安装步骤
```bash
1. 将 EFI 复制到 U 盘 EFI 分区
2. 从 U 盘启动进入 OpenCore
3. 选择 "Install macOS" 完成安装
4. 迁移 EFI 到系统硬盘
```

---

## 🛠️ 高级配置
<details>
<summary>📱 SMBIOS 三码生成（点击展开）</summary>

1. 使用 **OpenCore Configurator** 生成唯一三码  
2. 选择机型：`MacBook Pro 16,2` 或 `MacBook Air 9,1`  
3. 验证序列号状态需显示 **"无效"**  
4. 修改 `config.plist` 注入三码
</details>

<details>
<summary>💻 BootCamp 双系统配置</summary>

```bash
# 使用 brigadier 下载驱动
python brigadier -m <Mac机型ID>
# 将驱动文件复制到 Windows 系统盘
# 修改 SMBIOS 欺骗为 Mac 机型
# 安装完成后恢复原始配置
```
</details>

---

## ❓ 常见问题
**Q：HDMI 为何无法使用？**  
A：Intel Ice Lake 处理器已移除 HDMI 原生支持。

**Q：触控板突然失灵？**  
A：ELAN1200 已知偶发问题，尝试重启或睡眠唤醒。

**Q：如何设置默认启动项？**  
A：在 OpenCore 界面按 `Ctrl+Enter`，或在系统设置中选择启动磁盘。

---

## 🌟 贡献与支持
| 角色 | 贡献者 | 链接 |
|------|--------|------|
| 维护 | Aurora极光 | [GitHub](https://github.com/bilijp153) |
| 测试 | 若涵 | [GitHub](https://github.com/catlingyun) |

---

<div align="center">
  📮 问题反馈：<a href="https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/issues">GitHub Issues</a>  
  
  © 2021-2024 Aurora极光 | MIT License
</div>
