# ROS-Learning
##  1.Beaginner Tutorials

### 1.1 [Installing and Configuring Your ROS Environment](http://wiki.ros.org/ROS/Tutorials/InstallingandConfiguringROSEnvironment)

> 安装ubuntu 

首先要安装ubuntu环境。本次学习，通过虚拟机的方式安装ubuntu

https://multipass.run/是一个管理虚拟机的项目,可管理多个虚拟机。下载后搭配https://www.oracle.com/virtualization/technologies/vm/downloads/virtualbox-downloads.html使用

但是multipass 启动的系统都是server，没有desktop，本次采用了https://discourse.ubuntu.com/t/graphical-desktop-in-multipass/16229的方法给虚拟机添加图形界面；然后就可以在virtualbosx中使用了。

> 安装ROS

按照官方文档安装，遇到的第一个问题是http://wiki.ros.org/noetic/Installation/Ubuntu#Installation.2FUbuntu.2FSources.Set_up_your_keys

执行命令

- ```shell
  curl -s https://raw.githubusercontent.com/ros/rosdistro/master/ros.asc | sudo apt-key add -
  ```

下载添加key时包错：gpg: no valid OpenPGP data found.

解决方法：试了网上很多的方法都没有解决，思路是吧链接的内容下载到虚拟机中，然后添加到key中

