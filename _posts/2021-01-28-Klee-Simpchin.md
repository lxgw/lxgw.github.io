---
layout: post
title: 为 Klee 试制简化字（持续更新）
categories: 业余字体设计 开源中文字体
description: 为 FONTWORKS 的开源字体 Klee One 制作简化字。
keywords: Klee, 补字, 简化字
---

前段时间，日本著名字体厂商 FONTWORKS 在 GitHub 上释出了 [7 款开源日文字体](https://github.com/fontworks-fonts)，分别为 Train、Klee、Stick、Rock-n-Roll、Reggae、Rampart 和 DotGothic16。7 款开源日文字体各有各的特点，其中我最感兴趣的，当属 [Klee](https://github.com/fontworks-fonts/Klee)。

![Klee 样张](https://github.com/fontworks-fonts/Klee/raw/master/image_Klee-SemiBold.png)

> FONTWORKS 公司出品过很多以西方艺术家名字为代号的字体，比如之前分享过的 Seurat、Rodin、Cezzane 等。这款字体的名字叫 Klee，是以德裔瑞士籍画家保罗•克利（Paul Klee，1879-1940）命名的。这款字体是一款日式的教科书字体（日本小学教科书的标准书写字体，相当于我们的规范楷书）。原版只有 Medium 和 Semibold 两个字重，为 Pro 字集，含有近 8000 个汉字。
>
> <div align="right">——摘自公众号「霞鹜」（ID:lxgwshare）

[字体详细介绍（官网，日语）](https://fontworks.co.jp/fontsearch/KleePro-M/) 

这是一款本人非常喜欢的字体，有着日本教科书体的写法，兼有仿宋和楷体的特点，可读性高。宁静之雨、字由心雨等大佬曾先后用**仿宋、刻本仿宋、仓耳今楷**补全这款字体，做为手机系统的美化字体移稙在 iOS、Android 等手机系统中，受到很多机友的欢迎。

不过这样补全的字体有一些不足之处。 **第一**，原有字体和后补字体之间有着一定的差异，致使一些不同的文字（如 Klee 原有汉字与后补简体字）混排之后会有违和感。 **第二**，由于补字所用的字体（如刻本仿宋、仓耳今楷等）为商业版权字体，补全之后不可用于商业用途，还会有侵权的风险。

鉴于此，本人开始了为 Klee 这一高质量的日文字体补全简体字的尝试。选取**较粗的 SemiBold 字重**，目前已造了**近 500 个字**。部分字稿如下图所示，持续更新。

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
  
- 「贝」部和「车」部

  ![](\images\posts\klee-simpchin\klee-simpchin-finance-traffic.png)

由于要补的字多为简体字，而原字体里没有相应部件，所以需要**拆笔画**。比如「车」字旁，原字体里没有简体的车字旁，就需要从别的字里用切割轮廓工具拆出「㇐」「㇜」「㇑」「㇀」这四个笔画进行拼接，缩放后还要用到加粗/减细命令。调整字形的结构，有时也需要拆笔画。**用 FontCreator 拆笔画是一件烦琐且耗时的事情。*

![](\images\posts\klee-simpchin\tzay.png)

补字过程中，大多数汉字没有参照其它已有字体，全凭自己的感觉，只有少数汉字参考了**仓耳今楷**，也可以说是**「临摹」**，比如「辇」字。

![](\images\posts\klee-simpchin\nean.png)

下图左边的「辇」字是凭自己的感觉拼的，右边的「辇」字是参照仓耳今楷拼的。对比起来，右边的「辇」比左边的「辇」协调了很多。

![](\images\posts\klee-simpchin\nean-comparison.png)

由于不是专业的字体设计师，还有很多结构不协调的地方，还请大佬轻喷。

**在这里想知道还有哪个字库公司或者设计师想要补全 Klee 这款字体，如果已经有人开始补了，我就不用费这个工夫了。**![喵喵](https://img.t.sinajs.cn/t4/appstyle/expression/ext/normal/7b/2018new_miaomiao_org.png)



*（感觉这篇文章有一点卖弄的成分![](https://img.t.sinajs.cn/t4/appstyle/expression/ext/normal/a1/2018new_doge02_org.png)）*