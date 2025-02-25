# 🍎 ASUS VivoBook FL8700JP/X509JP Hackintosh

✨ **The most elegant Hackintosh solution for ASUS VivoBook FL8700JP/X509JP (Ice Lake i7-1065G7)**  
![Hackintosh](https://img.shields.io/badge/MacOS-Ventura%2013.6-292e33?logo=apple&logoColor=white)
![Platform](https://img.shields.io/badge/Platform-Intel%20Ice%20Lake-blueviolet)
![OpenCore](https://img.shields.io/badge/OpenCore-0.9.6-important)

<p align="center">
  <img src="https://placehold.co/600x400/png?text=Hackintosh+Showcase" alt="Demo" width="60%" style="border-radius: 12px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);">
</p>

## 🌟 特性概览
✅ **完美兼容组件**  
![Wi-Fi](https://img.shields.io/badge/Wi--Fi-BCM94360NG-yellowgreen) 
![Bluetooth](https://img.shields.io/badge/Bluetooth-5.0-9cf) 
![Audio](https://img.shields.io/badge/Audio-ALC256-green)  

⚠️ **部分工作组件**  
![Touchpad](https://img.shields.io/badge/Touchpad-80%25%20Gestures-orange) 
![HDMI](https://img.shields.io/badge/HDMI-No%20Audio-red)

## 🖥 硬件配置

| **组件**       | **型号**                          | **状态** |
|----------------|-----------------------------------|----------|
| **处理器**     | Intel Core i7-1065G7 (Ice Lake)  | ✅        |
| **内存**       | 16GB DDR4 3200MHz                | ✅        |
| **固态硬盘**   | Samsung PM981a 512GB             | ⚠️ [^1]  |
| **无线网卡**   | BCM94360NG                       | ✅        |
| **显示屏**     | 17.3" FHD IPS 60Hz               | ✅        |

[^1]: 需使用NVMeFix驱动

## 🛠 安装指南
### 📦 准备工作
1. 准备16GB以上U盘
2. 下载 [**macOS Ventura镜像**](https://example.com)
3. 使用 [**BalenaEtcher**](https://www.balena.io/etcher/) 制作启动盘

### ⚡ EFI配置
```bash
git clone https://github.com/your-repo/EFI-X509JP.git
cp -R EFI-X509JP/OC /Volumes/EFI/EFI/