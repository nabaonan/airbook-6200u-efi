# airbook-6200u-efi

[![macOS](https://img.shields.io/badge/macOS-10.15.7-blue)](https://developer.apple.com/documentation/macos-release-notes) [![OpenCore](https://img.shields.io/badge/OpenCore-0.7.2-blue)](https://github.com/acidanthera/OpenCorePkg) [![airbook](https://img.shields.io/badge/Airbook-6200U-lightgrey)](https://github.com/nabaonan/airbook-6200u-efi)

## 介绍

用oc0.7.2 支持macos catalina ，所有kext驱动更新最新，盒盖睡眠不好使，但是开盖唤醒可以，可以随航，如果需要bigsur请切换bigsur分支



## 基本配置

| 名称     | 型号                                         |
| -------- | -------------------------------------------- |
| cpu      | i5 6200u                                     |
| 内存     | 镁光单条16g ddr3l                            |
| 显卡     | hd520（核显）                                |
| 无线网卡 | dw1560（bcm94352z）                          |
| 声卡     | alc269vb                                     |
| 显示器   | 夏普显示器(**LQ133T1JW21**) 分辨率 2560x1440 |
| 硬盘     | 三星固态256g                                 |

## 系统驱动

| 名称                  | 版本                                                         | 描述                       |
| --------------------- | ------------------------------------------------------------ | -------------------------- |
| AirportBcrmFixup      | ![](https://img.shields.io/badge/version-1.2.3-informational) | 修复蓝牙                   |
| AppleALC              | ![](https://img.shields.io/badge/version-1.6.3-informational) | 声卡                       |
| BcrmPatchRAM3         | ![](https://img.shields.io/badge/version-2.6.0-informational) | 无线                       |
| BrcmBluetoothInjector | ![](https://img.shields.io/badge/version-2.6.0-informational) |                            |
| BrcmFirmwareData      | ![](https://img.shields.io/badge/version-2.6.0-informational) | 无线 蓝牙依赖              |
| HibernationFixup      | ![](https://img.shields.io/badge/version-1.4.2-informational) | 修复睡眠                   |
| Lilu                  | ![](https://img.shields.io/badge/version-1.5.5-informational) | 核心                       |
| VoodooPS2Controller   | ![](https://img.shields.io/badge/version-2.2.4-informational) | 触摸板和键盘               |
| WhateverGreen         | ![](https://img.shields.io/badge/version-1.5.2-informational) | 显卡                       |
| VirtualSMC            | ![](https://img.shields.io/badge/version-1.2.6-informational) | 核心                       |
| SMCProcessor          | ![](https://img.shields.io/badge/version-1.2.6-informational) | 处理器温度                 |
| SMCSuperIO            | ![](https://img.shields.io/badge/version-1.2.6-informational) | 温度检测                   |
| USBPorts              |                                                              | usb定制                    |
| ECEnabler             | ![](https://img.shields.io/badge/version-1.0.2-informational) | 电池驱动依赖，不用拆字节了 |
| SMCBatteryManager     | ![](https://img.shields.io/badge/version-1.2.6-informational) | 电池驱动                   |

## 功能完善度

- [x] 扩展分屏显示
- [x] 睡眠唤醒
- [x] usb定制，usb3达到5g传输速度
- [x] 电池电量显示（显示充电图标，显示电量百分比）
- [x] 内置喇叭外放内放出声，插拔耳机正常
- [x] Wifi 无线连接，蓝牙，airdrop，投屏显示正常
- [x] cpu，硬盘温度监控，功耗监控
- [x] cpu睿频加速
- [x] 亮度调节（f1，f2  自行设置快捷键）
- [x] 开盖唤醒
- [x] 内屏hidpi（自行使用hidpi.sh）
- [x] 摄像头正常使用
- [ ] 盒盖睡眠，不明原因，在bigsur支持，怀疑有可能系统原因
- [x] 随航
- [ ] 内置sd卡识别



## 变更记录

- 2.3.1

  - 更换电池驱动

- **2.3.0**

  - 支持catalina

  

  


## 效果截图

### wifi：

稳定链接，中途不自动中断，睡眠唤醒不中断

![](./assets/17.jpg)



![](./assets/4.jpg)

蓝牙：经测试可以实现接力和隔空投送

![](./assets/5.jpg)



Geekbench-5 跑分

![](./assets/15.jpg)



![](./assets/11.jpg)

![](./assets/16.jpg)



