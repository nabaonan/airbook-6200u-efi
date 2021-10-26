# airbook-6200u-efi

[![macOS](https://img.shields.io/badge/macOS-11.6.1-orange)](https://developer.apple.com/documentation/macos-release-notes) [![OpenCore](https://img.shields.io/badge/OpenCore-0.7.4-blue)](https://github.com/acidanthera/OpenCorePkg) [![airbook](https://img.shields.io/badge/Airbook-6200U-lightgrey)](https://github.com/nabaonan/airbook-6200u-efi)

## 介绍
airbook支持macos bigsur ，所有kext驱动更新最新，经过测试睡眠完美，随航可用

## 效果预览
**b站**：  [效果预览](https://www.bilibili.com/video/BV183411r77B)

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

| 名称                  | 版本                                                         | 描述                       |
| --------------------- | ------------------------------------------------------------ | -------------------------- |
| AirportBcrmFixup      | ![](https://img.shields.io/badge/version-2.1.3-informational) | 修复蓝牙                   |
| AppleALC              | ![](https://img.shields.io/badge/version-1.6.5-informational) | 声卡                       |
| BcrmPatchRAM3         | ![](https://img.shields.io/badge/version-2.6.0-informational) | 无线                       |
| BrcmBluetoothInjector | ![](https://img.shields.io/badge/version-2.6.0-informational) | 蓝牙                       |
| BrcmFirmwareData      | ![](https://img.shields.io/badge/version-2.6.0-informational) | 无线 蓝牙依赖              |
| HibernationFixup      | ![](https://img.shields.io/badge/version-1.4.4-informational) | 修复睡眠                   |
| Lilu                  | ![](https://img.shields.io/badge/version-1.5.6-informational) | 核心                       |
| VoodooPS2Controller   | ![](https://img.shields.io/badge/version-2.2.6-informational) | 触摸板和键盘               |
| WhateverGreen         | ![](https://img.shields.io/badge/version-1.5.4-informational) | 显卡                       |
| VirtualSMC            | ![](https://img.shields.io/badge/version-1.2.7-informational) | 核心                       |
| SMCProcessor          | ![](https://img.shields.io/badge/version-1.2.7-informational) | 处理器温度                 |
| SMCBatteryManager     | ![](https://img.shields.io/badge/version-1.2.7-informational) | 电池驱动                   |
| SMCSuperIO            | ![](https://img.shields.io/badge/version-1.2.7-informational) | 温度检测                   |
| ECEnabler             | ![](https://img.shields.io/badge/version-1.0.2-informational) | 电池驱动依赖，不用拆字节了 |
| USBPorts              |                                                              | usb定制                    |

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
- [x] 盒盖睡眠
- [x] 随航
- [ ] 内置sd卡识别



## 变更记录

- 3.1.0
  
  - 升级oc到0.7.4   升级所有驱动到最新版

- 3.0.5
  
  - 更换smc电池驱动，提升性能

- **3.0.3**
  
  - 修复睡眠一段时间自动唤醒的问题  禁用appleRTC
  - 清理无用的驱动
  
- **3.0.1**
  
  - 支持bigsur11.5.1，oc升级到0.7.2，驱动所有硬件
  - 修复睡眠就唤醒的问题
  - 解决wifi驱动冲突导致启动缓慢的问题
  
  

## 效果截图

![7](./assets/11.jpg)

### 系统

![7](./assets/12.jpg)

### oc版本

![9](./assets/9.jpg)

### 电池状态：

- 弱电：低于10%电池变红
- 充电：插电出闪电
- 拔掉电源：闪电消失
- 满格：电池进度满格加闪电标识

![1](./assets/1.jpg)

![2](./assets/2.jpg)

![3](./assets/3.jpg)

![4](./assets/4.jpg)



### 显卡硬件解码

![5](./assets/5.jpg)

### Geekbench5跑分

![6](./assets/10.jpg)ß

### USB定制

![8](./assets/8.jpg)
