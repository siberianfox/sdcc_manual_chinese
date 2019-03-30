第一章
======

介绍
----

#### 1.1 关于SDCC

**SDCC**(small device c compiler 微控制器C编译器)是由**Sandeep
Dutta**设计的用于8位微控制器的免费开源，可重定向，优化的标准(ISO C90,ISO
C99,ISO
C11)C编译工具。当前版本可编译英特尔MCS51架构微处理器(8031,8032,8051,8052等等)、Dallas
的DS80C390以及它的一些变种,飞思卡尔(原先的摩托罗拉)的HC08系列(hc08,
s08)以及Zilog的基于Z80的MCUs (Z80, Z180, gbz80, Rabbit 2000/3000, Rabbit
3000A)和Toshiba TLCS90系列，
Zilog的Z80模式的eZ80，STMicroelectronics的STM8。SDCC它可以重定向到其它的微控制器，对Microchip
PIC系列和 Padauk
PDK15系列的支持正在开发中。编译器的全部源码都是在GPL开源协议下发布。SDCC使用ASXXXX和ASLINK的改良版本,它们是开源、可重定向汇编器和链接器。

除了针对特定MCU的优化外，SDCC也做了许多标准优化例如：

-   全局子表达式消除
-   循环优化
-   const
-   复制传播
-   死代码消除
-   jumps table for switch statements

#### 1.2 SDCC 套件许可(译注:licence)

SDCC 套件是由一些源于不同地方，拥有不同licence的组件组成的集合：

-   可执行文件：

-sdcc编译器

sdcc编译器是在GPLv2下的许可。通过sdcc生成的代码或者object文件，不受限于该许可，所以它们可以用于FLOSS或者专有(闭源)应用。

-sdcc预处理器

从GCC
[C++预处理器衍生而来http://gcc.gnu.org/;GPLv3许可](#Home:CNC:翻译:SDCC官方使用手册:C++预处理器衍生而来http:gcc.gnu.org;GPLv3许可)。

--sda汇编器和sdll链接器

从ASXXXX衍生而来，<http://shop-pdp.kent.edu/ashtml/asxxxx.htm>;
GPLv3许可。

--SDCC运行时库

主要
