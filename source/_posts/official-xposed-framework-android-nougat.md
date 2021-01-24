---
title: 支持Android7.0/7.1的官方Xposed框架发布
tags:
  - Android
  - Xposed
id: '475'
categories:
  - - 日常&amp;搞机
date: 2017-10-09 17:04:36
---

虽说Android8.0 Oreo已经发布，但是估计国内还有不少机器停留在Android7.0/7.1，以前菊部也总是吐槽Xposed迟迟没有适配Nougat，之前分享过一个[非官方版本的Xposed](https://www.jubuzz.com/geek/350.html)，现在**官方的Android7.0/7.1 Xposed框架**总算来了。

## 下载官方Android7.0/7.1 Xposed框架

洋文比较好的同学可以到XDA的相关帖子下载最新的**Xposed Installer 3.1.2**即可（写此文的时候我搜了一下，酷安貌似还没有，可能在路上）。 ![下载适用于Android7.0/7.1的Xposed框架](https://s1.ax2x.com/2017/10/09/9ZU1Q.png) 看句子有困难，能认识拉丁字母的同学可以到[Xposed的官方下载FTP](http://dl-xda.xposed.info/framework/)对号入座： ![Xposed官方下载FTP](https://s1.ax2x.com/2017/10/09/9ZKo2.png) 如图所示，SDK24即为Android7.0，同理SDK25为Android7.1，亲测这个下载站国内直连速度还不错。 选择完系统版本之后需要选择CPU类型，是arm、arm64还是X86，这一点不太清楚的话可以到对应机型的贴吧问下。 然后就可以下载zip包了。 刷入zip包的方式与刷入第三方ROM包的操作基本一致，直接套用即可，如果不太清楚的话可以参考[这篇文章](http://jingyan.baidu.com/article/154b4631611cc028ca8f41df.html)。 至于为什么要用Xposed框架，可以看看下面的部分Xposed模块图，图片来自酷安。 ![部分Xposed模块](https://s1.ax2x.com/2017/10/09/9ZAda.png) 安装过Xposed后，还有成千上万的模块供你使用。 如果对Xposed一无所知，但又想使用的朋友可以看看[这篇文章](https://sspai.com/post/24538)，感谢少数派。