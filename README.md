# airbook-6200u-efi

[![macOS](https://img.shields.io/badge/macOS-13.4-yellow)](https://github.com/nabaonan/airbook-6200u-efi) [![OpenCore](https://img.shields.io/badge/OpenCore-0.9.2-blue)](https://github.com/nabaonan/airbook-6200u-efi) [![airbook](https://img.shields.io/badge/Airbook-6200U-lightgrey)](https://github.com/nabaonan/airbook-6200u-efi)

## 介绍
airbook支持ventura ，所有kext驱动更新最新

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=nabaonan/airbook-6200u-efi&type=Date)](https://star-history.com/#nabaonan/airbook-6200u-efi&Date)


## 已知问题

电量低于30会黑屏死机

## 基本配置

| 名称     | 型号                                         |
| -------- | -------------------------------------------- |
| cpu      | i5 6200u                                     |
| 内存     | 镁光单条16g ddr3l                            |
| 显卡     | hd520（核显）                                |
| 无线网卡 | dw1560（bcm94352z）                          |
| 声卡     | alc269vb                                     |
| 显示器   | 夏普显示器(**LQ133T1JW21**) 分辨率 2560x1440 |
| 硬盘     | 朗科120g固态                                 |

## 系统驱动

| 名称                         | 版本                                                         | 描述                         |
| ---------------------------- | ------------------------------------------------------------ | ---------------------------- |
| AirportBcrmFixup             | [![](https://img.shields.io/badge/version-2.1.6-informational)](https://github.com/nabaonan/airbook-6200u-efi) | wifi                         |
| AppleALC                     | [![](https://img.shields.io/badge/version-1.7.8-informational)](https://github.com/nabaonan/airbook-6200u-efi) | 声卡                         |
| BcrmPatchRAM3                | [![](https://img.shields.io/badge/version-2.6.4-informational)](https://github.com/nabaonan/airbook-6200u-efi) | 蓝牙                         |
| BlueToolFixup                | [![](https://img.shields.io/badge/version-2.6.4-informational)](https://github.com/nabaonan/airbook-6200u-efi) | 蓝牙                         |
| BrcmFirmwareData             | [![](https://img.shields.io/badge/version-2.6.4-informational)](https://github.com/nabaonan/airbook-6200u-efi) | 蓝牙                         |
| HibernationFixup             | [![](https://img.shields.io/badge/version-1.4.7-informational)](https://github.com/nabaonan/airbook-6200u-efi) | 修复睡眠                     |
| Lilu                         | [![](https://img.shields.io/badge/version-1.6.3-informational)](https://github.com/nabaonan/airbook-6200u-efi) | 核心                         |
| VoodooPS2Controller          | [![](https://img.shields.io/badge/version-2.2.4-informational)](https://github.com/nabaonan/airbook-6200u-efi) | 触摸板和键盘                 |
| WhateverGreen                | [![](https://img.shields.io/badge/version-1.6.4-informational)](https://github.com/nabaonan/airbook-6200u-efi) | 显卡                         |
| VirtualSMC                   | [![](https://img.shields.io/badge/version-1.3.0-informational)](https://github.com/nabaonan/airbook-6200u-efi) | 核心                         |
| SMCProcessor                 | [![](https://img.shields.io/badge/version-1.3.0-informational)](https://github.com/nabaonan/airbook-6200u-efi) | 处理器温度                   |
| SMCBatteryManager            | [![](https://img.shields.io/badge/version-1.3.0-informational)](https://github.com/nabaonan/airbook-6200u-efi) | 电池驱动（不用了）           |
| ACPIBatteryManage            | [![](https://img.shields.io/badge/version-1.81.4-informational)](https://github.com/nabaonan/airbook-6200u-efi) | 旧版电池驱动（结合ssdt补丁） |
| SMCSuperIO                   | [![](https://img.shields.io/badge/version-1.3.0-informational)](https://github.com/nabaonan/airbook-6200u-efi) | 温度检测                     |
| ECEnabler                    | [![](https://img.shields.io/badge/version-1.0.3-informational)](https://github.com/nabaonan/airbook-6200u-efi) | 电池驱动依赖，不用拆字节了   |
| USBPorts                     |                                                              | usb定制                      |
| RealtekCardReaderFriend.kext | [![](https://img.shields.io/badge/version-1.0.4-informational)](https://github.com/nabaonan/airbook-6200u-efi) |                              |
| RealtekCardReader.kext       | [![](https://img.shields.io/badge/version-0.9.7-informational)](https://github.com/nabaonan/airbook-6200u-efi) |                              |

## 功能完善度

- [x] 扩展分屏显示
- [x] 睡眠唤醒
- [x] usb定制，usb3达到5g传输速度
- [x] 电池电量显示（显示充电图标，显示电量百分比）
- [x] 内置喇叭外放内放出声，插拔耳机正常
- [x] Wifi 无线连接，蓝牙
- [x] airdrop，接力
- [x] cpu，硬盘温度监控，功耗监控
- [x] cpu睿频加速
- [x] 亮度调节（f1，f2  自行设置快捷键）
- [x] 开盖唤醒
- [x] 内屏hidpi（自行使用hidpi.sh）
- [x] 摄像头正常使用
- [x] 盒盖睡眠
- [ ] 随航（有线可以，无线不行）
- [x] 内置sd卡识别



## 变更记录



- 5.12 再次尝试使用acpi 电池驱动  升级oc0.9.2

- 5.11 重新定制usb

- 恢复使用smc驱动，调整加载顺序

- 5.10
  - 改用acpibattery驱动 ，结合ssdt补丁 完美解决电池显示和盒盖睡眠，黑屏死机问题

- 5.9
  - 解决hidpi开启闪屏问题，更新weg驱动1.6.4

- 5.8.1
  - 定制usb 解决丢失sd卡不识别
- 5.8
  - 更新0.8.6，更新sd卡驱动，解决睡眠唤醒掉sd卡的问题
- 5.6
  - 更新085
- 5.5
  - 更新驱动和oc084
- 5.4
  - 解决外接显示紫色屏幕的问题
- 5.3
  - 更新hackintosh主题
  - 增加启动画面截屏
  - 修改睡眠唤醒wifi断开问题，更新驱动
- 5.2
  - 基本完美，完善驱动和机型


## 效果截图



### 系统

![1](./assets/1.jpg)

### 美化启动界面

![6](./assets/6.png)

### oc版本

![1](./assets/2.jpg)



### Geekbench6 跑分

![3](./assets/7.png)

### Geekbench5跑分

![3](./assets/3.jpg)



### 视频解码

![4](./assets/4.jpg)

### sd 读卡器测速

![5](./assets/5.png)

## bios相关配置参考：

![](./assets/bios/IMG_0149.jpeg)

![](./assets/bios/IMG_0150.jpeg)

![](./assets/bios/IMG_0151.jpeg)



![](./assets/bios/IMG_0152.jpeg)

![](./assets/bios/IMG_0153.jpeg)

![](./assets/bios/IMG_0154.jpeg)



![](./assets/bios/IMG_0155.jpeg)
