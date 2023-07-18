# ArchLinux安装

Arch是一个可以根据用户需求而自行定制的Linux发行版本，而它采用滚动更新的模式来提供最新稳定的版本软件。

## 本例子笔记本环境为如下：
- CPU: 12th Gen Intel i9-12900H（带核显）
- GPU: NVIDIA GeForce RTX 3060
- 电脑上已经存在一个windows11专业版系统
- 注意！这是一篇关于双系统的安装方法

## 准备工作：
  1.[在Arch Linux 中文维基下载iso镜像](https://archlinux.org/download/)  
  
  2.使用免费开源的工具[Ventoy](https://github.com/ventoy/Ventoy/releases)在windows上写入引导信息在u盘  
  
  该工具会把u盘分为两个分区，一个分区是存放着引导信息，另一个分区存放iso镜像，而我们需要把下载好的iso放进u盘里面  

  3.在windows的磁盘管理，选择一个分区(卷)压缩它的空间，来作为后面arch系统的根分区空间  

  4.检查windows上是否关闭了快速启动，重启，然后在 BIOS 关闭安全启动  

  5.找到您电脑的启动快捷键，在启动列表中，选择您的u盘  

  选择您的arch镜像，然后默认第一项启动，加载一会然后就会进入一个tty界面

  ## 安装arch:
  注意：必须确保是UEFI 模式下启动，可以自行输入ls /sys/firmware/efi/efivars指令来进行判断，如果能列出大量文件，则为UEFI 模式  

  1.连接wifi，不是使用wifi的可以跳过此步骤  

  注意：如果使用手机通过数据线共享网络，笔者使用的安卓手机出现了导致手机重启的情况，所以笔者还是建议使用wifi好  

  
  
