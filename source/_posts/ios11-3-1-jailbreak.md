---
title: iOS11.3.1越狱 Electra 正式发布，附教程
tags:
  - iOS11
  - 越狱
id: '940'
categories:
  - - 日常&amp;搞机
date: 2018-07-07 16:47:21
---

之前菊座的 iPhone SE 一直停留在 iOS10.2，但是 Apple 一直想尽办法让我们升级，其中用了一些比较极端的手段，比方说有些 App 只有在 iOS+ 才能使用，这就十分蛋疼了。于是某天实在受不了升级了 iOS11，然后一路升级到现在的 iOS11.4，使用起来各方面都还好，不过就是屏幕太小，没手势，home 键按得实在难受。 扯远了，今天说的东西跟 iOS11.4没有任何关系，而是知名越狱开发者 Coolstar 为我们带来了 iOS11.3.1的 Electra 越狱。 ![越狱](https://www.jubuzz.com/wp-content/uploads/2017/08/cydia-1-1-1.jpg)

## iOS11.3.1越狱

首先是 Electra 的[iOS11.3.1越狱工具官网下载地址](https://coolstar.org/electra/)，另外iOS11.0-iOS11.1.2的越狱工具地址[在此](https://coolstar.org/electra1112)。 ![Electra 越狱](https://i.loli.net/2018/07/07/5b407de28695a.png) 有开发者账号的请点击 Dev Account 进行下载，没有的话点另一个。 此次的 Electra 越狱支持所有从 iOS11.2 到 iOS11.3.1的 Apple 设备（包含 iPhone、iPad、iPod Touch 等）。 具体的 Electra 越狱说明如下（洋文）：

*   On iOS 11.3-11.3.1, the device will reboot twice and Electra will need to be re-run after the first reboot
*   An APFS snapshot is created of / so you may revert it at a later date if needed
*   It is recommended to futurerestore if you have blobs before running Electra to ensure the best possible installation
*   Cydia is included
*   OpenSSH is running on port 22
*   Electra repo added by default
*   Substitute, Tweak Loader and Substrate Compatibility Layer available from Electra repo
*   Many packages need to be updated for both Electra and iOS 11 (make sure they're updated before installing as they may not work yet)
*   RocketBootstrap 1.0.6 or higher is required for use on iOS 11
*   Many apps, launch daemons and installation binaries are broken as they require entitlements to be added

菊座赶鸭子上架，试翻一下：

*   iOS 11.3-11.3.1越狱过程中可能重启两次，第一次重启之后需要重新运行 Electra；
*   过程中会在根目录创建 APFS 快照，以便可能的恢复作用；
*   建议提前备份 blobs 以免悲剧；
*   内含 Cydia，OpenSSH 需要22端口运行；
*   默认添加 Electra 源，Substitute, Tweak Loader 和 Substrate Compatibility Layer 可以在 Electra 源下载；
*   iOS11需要运行 RocketBootstrap 1.0.6及以上版本；
*   未添加配置文件可能导致应用等崩溃。

## iOS11.3.1越狱教程

1.  下载Electra最新的越狱IPA文件，放在电脑桌面上
2.  下载Cydia Impactor
3.  将iPhone/iPad/iPod等与电脑连接，如果iTunes启动，直接关闭即可。
4.  运行Cydia Impactaor，拖入Electra1131 IPA文件
5.  当Cydia Impactaor要求输入Apple ID时，尽管做就是了，已经被无数次验证这是安全的。
6.  这时设备主屏上出现安装成功的Electra越狱APP。进入设置-通用-描述文件与设备管理，找到描述文件并点击信任。
7.  将iOS调至飞行模式，随后运行Electra越狱APP，并点击“Jailbreak”按钮，直到看见主屏上出现Cydia，即可关闭飞行模式，代表越狱成功。

因为菊座手上没有 iOS11.3.1的机器，所以这里就不做测试了，希望有机子的朋友测试下，如果遇到问题可以到威锋求助。