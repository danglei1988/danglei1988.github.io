---
title: Vultr 降价，何不用它来搭个 SS
tags: []
id: '147'
categories:
  - - 日常&amp;搞机
date: 2017-03-03 10:56:58
---

昨天惊奇地发现 Vultr 降价了，居然出现了 2.5 刀/月的服务器，惊叹之余，不禁赶紧开了一台测试SS压压惊，顺便也分享一下**在 Vultr 上搭建 Shadowsocks 的方法**。

## Vultr 简介

国际惯例 [Vultr 官网](https://www.vultr.com/?ref=7968869-4F)，自带小尾巴，租用服务器的话你也赠送我也赠送，不喜请去掉，注册没影响。 先说说 Vultr 是什么，可惜都没有百科，只好自己搜集点内容编辑一下： Vultr 是一家成立于 2014 年的 VPS 提供商，Vultr 家的服务器采用的 E3 的 CPU，清一色的 Intel 的 SSD 硬盘， Vultr 的计费按照使用计费（自行选择配置、可以按月或按小时计费），用多少算多少，可以随时取消， Vultr 的服务器托管在全球 14 个数据中心，即时开通使用。堪称是拥有最多机房的 VPS 服务商。大陆访问日本机房速度不错，延迟低、带宽足。其次西海岸洛杉矶的节点访问也很好，而且流量比东京要多得多。 ![Vultr](https://ooo.0o0.ooo/2017/03/03/58b8d0185aa14.jpg) 以上是摘自不同地方的 Vultr 简介，其中有些数据已经过时，比如说数据中心刚才我数了下，总共有 18 个，那个 Intel 的处理器估计也升级了。 总之，这个博客目前就是放在 Vultr 的服务器上，不过只是搭了个 WordPress，用的是当时最低 5 美元/月的服务器，这不最近出了 2.5 美元的，又想换了。 值得说明的是 Vultr VPS 的租用需要使用外币信用卡（VISA or Master）或 Paypal，国内的朋友可以使用某宝代购，如果长期用的话，建议自己申请一个信用卡，我自己是当时在招行申请的，速度也很快。（更加值得说明的是，Vultr 现已支持支付宝和微信付款）

## 注册租用 Vultr VPS

注册我就不多废话了，英文也很简单。 注册过后点击右上角加号“Deploy New Server”，基本上只需要选择系统版本、服务器位置、服务器类型就 OK ，其他的都不需要填写，自建 SS 的话建议 2.5 刀一个月的足矣，然后点击 “Deploy Now” 就行了。 ![申请 Vultr VPS](https://ooo.0o0.ooo/2017/03/03/58b8d356bd8c7.png) 如图所示，我选择的是 Vultr 的 Japan 节点，选择 2.5 刀的配置， Ubuntu 的服务器，大家都可以按照自己的喜好来配，网上都说洛杉矶的好，但实际感觉我觉得日本东京的也还行，那么既然如此，后面的内容我们就以新加坡节点的为例来进行...

## 利用 Vultr VPS 搭建 Shadowsocks

建立服务器后，点进 “Manage” 界面，里面会有 IP 和密码，下载一个 [Putty](https://www.baidu.com/s?wd=putty) ，后面会有用。 ![操作 Vultr VPS](https://ooo.0o0.ooo/2017/03/03/58b8d3fbe9f2f.png) \[caption id="" align="aligncenter" width="1237"\]![查看 Vultr VPS 密码](https://ooo.0o0.ooo/2017/03/03/58b8d4934adf8.png) 查看 Vultr VPS 密码\[/caption\] 然后以上图表示的 IP 和密码使用 Putty 登陆 VPS ，注意 Putty 中使用右键是可以直接复制内容的，不同的系统欢迎内容也不一样，下面是 Ubuntu 14 的欢迎语。 ![登陆 VPS](https://ooo.0o0.ooo/2017/03/03/58b8d4bc857e2.png) 然后输入如下字段，可复制用右键粘贴进 Putty。

wget --no-check-certificate https://raw.githubusercontent.com/teddysun/shadowsocks\_install/master/shadowsocks.sh

chmod +x shadowsocks.sh

./shadowsocks.sh 2>&1  tee shadowsocks.log

然后就会出现下面的提示要输入 Shadowsocks 的密码，请自行输入即可，对了，源码来自 Github，应该是博主[秋水逸冰](https://teddysun.com/)的作品，在此表示感谢。 ![输入 Shadowsocks 密码](https://ooo.0o0.ooo/2017/03/03/58b8d59714d98.png) 端口我不太懂，我是随便填的，结果可以用。 ![填写 Shadowsocks 端口](https://ooo.0o0.ooo/2017/03/03/58b8d7256081b.png) 然后随便按个键就可以安装，成功后会提示。 ![Vultr VPS 安装 Shadowsocks 成功](https://ooo.0o0.ooo/2017/03/03/58b8d7ab1e221.png) 上面的数据大家就不需要测试了，因为在测试完这些操作后，我已经撤销那台机器了... 以上是用 Python 来安装 VPS 端的 Shadowsocks，接下来我们应该在自己的电脑上安装 Shadowsocks 了，已有的同学请自行忽略此步。 PC Shadowsocks 的官方地址应该在[这里](https://github.com/shadowsocks/shadowsocks-windows/releases)，其他的版本可以在[这里](https://github.com/shadowsocks)查看。 安装过程中可能需要 .Net 支持，直接到微软官方下载即可。 这里以桌面端的 Shadowsocks 为例，填上上面获取到的信息，本地的端口可以默认。 ![新增 Shadowsocks 服务器](https://ooo.0o0.ooo/2017/03/03/58b8da5206e4c.png) 确定后打开 SS ，就可以畅游了，建议选用 PAC 模式，避免国内网站速度慢和流量损失。 ![测试自建的 Shadowsocks](https://ooo.0o0.ooo/2017/03/03/58b8dc84a0952.png) 亲测新加坡的也可以看 480P，感觉还行，国内的用户使用 Vultr 的话大家的一致意见是洛杉矶线路比较快。过几天弄个 BBR 再测试下。码字不易，希望能给大家有所帮助，本文仅供交流学习之用，请勿用于其他用途，如需转载，请注明来自菊部制造。