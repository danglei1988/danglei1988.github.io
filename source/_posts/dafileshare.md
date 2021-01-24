---
title: macOS 下传输文件到手机的神器
tags:
  - DaFileShare
  - macOS
id: '1829'
categories:
  - - 工作&amp;效率
date: 2020-11-22 14:10:01
---

之前介绍过一些从手机传输文件到电脑的各种神器，如[文叔叔](https://www.jubuzz.com/geek/efficiency/1772.html)、[空投](https://www.jubuzz.com/geek/efficiency/1802.html)等，今天来个逆向的，从 macOS 传输文件到 iOS 和 Android 设备，所用到的神器是来自大佬 deskangel 的 [DaFileShare](https://github.com/deskangel/DaFileShare/releases)。

## DaFileShare

桌面端的朋友可以直接点击上段末的链接进入 Github 进行下载，打不开 Github 的朋友可以试试[菊部的分享盘](http://share.jubuzz.com/file/18034009-472366651)，公号“十点神器”的朋友请直接回复“DFS”获得下载地址（但是最终还是要传到桌面端）。 DaFileShare 的原理是在本地环境下做了一个 http 服务器，通过局域网的其他设备的浏览器扫码就可以下载这个文件，软件非常的轻量级，只有 5.6M 大小，解压到“应用程序”中就可以直接使用。 DaFileShare 主要用来从 Mac 向手机传输文件，最方便的地方在于，Android 或者 iPhone 手机端无需下载任何App，通过浏览器就可以直接接收 macOS 传输过来的文件。 在 macOS 中打开 DaFileShare。 [![打开传输界面](https://images.jubuzz.com/uPic/0H78uQ.png)](https://images.jubuzz.com/uPic/0H78uQ.png) 把文件拖动到对话框中即可，这里我们用上图直接进行测试。 [![将文件拖入](https://images.jubuzz.com/uPic/jrkmUD.png)](https://images.jubuzz.com/uPic/jrkmUD.png) 拖入后会产生一个二维码，当然，这里不光是可以拖入图片，还可以拖入压缩包等各种形式的文件，因为主要依赖局域网进行传输，所以速度还是相当快的。 [![用手机扫码下载](https://images.jubuzz.com/uPic/0VSI1G.jpeg)](https://images.jubuzz.com/uPic/0VSI1G.jpeg) 这里用手机扫码下载，使用的是微信，但是实际的操作过程中间，建议大家不要使用微信，因为无论是 iPhone 还是 Android，微信保存后的文件很难找，现代智能手机的相机基本上都可以直接扫码，或者主流浏览器都具备直接扫码的功能，这里我墙裂推荐使用夸克浏览器，旦用难回。 另外 DaFileShare 的作者还提供了 Android 版本，此处不再进行测试，有兴趣的朋友可以试试。