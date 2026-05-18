# aic8800d80-driver
[中文](#中文) | [English](#English)

### 中文
aic8800d80无线网卡驱动（包含了dkms模块与固件）。

此驱动仅在本人购买的产品上做了测试，商品型号为水星UX9H免驱版。使用同样芯片的产品应该有效。

设备参数
```
# 安装驱动以前
$ lsusb
ID a69c:5721 aicsemi Aic MSC
# 安装驱动以后
$ lsusb
ID 2357:014b TP-Link AIC 8800D80
usb-devices
...
P:  Vendor=2357 ProdID=014b Rev=01.00
S:  Manufacturer=AICSemi
S:  Product=AIC 8800D80
S:  SerialNumber=20220103
...

```

安装方法：

Release页面下载aic8800d80-driver-dkms.deb与aic8800d80-driver-firmware.deb，用apt包管理器安装即可。

### English
(this section is translated by AI)

aic8800d80 Wi-Fi Adapter Driver (including DKMS rules and firmware)

This driver package has only been tested on my own device (Mercury UX9H USB Wi-Fi adapter), but it should also work for any other devices using the same chipset.

Some parameters about my device
```
# before installation
$ lsusb
ID a69c:5721 aicsemi Aic MSC
# after installation
$ lsusb
ID 2357:014b TP-Link AIC 8800D80
usb-devices
...
P:  Vendor=2357 ProdID=014b Rev=01.00
S:  Manufacturer=AICSemi
S:  Product=AIC 8800D80
S:  SerialNumber=20220103
...

```

how to install:

Download aic8800d80-driver-dkms.deb and aic8800d80-driver-firmware.deb on release page, then install them by apt package manager.

# 免责声明 | Disclaimer

本仓库中的驱动源码来自水星客服提供的 deb 包，仅重组了文件结构以适应DKMS模块。本仓库并不负责运行中可能产生的任何问题。

**由于原始包的许可证信息不明确，本仓库仅作为技术参考和教育用途。**

如果你是这个驱动的版权所有者，并且认为本仓库侵犯了您的权利，请联系我，我会立即处理。

**使用者请注意：**
- 请自行确认在你的地区使用/分发此驱动的合法性
- 建议从官方渠道获取驱动

---

The driver source code in this repository was extracted from a .deb package provided by Mercury Customer Support. The file structure has merely been reorganized to support the DKMS module. This repository is provided as-is, and I am not responsible for any issues that may arise during its operation.

**Due to unclear licensing information in the original package, this repository is intended for technical reference and educational purposes only.**

If you are the copyright holder of this driver and believe that this repository infringes upon your rights, please contact me and I will address it immediately.

**Notice to Users:**
- Please verify the legality of using/distributing this driver in your region on your own.
- It is highly recommended to obtain drivers from official channels.
