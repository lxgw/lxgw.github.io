---
layout: post
title: 为 Klee 试制简化字（持续更新，多图预警）
categories: 业余字体设计 开源中文字体
description: 为 FONTWORKS 的开源字体 Klee One 制作简化字。
keywords: Klee, 补字, 简化字
---

前段时间，日本著名字体厂商 FONTWORKS 在 GitHub 上释出了 [7 款开源日文字体](https://github.com/fontworks-fonts)，分别为 **Train、Klee、Stick、Rock-n-Roll、Reggae、Rampart 和 DotGothic16。**7 款开源日文字体各有各的特点，其中我最感兴趣的，当属 [Klee](https://github.com/fontworks-fonts/Klee)。

![Klee 样张](https://github.com/fontworks-fonts/Klee/raw/master/image_Klee-SemiBold.png)

> FONTWORKS 公司出品过很多以西方艺术家名字为代号的字体，比如之前分享过的 Seurat、Rodin、Cezzane 等。这款字体的名字叫 Klee，是以德裔瑞士籍画家保罗•克利（Paul Klee，1879-1940）命名的。这款字体是一款日式的教科书字体（日本小学教科书的标准书写字体，相当于我们的规范楷书）。原版只有 Medium 和 Semibold 两个字重，为 Pro 字集，含有近 8000 个汉字。
>
> <div align="right">——摘自公众号「霞鹜」（ID:lxgwshare）

[字体详细介绍（官网，日语）](https://fontworks.co.jp/fontsearch/KleePro-M/) 

## 初衷

这是一款本人非常喜欢的字体，有着日本教科书体的写法，兼有仿宋和楷体的特点，可读性高。宁静之雨、字由心雨等大佬曾先后用**仿宋、刻本仿宋、仓耳今楷**补全这款字体，做为手机系统的美化字体移稙在 iOS、Android 等手机系统中，受到很多机友的欢迎。

不过这样补全的字体有一些不足之处。 **第一**，原有字体和后补字体之间有着一定的差异，致使一些不同的文字（如 Klee 原有汉字与后补简体字）混排之后会有违和感。 **第二**，由于补字所用的字体（如刻本仿宋、仓耳今楷等）为商业版权字体，补全之后不可用于商业用途，还会有侵权的风险。

鉴于此，本人开始了为 Klee 这一高质量的日文字体补全简体字的尝试。选取**较粗的 SemiBold 字重**，截至 2021.02.03，已造了**1650 个字**，已基本补完原字体（Klee One）所含繁体字对应的简体字。部分字稿如下图所示，持续更新。补全后的字体拟命名**「霞鹜文楷」**。

## 字稿

![](\images\posts\klee-simpchin\wenkai-overview.png)

### 截至 2021.1.30 的所有新造汉字

![](\images\posts\klee-simpchin\wenkai-demo.png)

[PDF 格式](https://github.com/lxgw/LxgwWenKai/raw/main/demo.pdf)

### 2021.1.31 后的新造汉字

#### 2021.01.31

![](\images\posts\klee-simpchin\wenkai-20210131.png)

#### 2021.02.01

![](\images\posts\klee-simpchin\wenkai-20210201.png)

#### 2021.02.02

![](\images\posts\klee-simpchin\wenkai-20210202-1.png)

![](\images\posts\klee-simpchin\wenkai-20210202-2.png)

#### 2021.02.03



### 部分字稿

- Unicode 编码靠前的简体字

  ![](\images\posts\klee-simpchin\klee-simpchin-single.png)

- 「亻」旁

  ![](\images\posts\klee-simpchin\klee-simpchin-person.png)

- 「纟」旁

  ![](\images\posts\klee-simpchin\klee-simpchin-silk.png)

- 「讠」旁

  ![](\images\posts\klee-simpchin\klee-simpchin-language.jpeg)

- 「钅」旁

  ![](\images\posts\klee-simpchin\klee-simpchin-metal.png)
  
- 「贝」部和「车」部 *（贝字旁需要重做了![](https://img.t.sinajs.cn/t4/appstyle/expression/ext/normal/a1/2018new_doge02_org.png)）*

  ![](\images\posts\klee-simpchin\klee-simpchin-finance-traffic.png)

## 一些操作 & 后记

由于要补的字多为简体字，而原字体里没有相应部件，所以需要**拆笔画**。比如「车」字旁，原字体里没有简体的车字旁，就需要从别的字里用切割轮廓工具拆出「㇐」「㇜」「㇑」「㇀」这四个笔画进行拼接，缩放后还要用到加粗/减细命令。调整字形的结构，有时也需要拆笔画。**用 FontCreator 拆笔画是一件烦琐且耗时的事情。**

![](\images\posts\klee-simpchin\tzay.png)

补字过程中，大多数汉字没有参照其它已有字体，全凭自己的感觉，只有少数汉字参考了**仓耳今楷**，也可以说是**「临摹」**，比如「辇」字。

![](\images\posts\klee-simpchin\nean.png)

下图左边的「辇」字是凭自己的感觉拼的，右边的「辇」字是参照仓耳今楷拼的。对比起来，右边的「辇」比左边的「辇」协调了很多。

![](\images\posts\klee-simpchin\nean-comparison.png)

由于不是专业的字体设计师，有些字基本上是直接替换偏旁，还有很多结构比例不协调的地方，还请大佬轻喷。

感谢 FONTWORKS 以及 Klee 字体的设计师，提供了这么高品质的开源字体。

**在这里想知道还有哪个字库公司或者设计师想要补全 Klee 这款字体，如果已经有人开始补了，我就不用费这个工夫了。**![喵喵](https://img.t.sinajs.cn/t4/appstyle/expression/ext/normal/7b/2018new_miaomiao_org.png)



*（感觉这篇文章有一点卖弄的成分![](https://img.t.sinajs.cn/t4/appstyle/expression/ext/normal/a1/2018new_doge02_org.png)）*

---

## 后续

没想到有人把这些字稿转发到 Facebook 上了，居然引来了大佬们的讨论。

![](\images\posts\klee-simpchin\fb-snapshot.jpg)

![](\images\posts\klee-simpchin\fb-comment.jpg)

Francis Chow 是 Klee 系列字体的原作者，居然认为我补的简体字达到了合格水平，受宠若惊……（

此外很多人感觉补的字有点怪，我个人总结了一些原因：

1. 简体字里面有很多**草书楷化字**，如**「专车东乐练买卖贝见页」**等 *（对应繁体字「專車東樂練買賣貝見頁」）* ，虽然这些简体字的笔画比繁体字少了很多，但比繁体字**更难设计**。
2. 补字过程中很多字都是直接**将繁体字的偏旁替换成简体字的偏旁** *（如「車」→「车」、「金」→「钅」）*，容易造成字形**结构比例失衡**。

此时明白了字体设计工作是有多么的不容易。

## 演示版字体下载

[点击此处](https://github.com/lxgw/LxgwWenKai/)进入霞鹜文楷项目页面，下载 DEMO 版字体文件。预计将在除夕放出完整版字体文件，将覆盖 3500 + 4808 简繁常用字。