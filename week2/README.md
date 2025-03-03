---
cover: ../.gitbook/assets/100107076_p0_master1200.jpg
coverY: 0
---

# Lesson 2

## 一 任务

* 初步掌握Arduino nano各引脚作用
* 掌握arduino烧录程序步骤
* 熟悉使用面包板
* 利用nano板点亮二极管灯泡|[代码地址](https://github.com/NJURobotClub/arduino\_teaching/blob/c0e8ddbf151aac21e55acbd8d0355d32ab56b068/week2/led.ino)



## 二 器材

* LED灯\*1
* Arduino Nano 板 \*1
* USB-micro数据线\*1
* 面板板、排针、杜邦线

## 三 模块介绍

### 1 面包板

#### 介绍

> **面包板**（Breadboard）或叫**免焊万用电路板**（solderless breadboard）是[电子电路设计](https://zh.wikipedia.org/wiki/%E7%94%B5%E5%AD%90%E7%94%B5%E8%B7%AF%E8%AE%BE%E8%AE%A1)中所常用的一种基底。

由于板子上有很多小插孔，各种电子元器件可根据需要任意插入或拔出，免去了焊接的工序，节省了电路的组装时间，且元件可以重复使用，非常适合电子电路的组装、调试和训练。

面包板背面有背胶，方便其贴在不同的仪器上。

​​\


<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FZxeMQfMZX2oMRKHn9QX1%2Fuploads%2Fd4ZThbLa6esDfxtCPb18%2Fbreadboard.jpg?alt=media&#x26;token=f38524b1-bb53-4ff6-b5b9-b8f1eb07468e" alt=""><figcaption></figcaption></figure>

#### 结构

1.  电源轨

    在面包板的上下两侧分别有两列插孔，一般是作为电源引入的通路。上方第一行标有“+”的一列有5组插孔，每组5个（内部5个孔连通），均为正极。上方第二行标有“-”的一列有5组插孔，每组5个（内部5个孔连通），均为接地。面包板下方第一行与第二行结构同上。如需用到整个面包板，通常将“+”与“+”用导线连接起来，“-”与“-”用导线连接起来。

<figure><img src="../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>



<figure><img src="../.gitbook/assets/breadboard-power-slots2.jpg" alt=""><figcaption></figcaption></figure>



2\. 接线轨

连接孔分为上下两部分，是我们的主工作区，用来插接原件和跳线。在同一列中的5个插孔（即a-b-c-d-e，f-g-h-i-j）是互相连通的；列和列（即1-30）之间以及凹槽上下部分（即e-f）是不连通的。



<figure><img src="../.gitbook/assets/breadboard-slots.jpg" alt=""><figcaption></figcaption></figure>

### 2 Arduino Nano

Arduino Nano结构

![](../.gitbook/assets/nano.jpg)

我们主要使用Digital Pins

Arduino Nano板需要**电源供电**

有三种方式：

* USB接口：电源电压是稳定的+5V的直流电压。
* 5V Pin：为Arduino开发板供电使用，也可以为外部电子元件提供+5V电源。
* Vin：Vin引脚为Arduino开发板供电时，直流电源电压必须为7V \~ 12V。

#### 四 点亮二极管

引脚连接：

Arduino

| Arduino Nano               | LED等 |
| -------------------------- | ---- |
| 3.3V / D13(Digital Pin 13) | 长端   |
| GND                        | 短端   |
