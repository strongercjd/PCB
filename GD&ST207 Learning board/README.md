# ST和GD207的学习板
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

**板载资源**：

- USB串口
- 网口（RTL8201）
- 两颗LED
- RTC
- NorFlash
- 电源（5V转3.3V）
- TF卡
- 触摸按键
- 4个独立按键
- 8位并口LCD
- USB
- ESP8266的WIFI模块
- ESP8266的USB下载口

**设计缺陷**

- 四个角忘记放置定位孔
- BOOT0和BOOT1的丝印错写为GND
- 没有纽扣电池供电给RTC
- 很水的原理图和layout

**重要说明**

使用的LCD的型号是深圳市拓普微科技开发有限公司的LMT028DNHFWL，分辨率320*240，使用565模式显示一整屏幕图片需要150KB的内存。



STM32F207VC只有96KB的SRAM，只能用于显示一些文字，图形等。当然也可以使用曲线救国方式显示一张图片。



GD32F207VG有256KB的SRAM，有足够的内存显示一张图片。



<center>PCB图</center>

![](https://gitee.com/strongercjd/PCB/raw/master/GD&ST207%20Learning%20board/image/1.jpg)

<center>渲染图</center>

![](https://gitee.com/strongercjd/PCB/raw/master/GD&ST207%20Learning%20board/image/2.jpg)


<center>实物图</center>

![](https://gitee.com/strongercjd/PCB/raw/master/GD&ST207%20Learning%20board/image/0.jpg)


> 上述设计只用于学习参考使用，在普通室温环境下使用没问题，对于参考电路造成商业产品或工业产品故障，本人不负责