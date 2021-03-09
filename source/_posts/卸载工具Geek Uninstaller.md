---
title: 可能是最简单暴力的卸载工具Geek Uninstaller
categories: tech
keywords: 'Windows,软件,卸载'
description: 卸载个QQ游戏，居然把我有关联的QQ等其他软件快捷方式也清理掉了
date: '2021/3/8 23:22:49'
cover: https://images.jubuzz.com/PicGo/4e35f37fe71f97873b1225ec2e5ebabc-994983.jpg
---

昨天分享了一个[Glary Utilities Pro](https://www.jubuzz.com/tech/33556528.html)，可能是Windows平台最为全面强大的优化工具，在谈到功能概览的时候，看到里面有软件卸载的相关功能，但是对于卸载，我们总是担心不够干净不够彻底，刚好最近发现了一款用于Windows平台的比较小巧暴力的卸载软件**Geek Uninstaller**，今天分享出来。

Geek Uninstaller一路从Windows XP支持到Windows10，作为一款免费软件，非常良心，但是同样非常遗憾的是软件自从2019年9月11日后就没再更新过了，最终的版本号是1.4.7.142，不过我自己一直在用，也没察觉到有什么异样。

简单介绍一下。

简单在官网下载Free版本的zip压缩包即可，只有2.52MB，解压后也只有1个exe文件，大小6MB，非常小巧，并且即便是把它当做一个快捷方式放在桌面上来用，也不会产生其他的临时文件或软件日志。

![Geek Uninstaller](https://images.jubuzz.com/PicGo/cecca3f8789c5dec23567a652ab74744-781308.png)

但是如果你因为其身型小巧就此认为它是个软蛋，那就错了。打开是常规的软件列表界面，于Windows设置自带的应用卸载无异，也含有Windows各种运行库，可随意卸载。

![过于奥利给了](https://images.jubuzz.com/PicGo/0070c2b9b149aaa908bee0e81c181be3-0592b4.png)

列表点击具体软件右键选择下载后，会弹出软件自带的卸载程序，这里以QQ游戏为例，因为我安装了它之后实在是打开次数太少，不如删掉。

常规默认卸载过后会自动呼出一个强制扫描，从上图完全可以看到，Geek Uninstaller在扫描残留信息的时候，把微信、QQ和软件管理独立版的快捷方式和开始菜单也扫描出来了，我知道选定后可能会造成这些软件快捷方式的丢失，但是我还是尝试了一下。

果然。

费了好大劲把这些软件的快捷方式重新拖回桌面后，我不禁思考：为什么会这样？

难道是因为名字相近？不对，“微信”这俩字和QQ游戏完全无关；难道是它们和QQ游戏之间有暗藏的钩子关系？有可能，不过作为小白，咱也不敢肯定，不知道有没有大佬可以解答一下，毕竟其他非鹅厂的软件完全没有受到任何影响。

不过不管怎么说，Geek Uninstaller这种宁可错杀一千的态度我还是非常喜欢的。

当然，如果你也跟它一样暴力，也可以选择一开始就直接强制卸载。

![强制卸载Windows软件](https://images.jubuzz.com/PicGo/433cc8b49dc517c61bb72de9e8565a2f-5e2bed.png)

以上是我删除软件管理单文件版的相关内容，其实还是有注册表写入。

![批量卸载UWP应用](https://images.jubuzz.com/PicGo/49f46b7717ccc218cfed153e9d49526b-0e8e04.png)

除了常规的软件卸载外，针对Windows10，还可以卸载UWP应用，你懂的，现在再纯净再原版的Windows10系统，安装后微软也会给你内置一堆你用不上的东西，虽然直接开始菜单就能右键卸载，不过列表操作还是香一些。

官网[在此](https://geekuninstaller.com/)，“十点神器”的朋友回复“**极客卸载**”获取地址。