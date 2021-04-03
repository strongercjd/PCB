# JlinkV9

此硬件可以烧录成Jlink V9。

**AD的渲染图**

![](https://gitee.com/strongercjd/PCB/raw/master/JlinkV9/image/0.jpg)

使用方法

焊接完毕后，先按下图进行跳线选择，这时候外接的引脚连接的STM32F205RET6的SWD管脚。

![](https://gitee.com/strongercjd/PCB/raw/master/JlinkV9/image/1.jpg)

烧录方式有两种：

1、不可升级

直接烧录\Tools\Firmware\不可升级\J-Link V9 ALL.bin文件。缺点是，使用IAR或Keil时会提示升级Jlink固件，点击否，不升级。每次debug都需要点击，比较烦。至于需不需要修改SN，我测试了下，是不需要的。（我就简单测试下，我正在用的JlinkV9 mini，使用方法2烧录的）



2、可以升级

烧录Tools\Firmware\可以升级\bootloader.bin。烧录完毕后，打开J-Link Commander V6.98c（我使用的Jlink驱动版本是V6.98c），打开后，会提示升级，点击升级即可。升级完后，需要添加license，使用方法和工具在Tools\Firmware\可以升级\添加license.rar中。



烧录完毕，把跳线修改成如下图，这个时候外接的引脚作为Jlink的SWD管脚了，就可以使用Jlink了（需要安装Jlink的驱动）。

![](https://gitee.com/strongercjd/PCB/raw/master/JlinkV9/image/3.jpg)



已经打样验证没有问题了

![](https://gitee.com/strongercjd/PCB/raw/master/JlinkV9/image/4.jpg)

