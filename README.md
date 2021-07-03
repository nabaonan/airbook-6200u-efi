# airbook-6200u-efi

#### 介绍
基于oc7.0定制，已经测试过，满足日常使用需求，就是盒盖睡眠不管用（怀疑没有定制原生电源管理）

理论支持macos最新版，但是需要替换蓝牙的kext，自行查询资料，这版就是停在10.14.6养老了

#### 基本配置

cpu：i5 6200u

内存：镁光单条16g ddr3l

显卡：hd520（核显）

无线网卡：dw1560（bcm94352z）

声卡：alc269vb

显示：lg的显示器(**LQ133T1JW21**) 2560x1440

硬盘：三星的固态256g(SAMSUNG MZMTE256HMHP-000L1)

系统：osx 10.14.6

#### 功能完善度

- [x] 扩展分屏显示（没有测试外接4k，只测试外接1080p）
- [x] 睡眠唤醒
- [x] usb定制，usb3达到5g传输速度
- [x] 电池电量显示（显示充电图标，显示电量百分比）
- [x] 内置喇叭外放内放出声，插拔耳机正常
- [x] Wifi 无线连接，蓝牙，airdrop，投屏显示正常（睡眠唤醒不断）
- [ ] cpu，硬盘温度监控，功耗监控
- [ ] cpu睿频加速，自定义最低频率800，最高频率2700[现在睿频是最低1.3最高2.8，档位不够多]
- [x] 亮度调节（f1，f2   16档调节）
- [ ] 开盖唤醒
- [x] 内屏hidpi（自行使用hidpi.sh）
- [x] 摄像头正常使用
- [ ] 内置sd卡识别
- [ ] 盒盖睡眠

#### 

