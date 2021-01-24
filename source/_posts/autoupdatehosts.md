---
title: AutoUpdateHosts，你的PC也可以一键更换hosts
tags:
  - AutoUpdateHosts
  - hosts
  - 科学上网
id: '282'
categories:
  - - 日常&amp;搞机
date: 2017-04-17 11:28:16
---

最近正值刷了Android7.1.2，[Go Hosts](https://www.jubuzz.com/geek/19.html)用得风生水起，可是平时在PC上的时候还是有些依赖Shadowsocks，总是开啊关的，挺麻烦的，于是就搜了下，搜到了这个**AutoUpdateHosts**，一定程度上可以解决正常需求。

## AutoUpdateHosts简介及使用

AutoUpdateHosts是Github作者[morgengc](https://github.com/morgengc)的作品，是一款一键下载、更新Windows Hosts的文件，用于常见网络访问，目前**只有64位版本**。 AutoUpdateHosts的hosts文件来源于[此地址](https://github.com/racaljk/hosts)，作者基于 CC BY-NC-SA 4.0协议发布，有需要的朋友可以按照本文后面的操作直接用hosts进行替换。

### AutoUpdateHosts怎么下载怎么用？

下载可以到[Github](https://github.com/morgengc/AutoUpdateHosts)直接打包Zip，没有Github使用经验的朋友也可以直接到我分享的[网盘地址](https://pan.baidu.com/s/1eSadBI6)下载，密码7red。 使用方法也很简单，下载后直接解压，然后打开解压后的文件夹，右键“以管理员身份运行”即可，其他的部分软件会自动运行。 ![如何使用AutoUpdateHosts](https://ooo.0o0.ooo/2017/04/17/58f4331c6e67e.png) 然后就可以打开你的浏览器查看结果了。 ![用AutoUpdateHosts上Facebook](https://ooo.0o0.ooo/2017/04/17/58f43417338e7.png)

## 如何直接在电脑上替换Hosts

首先找到Windows中的hosts文件位置，一般在系统盘:\\Windows\\System32\\drivers\\etc\\hosts，用记事本打开（或用各种Notepad++等第三方高级记事本软件），替换[这个地址](https://github.com/racaljk/hosts)中下载的hosts文件内容进去保存即可。 ![找到Windows中的hosts文件位置](https://ooo.0o0.ooo/2017/04/17/58f434a7c8ac1.jpg) 好了，Android和PC都可以一步到位的一键更新hosts来实现科学上网了，本文仅供交流学习之用，请勿用于其他用途，请各位低调使用。 2017年4月19日更新：Android下的[BypassGeo](https://www.jubuzz.com/geek/291.html)也可以用来一键科学上网。