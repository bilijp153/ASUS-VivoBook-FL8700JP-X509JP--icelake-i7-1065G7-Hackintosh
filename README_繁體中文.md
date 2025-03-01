<div align="center">
  <img src="https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/hackintosh2.png" width="180" alt="Hackintosh Logo">
  <h1>華碩 VivoBook FL8700JP 黑蘋果</h1>
  <p>讓 Windows 筆記本成功運行 macOS</p>
</div>

---

## 📌 快速導航([简体中文](README.md))([English](README_en.md))

|[🌟 專案亮點](#-專案亮點) |[🚩 專案概覽](#-專案概覽) |[📸 實機展示](#-實機展示)|[💻 硬體相容性](#-硬體相容性) |
|------------------|------------------|----------------------------|----------------------------|
|[🖥️ 系統支援](#️-系統支援)|[⚙️ 安裝指南](#️-安裝指南) |[🛠️ 進階配置](#️-進階配置) |[❓ 常見問題](#-常見問題) |
|[⚠️ 注意事項](#️-注意事項)|[🌟 貢獻與支持](#️-貢獻與支持) |[📮 問題回饋](#-問題回饋) |[🙏 致謝](#-致謝) |
---

## 🌟 專案亮點
- ✅ **完美相容**：支援 macOS Catalina ~ Sequoia 全版本  
- 🖥 **硬體優化**：核顯/聲卡/網卡深度適配  
- 🚀 **效能調校**：原生 CPU 電源管理 + 智能睿頻  
- 🔋 **電源優化**：原生電源管理 + 休眠支援  
- 🛠 **持續維護**：定期更新 EFI 與問題修復  

---

## 🚩 專案概覽
### 配置文件結構
```bash
EFI/                         # EFI 引導文件夾
├── BOOT/                    # Boot 引導文件夾
│   └── BOOTx64.efi          # UEFI 引導文件
└── OC/                      # OpenCore 引導文件夾
    ├── ACPI/                # DSDT/SSDT 補丁
    ├── Kexts/               # 核心驅動
    ├── Drivers/             # OpenCore 驅動
    ├── config.plist         # 主配置文件
    └── ...                  # 其他資源文件
└── ...                      # 其他系統引導文件夾


```
### 注意事項
- **僅適配 ASUS FL8700JP (X509JP) 機型**，其他設備不保證相容性。  
- **不包含 macOS 安裝檔**，需自行準備安裝文件。  
- 安裝前請備份資料，**操作風險自負**。  
- 本專案遵循 [MIT 許可證](License)，禁止商業用途。  

### [↩️ 返回快速導航](#-快速導航简体中文English)

---

## 📸 實機展示
<div align="center">
  <img src="https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/computer1.png" width="45%">
  <img src="https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-icelake-1065G7-Hackintosh/blob/main/机型效果图/computer2.png" width="45%">
</div>

---

## 💻 硬體相容性
| 組件         | 型號                      | 狀態     | 備註                     |
|--------------|---------------------------|----------|--------------------------|
| **處理器**   | Intel i7-1065G7           | ✅ 正常工作 | Ice Lake 架構           |
| **核顯**     | Intel Iris Plus G7        | ⚠️ 部分支援 | 不支援 HDMI 顯示        |
| **獨顯**     | NVIDIA MX330              | ❌ 未支援  | 已透過 SSDT 屏蔽        |
| **聲卡**     | Realtek ALC256            | ✅ 正常工作 | 支援外設自動切換        |
| **無線網卡** | Intel Wireless-AC 9461    | ✅ 部分支援 | 不支援 AirDrop/AirPlay  |
| **觸控板**   | ELAN1200                  | ⚠️ 部分支援 | 偶發無回應（需重啟）    |
| **Type-C**   | -                         | ⚠️ 部分支援 | 不支援 DP 顯示與 Thunderbolt |

---

## 🖥️ 系統支援
| 系統版本       | 相容性 | 最低支援版本        |
|----------------|--------|---------------------|
| macOS Catalina | ✅      | 10.15.4            |
| Big Sur        | ✅      | 11.0               |
| Monterey       | ✅      | 12.0               |
| Ventura        | ✅      | 13.0               |
| Sonoma         | ✅      | 14.0               |
| Sequoia        | ✅      | 15.0               |

### [↩️ 返回快速導航](#-快速導航简体中文English)

---

## ⚙️ 安裝指南
### 1. BIOS 設定

- **Secure Boot**：關閉  
- **Fast Boot**：關閉  
- **DVMT Pre-Allocated**：64M  

### 2. 安裝步驟

1. 下載 macOS 安裝檔 ➔ 推薦使用 [黑果小兵的部落閣](https://blog.daliansky.net/)  
2. 製作 macOS 安裝隨身碟 ➔ 使用 [BalenaEtcher](https://www.balena.io/etcher/)  
3. [**下載**](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/releases) EFI 文件 ➔ 替換隨身碟中的 EFI 文件夾  
4. 設定隨身碟為第一啟動裝置  
5. 透過 OpenCore 啟動 ➔ 選擇「Install macOS XXX」  
6. 多次重啟直至安裝完成  
7. 將 EFI 遷移至本機 SSD 並移除隨身碟  

### 3. SMBIOS 設定

1. 使用 **OpenCore Configurator** 或 [**OCAuxiliaryTools**](https://github.com/ic005k/OCAuxiliaryTools) 將 **SystemProductName** 設為 **MacBookAir9,1** 或 **MacBookPro16,2**（推薦：MacBookAir9,1）  
2. 生成有效 **SystemSerialNumber** 並於 Apple [檢查保固頁面](https://checkcoverage.apple.com/)驗證  
3. 儲存**config**文件後重啟  

---

## 🛠️ 進階配置

💻 BootCamp 雙系統配置

1. 透過 [**brigadier**](https://github.com/corpnewt/brigadier) 下載所需文件  
2. 執行腳本並按提示生成 **dmg**  
3. 將 BootCamp 文件夾複製至 Windows 分割區  
4. 在 `config.plist` 中將 **updateSMBIOSMod** 設為 **Create** 並重啟  
5. 在 OpenCore 中選擇 **Windows** 啟動  
6. 透過 `Setup.exe` 安裝 BootCamp 驅動  
7. 重啟後將 **updateSMBIOSMod** 改回 **Custom**  

### [↩️ 返回快速導航](#-快速導航简体中文English)

---

## ❓ 常見問題
<details>
  <summary><b>Q: 如何關閉開機「咚」聲？</b></summary>
  前往「系統設定」➔「聲音」➔ 關閉「開機時播放聲音」。
</details>

<details>
  <summary><b>Q: 觸控板偶爾無回應？</b></summary>
  需重啟或透過睡眠喚醒恢復，此為 ELAN1200 驅動已知問題。
</details>

<details>
  <summary><b>Q: 如何切換預設系統？</b></summary>
  在 OpenCore 介面按 Ctrl+Enter，或於「系統設定」➔「啟動磁碟」設定。
</details>

---

## ⚠️ 注意事項
1. 初次設定時請**跳過 Apple ID 登入**，後續於「系統設定」中補登。  
2. 務必生成**唯一 SMBIOS** 並確保序號於 Apple 網站顯示「無效」。  
3. 完成後方可嘗試註冊並登入 Apple ID。  

---

## 🌟 貢獻與支持
| 角色           | 貢獻者                |
|----------------|-----------------------|
| 維護者         | [极光呆呆脑](https://github.com/bilijp153) |
| 測試者         | [若涵](https://github.com/catlingyun)     |

---

## 📮 問題回饋
提交至 [GitHub Issues](https://github.com/bilijp153/ASUS-VivoBook-FL8700JP-Hackintosh/issues) 或聯絡：  
📧 **電子郵件**: 1551656605@qq.com  

<a href="https://space.bilibili.com/329351708">
    <img src="https://img.shields.io/badge/嗶哩嗶哩-极光呆呆脑-FF69B4?logo=bilibili" alt="Bilibili">
  </a>
  <a href="https://weibo.com/u/5264002671">
    <img src="https://img.shields.io/badge/微博-草莓小极光-1DA1F2?logo=sinaweibo" alt="Weibo">
  </a>
  <a href="https://qm.qq.com/cgi-bin/qm/qr?k=B2Omg5IKCGWoMNXgMIPmA_AJqEMnMCUb&noverify=0&personal_qrcode_source=3">
    <img src="https://img.shields.io/badge/QQ-极光呆呆脑-26A5E4?logo=QQ" alt="QQ">
  </a>

---

## 🙏 致謝
- [OpenCore 官方指南](https://dortania.github.io/OpenCore-Install-Guide/)  
- [Acidanthera](https://github.com/acidanthera) 驅動開發團隊
- [laobamac](https://github.com/laobamac) OCLP-Mod開發者 

### [↩️ 返回快速導航](#-快速導航简体中文English)

---

<div align="center">
本專案基於 [MIT 許可證](License) 開源。  

© 2021-2024 Aurora极光呆呆脑。保留所有權利。
</div>
[file content end]
```
