---
title: 将不愿自启的Android应用放进黑域
tags:
  - Android
  - 黑域
id: '142'
categories:
  - - 日常&amp;搞机
date: 2017-03-01 11:19:18
---

Android 在于折腾，自启和唤醒一直是一个十分蛋疼的问题，也影响着 Android 的使用体验，尤以国内大厂的相互唤醒为甚，今天分享一个叫做**黑域**的黑科技神器。

## 黑域是什么

黑域就是曾经的组织运行（遥远的菊部1.0时代曾经分享过，可惜现在并没办法找到地址了），是由开发者 Brevent 开发的一款不需要 root 的 Android 防唤醒应用。 黑域使用一些黑科技休眠（Android 6.0引入）或者强行停止应用，防止程序持续运行。黑域不需要 root，也不需要改变系统。 黑域通过事件智能判断您是否在使用应用，当您打开某个应用，使用完退出以后，黑域会休眠它；如果您从最近列表划掉它，黑域会强行停止它。对于任何恶意唤醒，只要您没有打开过，都将强行停止它

## 黑域怎么用

这里分两部分来说：

### 懒人用户

自认为懒人用户或小白用户的话，可以直接不用看后面的部分，直接到酷安去下载[黑域](http://www.coolapk.com/apk/me.piebridge.brevent)和[黑域一键补丁](http://www.coolapk.com/apk/tk.schspa.preventpatch)。 分别安装好黑域和黑域一键补丁后，打开黑域一键补丁按照提示说明一步步操作即可，注意在过程中需要打开开发者模式中的网络 ADB 调试功能，并且切记在打好黑域补丁后将网络 ADB 调试功能关闭。 然后打开黑域就可以正常使用了，一键补丁可以卸载。 ![黑域阻止运行](https://ooo.0o0.ooo/2017/03/01/58b63b9bc226d.jpg)

### 发烧友

Android 发烧友当然自备 ADB，如果没有 ADB 的同学可以到[这个地址](http://adbshell.com/downloads)下载。ADB 的使用方法[请看此帖](http://jingyan.baidu.com/article/60ccbceb634e2364cab197c6.html)。 同样开启开发者模式中的 USB 调试功能，然后进入 ADB Shell，输入：

adb -d shell /data/app/me.piebridge.brevent-2/lib/arm/libbootstrap.so

大功告成。 如果在使用 ADB 的过程中出现各种问题，请善用搜索， ADB 这个东西是一劳永逸的，喜欢刷机的同学总能用得上。 对了，黑域支持 Android 6.0 - Android 7.1，现在的设备基本上都存在在这个区间内，配合绿色守护一起使用更是如虎添翼，如果在使用中遇到问题请直接到[作者 Github](https://github.com/liudongmiao/Brevent/issues) 留言解决。 2018年3月3日更新：其实也还可以试试[黑白门](https://www.jubuzz.com/geek/601.html)。