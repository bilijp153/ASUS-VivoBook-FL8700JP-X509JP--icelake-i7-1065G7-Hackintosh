 
<div align="center">
  <img src="https://img.shields.io/github/stars/bilijp153/ASUS-VivoBook-FL8700JP-X509JP--icelake-i7-1065G7-Hackintosh?style=for-the-badge&logo=appveyor">
  <img src="https://img.shields.io/badge/macOS-Monterey-2996cc?style=for-the-badge&logo=apple">
  <img src="https://img.shields.io/github/license/bilijp153/ASUS-VivoBook-FL8700JP-X509JP--icelake-i7-1065G7-Hackintosh?style=for-the-badge">
</div>

<h1 align="center">🍎 华硕VivoBook FL8700JP Hackintosh 指南</h1>

<div align="center">
📱📊🖥 三端自适应 | 🌈 Material Design风格 | 📌 交互式目录
</div>

---

## 📑 目录导航
[✨ 项目简介](#-项目简介) | [💻 硬件配置](#-硬件配置) | [✅ 正常工作](#-正常工作) | [⚠️ 已知问题](#️-已知问题) | [⚙️ BIOS设置](#️-bios设置) | [📥 安装指南](#-安装指南)

---

## ✨ 项目简介
适用于**ASUS VivoBook FL8700JP/X509JP**的Hackintosh配置文件，基于：
- OpenCore 0.9.5
- macOS Monterey 12.6.6
- 特别适配i7-1065G7 (Ice Lake)平台

> ⚠️ 注意：本EFI仅限学习交流，不得用于商业用途

---

## 💻 硬件配置表

| 组件类别       | 具体配置                          |
|----------------|-----------------------------------|
| **处理器**     | Intel Core i7-1065G7 (10nm Ice Lake) |
| **内存**       | 16GB DDR4 3200MHz (8GB x2)       |
| **存储**       | WD SN550 1TB NVMe SSD            |
| **显示屏**     | 17.3" FHD IPS 60Hz               |
| **无线网卡**   | Intel AX201NGW                   |
| **声卡**       | Realtek ALC256                   |

<details>
<summary>📸 点击查看硬件架构图</summary>
<img src="your_screenshot_url_here" width="100%" alt="硬件架构示意图">
</details>

---

## ✅ 正常工作功能
<table>
  <tr>
    <th>功能模块</th>
    <th>支持状态</th>
    <th>备注</th>
  </tr>
  <tr>
    <td>CPU电源管理</td>
    <td>⭕ 完整支持</td>
    <td>支持变频/睿频</td>
  </tr>
  <tr>
    <td>显卡加速</td>
    <td>⭕ 完整支持</td>
    <td>Iris Plus 64EU驱动正常</td>
  </tr>
  <!-- 其他表格行保持原内容 -->
</table>

---

## ⚙️ BIOS设置指南
```markdown
1. 开机按 `F2` 进入BIOS
2. 关键设置项：
   - ❌ Disable Secure Boot
   - ✅ Enable VT-d
   - ⚡ 调整DVMT为64M
3. 保存设置并重启
 