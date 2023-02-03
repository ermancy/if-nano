#IF NANO

#### introduce
One is suitable for zmk, and the software and hardware are compatible with nice! Nano's main control.
IFNANO mainly refers to nice! Nano's design is re-layouted as a double-sided board, and a switch function and an ipx antenna socket (1st generation) are added, which reduces production costs and improves practicability.
At present, the basic functions have been tested and can be used normally.

#### Circuit Design
For details, please see the Schematic_IFNANOV5_2022-08-10.pdf file, which is basically a nice clone! Nano original design.
Bootloader can use nice directly! The nano file, the test uses nice_nano_bootloader-0.6.0_s140_6.1.1.hex, has been attached.


#### Soldering Tutorial
Due to space reasons, the silkscreen of the original part is removed from the pcb, so please refer to the "Soldering Assistant" file for the specific value and position of the original part.
The "Welding Assistant" file is essentially a web page, which needs to be opened with a browser.

#### Instructions for use
![](./img/top.png)


1. The LED in the upper right corner is a red LED. When the light is on, it is in the charging state. If it is not on, it is in the full state or not in the charging state (not plugged in).
2. The LED in the lower left corner is the function indicator light, which will display breathing in the BL state, and will not light up in the normal working state.
3. The extra row of four-hole interface in the lower left corner of the pcb is the SWD interface, use jlink to burn the bootloader program or erase the chip.
4. There are two antennas in this design, the front is a patch antenna (bottom, red original), and the back is an ipx generation antenna base. Please choose one of these two antennas when using them, and do not use them at the same time.
5. There is a switch designed on the back, and a 1-digit SMD DIP switch is required. (untested)
6. This design uses ti bq24057 charging chip, supports 4.2V lithium battery, and nice! Nano is the same. The chip is set in usb 500ma mode, and a resistor (R9 1.68K) is reserved to control the charging current. The actual test keeps the maximum charging current at about 430ma, accompanied by a certain amount of heat, so be careful to touch the pcb board when charging. (There is no specific test for the heating temperature. Personally, it is estimated to be about 60 degrees, and the work is stable and normal)
7. 32k crystal needs to be installed



#### References

1. https://nicekeyboards.com/docs/nice-nano/pinout-schematic
2. https://github.com/joric/jorne/wiki

   

#### connect:

IFKB customized QQ group

78769032



author

(QQ)463365135

(email)463365135@qq.com



# IF NANO

#### 介绍
一个适用于用于zmk，软硬件兼容nice！nano的主控。
IFNANO主要参考了nice！nano的设计，重新layout为双面板，并且增加了开关功能和ipx天线插座（1代），降低了生产成本的同时提高了实用性。
目前基本功能已经完成测试，可以正常使用。

#### 电路设计
具体请看Schematic_IFNANOV5_2022-08-10.pdf文件，基本就是克隆nice！nano原版设计。
bootloader可以直接使用nice！nano的文件，测试使用的是nice_nano_bootloader-0.6.0_s140_6.1.1.hex，已经附上。


#### 焊接教程
因为空间的原因，pcb上去除了原件相关的标号丝印，所以具体原件的值和位置请参考“焊接助手”文件。
“焊接助手”文件本质是一个网页，需要用浏览器打开。

#### 使用说明
![](./img/top.png)


1.  右上角LED为红色LED，亮灯为充电状态，不亮为充满状态或者不在充电状态（未插线）。
2.  左下角LED为功能指示灯，在BL状态下会呼吸显示，正常工作状态不亮。
3.  pcb左下角多出来的一排四孔接口为SWD接口，使用jlink用来烧录bootloader程序或者擦除芯片。
4.  本设计是有两个天线，正面是贴片天线（底部，红色原件），背面是ipx一代天线座。这两个天线在使用的时候请二选一，不要同时使用。
5.  背面设计有开关，需要使用1位的贴片拨码开关。（未经测试）
6.  本设计使用的是ti bq24057充电芯片，支持4.2V锂电池，与nice！nano的一致。芯片设定在usb 500ma模式，保留了一个控制充电电流的电阻（R9 1.68K），实际测试最大保持充电电流在430ma左右，伴随一定的发热量，所以充电的时候谨慎触摸pcb板。（没有具体测试发热温度，个人估计是60度左右，工作稳定正常）
7.  32k晶振需要安装



#### 参考资料

1.  https://nicekeyboards.com/docs/nice-nano/pinout-schematic
2. https://github.com/joric/jorne/wiki

   

#### 联系:

IFKB客制化QQ群 

78769032



作者

(QQ)463365135

(email)463365135@qq.com


