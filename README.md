# airbook-6200u-efi

[![macOS](https://img.shields.io/badge/macOS-12.3.1-blueviolet)](https://developer.apple.com/documentation/macos-release-notes) [![OpenCore](https://img.shields.io/badge/OpenCore-0.8.0-blue)](https://github.com/acidanthera/OpenCorePkg) [![airbook](https://img.shields.io/badge/Airbook-6600U-lightgrey)](https://github.com/nabaonan/airbook-6200u-efi)

## 介绍
airbook  6代i7  支持monterey ，所有kext驱动更新最新

## 已知问题





## 基本配置

| 名称     | 型号                                                         |
| -------- | ------------------------------------------------------------ |
| cpu      | 英特尔 Core i7-6600U @ 2.60GHz 双核                          |
| 主板     | Wbin AirBook（6th/7th Generation Intel Processor Family I/O - 9D48 笔记本芯片组） |
| 内存     | 8 GB ( DDR3L 1600MHz )                                       |
| 显卡     | 英特尔 HD Graphics 520 ( 128 MB )                            |
| 无线网卡 | 瑞昱 RTL810x/8139 Family Fast Ethernet NIC                   |
| 声卡     | 英特尔 High Definition Audio 控制器                          |
| 显示器   | 夏普 SHP1423 LQ133T1JW21 ( 13.3 英寸  )                      |
| 硬盘     | (256 GB / 固态硬盘)                                          |

## 系统驱动

| 名称                         | 版本                                                         | 描述                       |
| ---------------------------- | ------------------------------------------------------------ | -------------------------- |
| AppleALC                     | ![](https://img.shields.io/badge/version-1.7.0-informational) | 声卡                       |
| HibernationFixup             | ![](https://img.shields.io/badge/version-1.4.5-informational) | 修复睡眠                   |
| Lilu                         | ![](https://img.shields.io/badge/version-1.6.0-informational) | 核心                       |
| VoodooPS2Controller          | ![](https://img.shields.io/badge/version-2.2.4-informational) | 触摸板和键盘               |
| WhateverGreen                | ![](https://img.shields.io/badge/version-1.5.8-informational) | 显卡                       |
| VirtualSMC                   | ![](https://img.shields.io/badge/version-1.2.9-informational) | 核心                       |
| SMCProcessor                 | ![](https://img.shields.io/badge/version-1.2.9-informational) | 处理器温度                 |
| SMCBatteryManager            | ![](https://img.shields.io/badge/version-1.2.9-informational) | 电池驱动                   |
| SMCSuperIO                   | ![](https://img.shields.io/badge/version-1.2.9-informational) | 温度检测                   |
| ECEnabler                    | ![](https://img.shields.io/badge/version-1.0.2-informational) | 电池驱动依赖，不用拆字节了 |
| USBPorts                     |                                                              | usb定制                    |
| RealtekCardReaderFriend.kext | ![](https://img.shields.io/badge/version-1.0.2-informational) |                            |
| RealtekCardReader.kext       | ![](https://img.shields.io/badge/version-0.9.6-informational) |                            |

## 功能完善度

- [ ] 扩展分屏显示
- [ ] 睡眠唤醒
- [ ] usb定制，usb3达到5g传输速度
- [ ] 电池电量显示（显示充电图标，显示电量百分比）
- [ ] 内置喇叭外放内放出声，插拔耳机正常
- [ ] Wifi 无线连接，蓝牙
- [ ] airdrop，接力
- [ ] cpu，硬盘温度监控，功耗监控
- [ ] cpu睿频加速
- [ ] 亮度调节（f1，f2  自行设置快捷键）
- [ ] 开盖唤醒
- [ ] 内屏hidpi（自行使用hidpi.sh）
- [ ] 摄像头正常使用
- [ ] 盒盖睡眠
- [ ] 随航（有线可以，无线不行）
- [ ] 内置sd卡识别



## 变更记录



## 效果截图

