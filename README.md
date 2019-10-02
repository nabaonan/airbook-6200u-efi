# airbook-6200u-efi

#### 介绍
自己定制efi，由于网上的黑苹果某些技术人员水平太差，太不负责，只能自己搞，一点点爬帖子，一点点完善，定制优化，还是不算特别完美，基本日常使用没有啥问题

#### 基本配置

cpu：i5 6200u

内存：镁光单条16g ddr3l

显卡：hd520（核显）

无线网卡：dw1560（bcm94352z）

声卡：alc269vb

显示：lg的显示器 2560x1440

硬盘：三星的固态256g

系统：osx 10.14.6

#### 功能完善度

- [x] 扩展分屏显示（没有测试外接4k，只测试外接1080p）
- [x] 睡眠唤醒（不是特别完美，唤醒会有局部闪屏现象，待进一步优化）
- [x] usb定制，usb3达到5g传输速度
- [x] 电池电量显示（显示充电图标，显示电量百分比）
- [x] 内置喇叭外放内放出声，音量调节（声音无底噪）
- [x] 无线连接，蓝牙，airdrop，投屏显示正常（睡眠唤醒不断）
- [x] cpu，硬盘温度监控，功耗监控
- [x] cpu睿频加速，自定义最低频率800，最高频率2700
- [x] 亮度调节（f1，f2   16档调节）
- [x] 开盖唤醒
- [x] 内屏hidpi（自行设置）
- [x] 摄像头正常使用
- [ ] 内置sd卡识别
- [x] 盒盖睡眠

#### 软件架构

cpu实现变频

1![](https://github.com/nabaonan/airbook-6200u-efi/blob/master/assets/1.png)

2.wifi，音频和电量可正常显示

![](https://github.com/nabaonan/airbook-6200u-efi/blob/master/assets/2.png)

3电池正常识别

![](https://gitee.com/nabaonan/airbook-6200u-efi/blob/master/assets/3.png)

4音频可以正常识别

![](https://github.com/nabaonan/airbook-6200u-efi/blob/master/assets/4.png)

5电池电量显示正常

![](https://github.com/nabaonan/airbook-6200u-efi/blob/master/assets/5.png)

6温度监控正常

![](https://github.com/nabaonan/airbook-6200u-efi/blob/master/assets/6.png)

