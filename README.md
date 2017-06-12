### 基于TCP的socket网络传输图片（C++, python）###

### 一. 概述 ###


Socket的英文原义是“孔”或“插座”。作为BSD UNIX的进程通信机制，取后一种意思。通常也称作"套接字"，用于描述IP地址和端口，是一个通信链的句柄，可以用来实现不同虚拟机或不同计算机之间的通信。在Internet上的主机一般运行了多个服务软件，同时提供几种服务。每种服务都打开一个Socket，并绑定到一个端口上，不同的端口对应于不同的服务。Socket正如其英文原意那样，像一个多孔插座。一台主机犹如布满各种插座的房间，每个插座有一个编号，有的插座提供220伏交流电， 有的提供110伏交流电，有的则提供有线电视节目。 客户软件将插头插到不同编号的插座，就可以得到不同的服务。网络上的两个程序通过一个双向的通信连接实现数据的交换，这个连接的一端称为一个socket。

而socket与socket之间的连接以及数据传输需要一种规则，也就是我们通常所说的网络传输协议，最常用的有TCP和UDP，这两种协议的区别如下：

1.基于连接与无连接；

2.对系统资源的要求（TCP较多，UDP少）；

3.UDP程序结构较简单；

4.流模式与数据报模式 ；

5.TCP保证数据正确性，UDP可能丢包，TCP保证数据顺序，UDP不保证。

接下来将以图片传输为例，用Python和C++实现服务端和客户端。这里不用语言得到的端口之间也可以互相连接。

### 二. 运行要求 ###

（1）OpenCV

（2）Python 2.7 

（3）C++的源文件要求windows环境


### 三. 参考资料 ###

[C++ Socket编程步骤](http://blog.csdn.net/cyh183269855/article/details/70596463)

[Python Socket 编程详细介绍](https://gist.github.com/kevinkindom/108ffd675cb9253f8f71)

[树莓派用Python写几个简单程序5：用socket传图像](https://my.oschina.net/RagingTyphoon/blog/492950)
