# Jlink-OB

此硬件可以烧录成Jlink。

**AD的渲染图**

![](https://gitee.com/strongercjd/PCB/raw/master/Jlink-OB/image/0.jpg)

使用方法

焊接完毕后，先按下图进行跳线选择，这时候外接的引脚连接的STM32F103C8T6的SWD管脚。

![](https://gitee.com/strongercjd/PCB/raw/master/Jlink-OB/image/1.jpg)

这个时候使用其他的ST-link或者Jlink把固件烧录进去。固件可以选择J-Link.hex或者J-Link-OB-2.bin。我使用的是J-Link-OB-2.bin，使用时Keil和IAR不会提示升级Jlink。

烧录完毕，把跳线修改成如下图，这个时候外接的引脚作为Jlink的SWD管脚了，就可以使用Jlink了（需要安装Jlink的驱动）。

![](https://gitee.com/strongercjd/PCB/raw/master/Jlink-OB/image/3.jpg)



已经打样验证没有问题了

![](https://gitee.com/strongercjd/PCB/raw/master/Jlink-OB/image/4.jpg)

