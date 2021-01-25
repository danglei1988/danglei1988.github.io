---
title: Windows10字体设置或恢复还原
tags:
  - Windows10
  - 字体
id: '1889'
categories:
  - - 日常&amp;搞机
description: Windows10恢复默认字体远远没有Windows7简单。
date: 2021-01-23 21:14:40
---

最近因为一直在玩《新仙剑奇侠传XP重制版》（想起才玩，速度非常慢），加上自己喜欢折腾系统，导致**Windows10的字体**总是有问题，总结起来有两个大问题：

1.  《新仙剑奇侠传》繁体状态下字体显示不正常；
2.  Windows10添加或修改字体后不知怎么还原

现在已经解决了，爬了不少搜索，不过好像都没有什么特别有效的方案，就势分享一下。

## 《新仙剑奇侠传XP版》繁体字体显示不正常解决方法

打开Windows10的“设置-应用和功能-可选功能-添加功能-中文（繁体）的补充字体”，然后重启就可以了。 切记一定要重启。 [![中文繁体补充字体](https://images.jubuzz.com/PicGo/389016b75500e1a59d3ee77529170098-5ed7fa.png)](https://images.jubuzz.com/PicGo/389016b75500e1a59d3ee77529170098-5ed7fa.png)

## Windows10设置字体或恢复默认字体

试了百度得出的好多注册表或者“C:/Windows/Fonts”文件夹等设置办法，均无效，最后是被一个Github淘来的35KB的小软件解决了。 软件名字叫Windows-Font-Changer，Github地址[在此](https://github.com/alcortazzo/Windows-Font-Changer)，打不开Github请到[菊部的城通盘](http://share.jubuzz.com/f/18034009-479698045-d4be8a)下载，提取码jubuzz，公众号“十点神器”的朋友直接回复“**改字体**”获得。 ![设置Windows10字体](https://images.jubuzz.com/PicGo/934259e01ebfe68872c58821c8336761-0c4965.png) 左侧为设置自定义字体，右侧为设置默认字体，鼠标可以直接点击具体的版块来替换。 ![恢复Windows10默认字体](https://images.jubuzz.com/PicGo/da9d8cfd2e31254e55747d82d701f8ca-bd7459.png) 恢复Windows10默认微软雅黑的话点击右侧即可，然后关闭，重启。