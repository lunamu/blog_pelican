Title: 在墙内正确使用CodeSkulptor和Owltest
Date: 2014-06-11
Category: Coursera 
Tags: GoAgent, GFW  
Author: Lunamos

在Coursera上选了个Rice University的Principle of Computing，发现Scott Rixner在该课程该Owltest进行测试的方法十分方便，但在墙内无法使用，花了一下午摸索得到解决方案如下：

- 使用[乐飞加速器](http://www.lejsq.com/)能够实现CodeSkulptor的保存、模块加载等功能。
- 使用[GoAgent](https://code.google.com/p/goagent/)配合[乐飞加速器](http://www.lejsq.com/)能够实现OwlTest的测试功能。GoAgent的模式应当选择“GoAgent PAC”，不然会在测试界面超时。

另外注意，开了GoAgent之后，CodeSkulptor就不能进行保存和模块import了，所以二者分步进行。

终于有了点进行这个课的动力了。
