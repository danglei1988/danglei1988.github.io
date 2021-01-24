---
title: Nexus 5X的Android 8.0 Oreo刷机步骤
tags:
  - Android
  - Nexus5X
  - Oreo
id: '418'
categories:
  - - 他山之玉
date: 2017-09-06 21:56:39
---

首先，下载最新版的驱动：[platform-tools-latest-windows.zip](https://dl.google.com/android/repository/platform-tools-latest-windows.zip) （Qiang） 解压，win+R输入cmd，进入命令行，使用cd命令进入刚解压的文件夹中，输入：

> adb version

若出现： ![image](http://ws3.sinaimg.cn/large/82054d13ly1fiu3g06s6fj20oi02rdht.jpg) 说明adb配置成功。 下载Android 8.0 Oero镜像：[Android 8.0 System Images](https://developer.android.com/about/versions/oreo/download.html) 解压文件到上面的驱动文件目录下（为刷机时方面调用文件），目录文件大致如下： ![image](http://ws3.sinaimg.cn/mw690/82054d13ly1fiu47u4rpuj20ky0cmjsp.jpg) 电脑连接手机，手机打开USB调试模式， 命令行中输入：

> adb devices

查看ADB是否连接成功，若成功，重启至bootloader：

> adb reboot bootloader

如果显示设备被锁，请输入 ：

> fastboot oem unlock

进入bootloader后，命令行定位到刷机包文件所在目录，输入：

> flash-all.bat

待刷机完成，重启手机。 ![image](http://ws3.sinaimg.cn/mw690/82054d13ly1fiu3kwvi5tj20u01hc41m.jpg)

* * *

5X可能出现”missing system.img”的错误，解决办法参见：[http://www.pixcn.cn/article-2798-1.html](http://www.pixcn.cn/article-2798-1.html) 解压zip刷机包，单个刷入包（注意文件名对应包下文件）：

> fastboot erase cache fastboot erase userdata fastboot flash bootloader **bootloader-bullhead-bhz21c.img** fastboot flash radio **radio-bullhead-m8994f-2.6.39.3.03.img** fastboot reboot-bootloader fastboot flash recovery recovery.img fastboot flash boot boot.img fastboot flash system system.img

用以上方式刷Android 8.0 无法开机，后发现原因为fastboot版本太旧，本文开头部分找最新adb、fastboot驱动，用新版驱动fastboot.bat直接刷机即可，无需单刷各个包。 注意：如果你的环境变量中添加过fastboot，要么删除环境变量中的fastboot文件，要么命令行定位到新驱动目录，fastboot.exe调用。 原文转载自[Wonpn博客](http://wonpn.com/?p=123)，菊部也亲测成功，感谢Wonpn的分享。