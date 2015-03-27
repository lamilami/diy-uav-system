![https://diy-uav-system.googlecode.com/files/BOARD_PIC2.jpg](https://diy-uav-system.googlecode.com/files/BOARD_PIC2.jpg)

**UAV 系统大致可分为3部分**
1. 机载部分
2. 无线链路部分
3. 地面站

如果在视距范围内做定点航迹飞行，后两项可以省略。我们这里重点要做的就是第一项---机载部分
机载部分可分为姿态控制部分和导航部分，有人将其做成两块板分别做飞控和导航，有的只使用一个板将导航和控制整合在一个处理器上运行。本方案使用一个板有两个处理器一个用来做姿态控制另一个做导航，双处理器之间采用的是CAN总线通信方式，保证了数据传输的可靠性。目前导航点最大值设定为 64个way points.

_**整个板子的名字还没想好 ：-）。。。**_


飞控VIDEO:

**自导航飞航线测试：**
视频1 http://v.youku.com/v_show/id_XNDk0NDAwNDU2.html

视频2 http://v.youku.com/v_show/id_XNTA5ODcyODky.html


**神经元自适应PID算法在飞行器姿态控制上的应用**

视频3 http://v.youku.com/v_show/id_XMzg3NTAwNDEy.html

**惯导测试飞行视频--四旋翼室外自主GPS悬停飞行视频**
http://v.youku.com/v_show/id_XNTIxNzk3NDU2.html

> 3.MAVLINK1.0 协议
> 什么是MAVLINK协议，为什么要使用MAVLINK

> MAVLINK 的英文注解：Micro Air Vehicle Communication Protocol，协议主页：http://qgroundcontrol.org/mavlink/start
> 该协议具有 数据结构简洁，通信量小，功能覆盖全，扩展性强等特点，目前已经成为微型无人机控制领域内的标准协议，包括 APM，AR.DRONE,PixHAWK等飞控平台均使用MAVLINK协议作为通信协议。

  * 连接地面站视频演示：**http://v.youku.com/v_show/id_XNTI5MzIwOTg0.html**

> 当前飞控板使用的是惯性导航算法和神经元自适应PID控制输出，姿态刷新率200Hz，支持MAVLINK1.0协议。


**飞行前做仿真是必须的:**

使用FlightGear 做模拟飞行

![http://diy-uav-system.googlecode.com/files/sim2.jpg](http://diy-uav-system.googlecode.com/files/sim2.jpg)

**模拟控制飞行的仿真视频：**
http://v.youku.com/v_show/id_XMzE0MzgxNzc2.html




**GPS/IMU板 + 导航控制主板 + 数传模块：**

![https://diy-uav-system.googlecode.com/files/C10.jpg](https://diy-uav-system.googlecode.com/files/C10.jpg)

尺寸60mm（长） X 50mm（宽）



板上集成有3轴陀螺仪；3轴加速度计,FUTABA SBUS 接收机，罗盘和GPS。
处理器为两片STM32芯片分别负责姿态和导航。


**2013年7月 最新飞控板装机**

**飞控板固件程序：**

https://diy-uav-system.googlecode.com/files/GCS_FC_201308013_v01_115200.dfu

**装机后的飞行测试视频**
http://v.youku.com/v_show/id_XNTk1NTA1MTA4.html



![https://diy-uav-system.googlecode.com/files/C20.jpg](https://diy-uav-system.googlecode.com/files/C20.jpg)


---


**有关 无刷电机直驱 云台的开发**

经过一段时间的摸索和研究 掌握了一些较为成熟的控制方法，形成了一整套无刷云台的控制方案。

装机图片（前面的十字架夹在电机下面，起飞时震动的非常厉害）：![https://diy-uav-system.googlecode.com/files/C22.jpg](https://diy-uav-system.googlecode.com/files/C22.jpg)

**云台拍摄视频：** http://v.youku.com/v_show/id_XNTk4NTUzMzgw.html

**飞行测试  http://v.youku.com/v_show/id_XNTk4NDc5NTk2.html**

**测试视频：** http://v.youku.com/v_show/id_XNTk3OTQ2MDg0.html







---



**航模选型及安装方法 详见：**[AssembleMyPlane](AssembleMyPlane.md)


**飞行操控方法及整机调试 详见：**[ReadyToGo](ReadyToGo.md)


**使用地面站工具编辑一个航线 方法详见：**[EditMyPoint](EditMyPoint.md)











