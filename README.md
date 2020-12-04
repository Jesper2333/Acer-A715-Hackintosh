# Acer-A715-Hackintosh
Acer Aspire 7 A715 黑苹果 (OpenCore引导，仅在Big Sur正式版11.0.1进行测试) 
 
具体型号：Acer Aspire 7 A715-75G-55XU

(理论与此机型***使用相同BIOS***的机器均可使用该引导)

(理论与此机型***配置相近的Acer机器***也能使用该引导)

 配置| |
 ----|-----|
 CPU|Intel Core i5-9300H
 核显|Intel UHD Graphics 630
 独显|NVIDIA GeForce GTX 1650
 声卡|Reatlk ALC 255
 有线网卡|Realtek RTL8168H/8111H PCI Express Gigabit Ethernet
 无线网卡|Intel Wi-Fi 6 AX200 

**请务必解锁CFG Lock，不解锁无法使用该引导**

**[感谢知乎大佬提供的免刷BIOS，免引导U盘的傻瓜式CFG解锁方案](https://zhuanlan.zhihu.com/p/266400995)**

**注意：该型号只需要关闭CFG Lock，不需要修改DVMT**

**Intel的无线网卡请配合[HeliPort](https://github.com/OpenIntelWireless/HeliPort/releases/download/v1.0.2-alpha/HeliPort.dmg)使用，非常感谢[OpenIntelWireless项目组](https://github.com/OpenIntelWireless)**

已知存在的问题（系统：macOS Big Sur 11.0.1）
-

1、独显无法驱动（该问题目前全球无解）

2、HDMI无法使用（因为独显无法驱动，该问题无解）

3、触控板只能在PS2模式下使用，在macOS下手势正常（BIOS可进行设置，PS2模式下Windows不能使用触控板手势）

4、耳机接口没反应

可能遇到的问题
-

1、进入安装界面后找不到硬盘：进入BIOS，在“Main”栏目下，按下Ctrl+S，BIOS会显示部分隐藏选项，把SATA设置成AHCI模式。

2、进入系统后无法使用触控板：进入BIOS，在“Main”栏目下，按下Ctrl+S，BIOS会显示部分隐藏选项，把触控版由“I2C”改为“PS2”

（注意⚠️：该操作将会导致在Windows下无法使用触控板手势，macOS下手势正常）

3、Intel无线网卡不知道怎么用：[请配合HeliPort软件使用，点击下载](https://github.com/OpenIntelWireless/HeliPort/releases/download/v1.0.2-alpha/HeliPort.dmg)

运行效果图
-
![1](https://github.com/Jesper2333/Acer-A715-Hackintosh/blob/main/p1.png)

![2](https://github.com/Jesper2333/Acer-A715-Hackintosh/blob/main/p2.png)

![3](https://github.com/Jesper2333/Acer-A715-Hackintosh/blob/main/p3.png)


