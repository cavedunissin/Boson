# f7計數模組

## 实物图片

![Optional title](.gitbook/assets/boson-ji-shu-mo-kuai-shi-wu-tu.png)

## 基本信息

中文名称：计数模块

英文名称：Reversible Counter Module

序号：f7

SKU 号：BOS0026

## 模块简介

计数模块是功能模块中的一种，可以用来实现计数功能，还可以和其他模块组合使用，实现更为复杂的功能，如定时器、按键计数器、累加器等。

## 使用说明

计数模块可以通过接收输入接口的高脉冲信号来实现计数功能。在计数模式下，当接收到置零口的低电平信号时，计数会被清零。计数模块可以通过板载开关进行选择四种模式：

up模式（向上计数）：每输入一个高脉冲信号，计数器加1，范围为0-999。

down模式（向下计数）：每输入一个高脉冲信号，计数器减1，范围为0-999。

value模式（模拟值）：读取模拟值大小，并输出对应大小的模拟值，范围0-999。

volts模式（电压值）：读取电压值大小，并输出对应大小的电压值，单位为伏特\(V\)。

计数模块的输入输出口如下图所示：

![Optional title](.gitbook/assets/boson-ji-shu-mo-kuai-shi-yong-shuo-ming-1.png)

按照下图所示连接电路即可实现每按一次键，计数器加1。

![Optional title](.gitbook/assets/boson-ji-shu-mo-kuai-shi-yong-shuo-ming-2.png)

## 原理介绍

计数模块可以实现简单的计数功能。在up模式下，输入接口每接收一个高脉冲，计数器加1；在down模式下，输入接口每接收一个高脉冲，计数器减1；置零口每接收一个低脉冲，计数清零。

## 应用样例

### **\(1\) 按键计数器**

**样例说明：** 按钮每按一次，计数加1。

**元件清单：** 按钮模块；计数模块；电源主板-单路。

**连线图：**

![Optional title](.gitbook/assets/boson-ji-shu-mo-kuai-an-jian-ji-shu-qi-lian-xian-tu.png)

### **\(2\) 制作存钱罐**

**样例说明：** 每次投币时，硬币会使得倾斜开关倾斜，倾斜开关每倾斜一次，计数模块计数加1。

**元件清单：** 按钮模块；计数模块；倾斜传感器；电源主板-单路。

**连线图：**

![Optional title](.gitbook/assets/boson-ji-shu-mo-kuai-zhi-zuo-cun-qian-guan-lian-xian-tu.png)

### **\(3\) 景区客流量计数器**

**样例说明：** 保证恰当的景区客流量对游客安全非常必要，将运动传感器安置在景区入口安检处，每经过一人，计数器加1，实时监控客流量大小，掌握景区人数，保证游客安全。

**元件清单：** 按钮模块；计数模块；运动传感器；电源主板-三路。

**连线图：**

![Optional title](.gitbook/assets/boson-ji-shu-mo-kuai-jing-qu-ke-liu-liang-ji-shu-qi-lian-xian-tu.png)

## 规格参数

引脚说明： ![Optional title](.gitbook/assets/boson-ji-shu-mo-kuai-yin-jiao-shuo-ming.png)

尺寸：38mm\*32mm

工作电压：3.0-5.5V

