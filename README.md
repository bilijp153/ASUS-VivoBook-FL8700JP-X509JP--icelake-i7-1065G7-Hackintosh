# EFI-for-ASUS-VivoBook-FL8700JP-

该EFI为华硕 vivobook FL8700JP 专用的OpenCore EFI （版本OpenCore 0.7.7）

☇

☇

☇

☇

此机型配置：


CPU：i7-1065G7


显卡：Intel lris Plus Graphics G7 + MX330


硬盘：西数的512 SSD


网卡：Intel Wireless-AC 9461

内存8GB+4GB DDR4


没有带指纹识别

☇

☇

☇

☇

EFI完善程度：较为完善（支持安装最新的Monterey12.2）


MacOS模拟机型为MacBook Pro 16.2

☇

☇

☇

☇

什么工作：

☇

蓝牙 ✔


WiFi  ✔


触摸板 ✔


键盘 ✔


Type-C ✔


USB2.0和3.0 ✔ （读卡器没有测试，应该可以）


显卡 Intel lris Plus Graphics G7 ✔ （MX330不支持MacOS）


电池 ✔（除了显示的电池容量和电池的实际情况的对不上，其他都正常）


声音和麦克风 ✔

☇

☇

☇

☇

bug：


声音存在有时开机使用无声音问题


电池显示容量和电池实际情况对不上

☇

☇

☇

☇

注意事项：


默认开启跑码模式（-v），可自行关闭


如存在安装最新系统卡还剩15分钟可先安装黑果小兵的10.15.7（19H2）然后使用系统更新升级到最新系统


如OpenCore中的Windows无法启动，可打开oc编辑器 Misc>Entries 下修改Windows所在路径或删除此项去 Misc>Security 将Scan Policy值设为0


使用的时候记得更新三码！使用的时候记得更新三码！使用的时候记得更新三码！（重要的事情说三遍）
