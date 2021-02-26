# Jlink-OB

ST-link的硬件可以烧录成stlink，也可以烧录成Jlink

AD的渲染图

使用方法

焊接完毕后，先按下图进行跳线选择，这时候外接的引脚连接的STM32F103的SWD管脚。

这个时候使用其他的ST-link或者Jlink把固件烧录进去。固件可以选择J-Link.hex或者ST-Link V2.hex。

烧录完毕，把跳线修改成如下图，这个时候外接的引脚作为ST-link或Jlink的SWD管脚了，就可以使用ST-Link或Jlink了（需要安装ST-link或Jlink的驱动）。

