```markdown
<div align="center">
  <img src="https://placehold.co/600x200/3b82f6/white?text=ASUS+FL8700JP+Hackintosh" style="width: 80%; max-width: 800px; border-radius: 12px; box-shadow: 0 4px 12px rgba(0,0,0,0.1);">
  
  <h1>🍎 ASUS VivoBook FL8700JP Hackintosh</h1>

  <div style="margin: 24px 0">
    <a href="https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/releases">
      <img alt="Latest Release" src="https://img.shields.io/github/v/release/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh?color=3b82f6&label=Latest&style=for-the-badge">
    </a>
    <a href="https://github.com/acidanthera/OpenCorePkg">
      <img alt="OpenCore 0.9.7+" src="https://img.shields.io/badge/OpenCore-0.9.7+-3b82f6?style=for-the-badge&logo=apple">
    </a>
  </div>
</div>

---

## 🌟 核心特性
<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 16px; margin: 24px 0">

```markdown
<div style="background: #f8f9fa; padding: 20px; border-radius: 8px">
  <h3>✅ 完美兼容</h3>
  <ul>
    <li>macOS Ventura/Sonoma</li>
    <li>Intel Iris Plus 核显加速</li>
    <li>WiFi/蓝牙双模连接</li>
    <li>Type-C 扩展功能</li>
  </ul>
</div>

<div style="background: #f8f9fa; padding: 20px; border-radius: 8px">
  <h3>⚡ 性能表现</h3>
  <ul>
    <li>Geekbench 5 单核：1250+</li>
    <li>Geekbench 5 多核：4200+</li>
    <li>4K 视频硬解支持</li>
    <li>Apple Silicon 级响应速度</li>
  </ul>
</div>
</div>

---

## 📋 硬件兼容性
<table>
  <tr>
    <th>组件</th>
    <th>状态</th>
    <th>备注</th>
  </tr>
  <tr>
    <td>Intel i7-1065G7</td>
    <td>✅ 完美</td>
    <td>睿频/节能全支持</td>
  </tr>
  <tr>
    <td>Iris Plus G7</td>
    <td>✅ 完美</td>
    <td>Metal 3 加速支持</td>
  </tr>
  <tr>
    <td>Realtek ALC256</td>
    <td>✅ 完美</td>
    <td>杜比音效支持</td>
  </tr>
  <tr>
    <td>Intel AC9461</td>
    <td>⚠️ 部分</td>
    <td>不支持隔空投送</td>
  </tr>
</table>

---

## 🛠 快速开始
```bash
# 安装准备
1. 下载最新版 EFI
2. 使用 ProperTree 配置 SMBIOS
3. 修改 BIOS 设置：
   - Secure Boot: Disabled
   - DVMT: 64MB
   - SATA Mode: AHCI
4. 使用 OCAT 更新驱动
```

---

## 📸 实机预览
<div style="columns: 2; gap: 16px; margin: 24px 0">
  <img src="https://placehold.co/400x250/3b82f6/white?text=系统信息" style="width: 100%; border-radius: 8px">
  <img src="https://placehold.co/400x250/3b82f6/white?text=关于本机" style="width: 100%; border-radius: 8px">
  <img src="https://placehold.co/400x250/3b82f6/white?text=硬件加速" style="width: 100%; border-radius: 8px">
  <img src="https://placehold.co/400x250/3b82f6/white?text=多屏扩展" style="width: 100%; border-radius: 8px">
</div>

---

## 📌 注意事项
<details>
<summary>点击查看重要提示</summary>

1. **BIOS 版本要求**：需升级至 2022 年后的版本
2. **睡眠设置**：建议设置 `sudo pmset -a standbydelay 300`
3. **Windows 双系统**：需关闭 SpoofVendor 功能
4. **触控板修复**：ELAN1200 需定期重启服务
</details>

---

<div align="center" style="margin-top: 48px">
  <a href="https://github.com/bilijp153">
    <img src="https://img.shields.io/badge/维护者-@Aurora极光-3b82f6?style=flat-square">
  </a>
  <a href="https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/issues">
    <img src="https://img.shields.io/github/issues-raw/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh?color=3b82f6&style=flat-square">
  </a>
  <p>📧 技术支持：<a href="mailto:1551656605@qq.com">1551656605@qq.com</a></p>
  <sub>© 2021-2024 Aurora极光 | MIT Licensed</sub>
</div>
```