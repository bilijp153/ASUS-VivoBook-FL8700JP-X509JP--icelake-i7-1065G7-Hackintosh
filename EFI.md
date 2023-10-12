
 
## 📦 配置文件

该项目提供的 EFI 配置文件包含以下内容：

``` 
EFI
├── BOOT
│   └── BOOTx64.efi
└── OC
    ├── ACPI
    ├── Kexts
    ├── Drivers
    ├── Resources
    ├── Tools
    ├── config.plist
    └── Opencore.efi
```
 
其中，Boot 里的 Bootx64.efi 是笔记本 EFI 引导文件；OC 里的 ACPI 包含了 DSDT、SSDT、UEFI 变量和补丁等文件，Kexts 包含了驱动程序，Drivers 包含了 OpenCore 引导程序，Tools 包含了 OpenCore 的相关工具，Resources 包含了 Opencore 的引导界面主题（图形界面），config.plist 是 OpenCore 配置文件，Opencore.efi 是 Opencore 引导文件。
