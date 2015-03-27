#**操控方法及调试**

# Introduction #
**搭建这套系统的理念就是尽量减少人为操作，达到最大程度的无人飞行，因此本套系统不同于传统操作方法，操控方式摒弃了传统的遥控器，取而代之的是游戏操作杆。
因此其操作方式更接近在电脑上玩飞行模拟器，不过这次你实际控制的可是个真的能飞的飞机。**

http://using-joystick-as-remote-control.googlecode.com/files/BLOCK.JPG


_**无论是手工操控还是自动飞行，姿态自动平衡都处于工作状态**_

**使用 4-方向键 当作 微调 键**


> 上下键用于 【俯仰量】 微调
> Up-Down key is for Pitch FINE adjustment.

> 左右键用于 【侧倾量】 微调
> Left-Right key is for Roll FINE adjustment.


http://using-joystick-as-remote-control.googlecode.com/files/FINE_ADJ.JPG



# Details #


  * **操纵杆的连接**

> 操纵杆采用的是 USB 操纵杆，将其USB接头插入数据转发器中即可。

> http://diy-uav-system.googlecode.com/files/JOY_RC1.JPG

  * **操纵杆的按键定义**
![http://diy-uav-system.googlecode.com/files/JOYSTICK1.jpg](http://diy-uav-system.googlecode.com/files/JOYSTICK1.jpg)

> 在左手一侧的“7”号按键定义为手动操作键---按一下“7”号键后飞机进入人工手动操作。


> 在右手一侧的“8”号按键定义为自动导航键---按一下“8”号键后飞机进入按航点自动飞行模式。


  * **操控方法**

  * **如何启动电机和停止电机**
> 开机时飞机控制板初始状态为停机状态

> 启动电机：将右手操作杆下拉至最低并保持5秒钟后，停机状态解除，稍微上推拉杆电机便可启动。

> 如果当前处在启动状态，将右手操作杆下拉至最低并保持5秒钟后便可解除启动状态并进入停机状态，即便上推拉杆电机也不会启动。

  * **自动飞行模式与手工操作模式的切换方法**
> 开机时飞机控制板初始状态为手动模式和停机状态，首先解除停机状态，将飞机对准第一个航点的方向启动电机加速起飞，起飞后 按下右手一侧的“8”号键进入自动飞行模式。

> 飞机飞回来后当进入到最后一个航点时按下左手一侧的“7”号键进入手动飞行模式，降低电机转速让飞机缓缓滑行降落后将右手操作杆下拉至最低并保持5秒钟以解除启动状态并进入停机状态。。。一次飞行结束。



