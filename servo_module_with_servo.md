# 舵机控制模块

## 实物图片

![Optional title](.gitbook/assets/boson-duo-ji-kong-zhi-mo-kuai-shi-wu-tu.jpg)

## 基本信息

中文名称：舵机控制模块

英文名称：Servo Controller Module

序号：o10

SKU 号：BOS0025

## 模块简介

舵机控制模块是一种位置（角度）伺服的驱动器，适用于那些需要角度不断变化并可以保持的控制系统。目前，舵机控制模块在高档遥控玩具，如飞行器、机械手臂、潜艇模型、遥控机器人等场景中已经得到了普遍应用。

![Optional title](.gitbook/assets/boson-duo-ji-kong-zhi-mo-kuai-shi-li.png)

## 使用说明

舵机控制模块既可以接收数字信号，也可以接收模拟信号，分别对应swing模式和turn模式：

swing模式：舵机在指定角度和初始角度之间来回摆动；

turn模式：舵机转到指定角度后静止。

这两种模式可以通过舵机控制模块上的拨动开关进行切换。按照下图所示连接电路，通电后即可通过舵机控制模块上的拨动开关控制舵机。

![Optional title](.gitbook/assets/boson-duo-ji-kong-zhi-mo-kuai-shi-yong-shuo-ming.png)

## 原理介绍

舵机控制模块主要是由外壳、电路板、驱动马达、减速器与位置检测元件所构成。其工作原理是由接收机发出讯号给舵机，经由电路板上的IC驱动无核心马达开始转动，透过减速齿轮将动力传至摆臂，同时由位置检测器送回讯号，判断是否已经到达定位。位置检测器其实就是可变电阻，当舵机转动时电阻值也会随之改变，藉由检测电阻值便可知转动的角度。

## 应用样例

### **\(1\) 爬爬虫**

**样例说明：** 通过自锁开关和舵机控制模块控制舵机像虫子一样向前爬动。

**元件清单：** 自锁开关；舵机控制模块；9g金属舵机模块；电源主板-单路。

**连线图：**

![Optional title](.gitbook/assets/boson-duo-ji-kong-zhi-mo-kuai-pa-pa-chong-lian-xian-tu.png)

### **\(2\) 自动浇花装置**

**样例说明：** 利用土壤湿度传感器实时监测花盆中土壤的含水量，当土壤湿度值较小时，舵机带动软管口降低，达到自动浇水的目的。

**元件清单：** 土壤湿度传感器；9g金属舵机模块；软管；micro:bit；micro:bit BOSON扩展板。

**连线图：** 将土壤湿度传感器连接至micro:bit扩展板引脚P0，舵机模块连接至micro:bit扩展板引脚P8。

![Optional title](.gitbook/assets/boson-duo-ji-kong-zhi-mo-kuai-zi-dong-jiao-hua-zhuang-zhi-lian-xian-tu.png)

**执行流程：**

① 土壤湿度传感器检测土壤湿度值。

② 判断湿度值大小，如果湿度值小于600，即土壤较干时，舵机转动90°，带动软管口降低，实现浇水功能；否则，舵机一直保持在0°不动。

**程序示意图（中文版）：**

![Optional title](.gitbook/assets/boson-duo-ji-kong-zhi-mo-kuai-zi-dong-jiao-hua-zhuang-zhi-cheng-xu-shi-yi-tu-zhong-wen-ban.png)

**程序示意图（英文版）：**

![Optional title](.gitbook/assets/boson-duo-ji-kong-zhi-mo-kuai-zi-dong-jiao-hua-zhuang-zhi-cheng-xu-shi-yi-tu-ying-wen-ban.png)

## 规格参数

引脚说明：

![Optional title](.gitbook/assets/boson-duo-ji-kong-zhi-mo-kuai-yin-jiao-shuo-ming.png)

尺寸: 26mm\*22mm

工作电压:3.3V-5.0V

