# STlink

此硬件可以烧录成stlink。

**AD的渲染图**

![](https://gitee.com/strongercjd/PCB/raw/master/STlink-OB/image/0.jpg)

使用方法

焊接完毕后，先按下图进行跳线选择，这时候外接的引脚连接的STM32F103的SWD管脚。

![](https://gitee.com/strongercjd/PCB/raw/master/STlink-OB/image/1.jpg)

这个时候使用其他的ST-link把固件烧录进去。固件名字ST-Link V2.hex。

烧录完毕，把跳线修改成如下图，这个时候外接的引脚作为ST-link的SWD管脚了，就可以使用ST-Link了（需要安装ST-link）。

![](https://gitee.com/strongercjd/PCB/raw/master/STlink-OB/image/3.jpg)



以上方法烧录之后只能使用下载功能，没有虚拟串口功能，需要虚拟串口功能如下操作

通过跳线电阻，引脚连接的STM32F103的SWD管脚，使用其他ST-Link或其他烧录工具烧录Bootloader.bin文件，安装完ST-Link驱动后，插入电脑，使用ST-LinkUpgrade2.31软件进行升级。

![](https://gitee.com/strongercjd/PCB/raw/master/STlink-OB/image/4.jpg)

选择1，连接ST-LINK，选择升级固件，选择stm32 debug + VCP + MSD进行升级

把跳线选择另一边，就可以作为ST-Link使用了，同时也是USB转串口。

**注意**

**选择USB转串口的CPU需要STM32F103CBT6，不需要USB转串口的可以选择STM32F103C8T6。**



已经打样验证没有问题了

![](https://gitee.com/strongercjd/PCB/raw/master/STlink-OB/image/5.jpg)
