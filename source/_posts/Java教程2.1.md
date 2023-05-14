---
title: Java教程 1.2 Java开发工具包
date: 2023-02-19 21:14:32
tags: 
- Java教程
- 教程
- Java
catogories: Java
secret: true
---

## JVM、JRE和JDK

首先，我们要了解JVM、JRE和JDK是什么。

JVM，全称Java Virtual Machine，也就是Java虚拟机。所有Java程序都在Java虚拟机中运行，这也就是Java能跨平台运行的原因，也是Java启动慢的原因。注意，Java虚拟机不想其它虚拟机一样内存和CPU功耗那么大，简单的程序一般也就50MB左右的内存占用。JVM还需要JRE的支持才能运行Java程序。

JRE，全称Java Runtime Environment，也就是Java运行时环境，包含了JVM的所有功能。JRE可以运行`.class`文件，但不能编译`.java`文件。一般用于只运行不编译Java软件的服务器上。

JDK，全称Java Developement Kit，也就是Java开发资源包，包含了JRE的所有功能。支持编译程序，运行程序等功能。写程序通常就用的是JDK。

## JDK的安装

### Windows和MacOS

首先，进入[Oracle官网的Java下载页面](https://www.oracle.com/java/technologies/downloads/)。Java17是一个长期支持版本，建议大家用Java17。所以，找到下面的Java17按钮并点击，再点击Windows或MacOS。

- Windows7及以上请下载Windows栏的`x64 Installer`
- Intel芯片的Mac请下载MacOS栏的`x64 DMG Installer`
- Apple芯片的Mac请下载MacOS栏的`Arm 64 DMG Installer`

下载完成后，打开安装包并根据提示安装即可。

### Linux

对于Linux系统，只需在终端输入下面的指令并根据步骤即可下载到JDK17。

```bash
sudo apt-get update
sudo apt-get install software-properties-common
sudo add-apt-repository ppa:linuxuprising/java
sudo apt install oracle-java17-installer
```

[[返回目录]](https://tigercrl.github.io/2023/02/14/Java教程目录/)
