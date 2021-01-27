# ST和GD207的最小系统板
**兼容ST207和GD207**

代码开源地址：

STM32F207代码仓库

[GitHub仓库](https://github.com/strongercjd/STM32F207VCT6)

[码云仓库](https://gitee.com/strongercjd/STM32F207VCT6)

GD32F207代码仓库

[GitHub仓库](https://github.com/strongercjd/GD32F207)

[码云仓库](https://gitee.com/strongercjd/GD32F207)

| 引脚编号    | STM32F207 | GD32F207    | 兼容设计 |
| :---------- | --------- |--------- |--------- |
| 19 |接上VDD电源，再接电容接地  |接地|通过0欧姆电阻选择不同电路|
| 20 |接地  |VREF-，可以接地|直接接地|
| 49 |接电容接地  |接地|PCB设计电容接地，ST贴电容，GD贴0欧姆电阻|
| 73 |接电容接地  |悬空|PCB设计电容接地，ST贴电容，GD不贴|
| 99 | 悬空 |接电容接地|PCB设计电容接地，ST不贴，GD贴电容|

<center>PCB图</center>

![](https://gitee.com/strongercjd/PCB/raw/master/GD&ST207%20Mini%20System/image/1.jpg)

<center>渲染图</center>

![](https://gitee.com/strongercjd/PCB/raw/master/GD&ST207%20Mini%20System/image/2.jpg)


<center>实物图</center>

![](https://gitee.com/strongercjd/PCB/raw/master/GD&ST207%20Mini%20System/image/0.jpg)