---
layout: post
title: 天珩全字库外挂补全模块
categories: Magisk模块
description: 利用模块和自己修改的 fonts.xml 实现全 Unicode 字符的同台显示和处理，达到补全手机字库的目的。
keywords: Magisk模块, 字体, 天珩全字库
---

为使已 root 的 Android 手机实现全 Unicode 字符的同台显示和处理，方便 Magisk 用户使用，特制作此外挂模块，不过囿于本人技术水平，部分操作仍然需要用户手动进行 *（如修改 fonts.xml 文件）*，如有更便捷的方法，欢迎分享。

## 模块简介

在叶典网的下载页面，可以看到一个名叫[**「天珩全字库」**]((http://cheonhyeong.com/Simplified/download.html))的字体支持包，号称「**字符数量最全**的字体支持包」，是一款非盈利的、学习研究型的字库，目的是为了汉字等字符的显示，不制作或出售任何商业作品。目前天珩全字库已经更新到了 3.0.0，支持 14 余万汉字，并支持 **Unicode 13.0** 以内的所有字符，包括 CJK 扩展 G 区汉字，如「𰻝𰻝面」的「𰻝（biáng）」字。

*（Biang 字的简体「𰻝」的 Unicode 码位为 U+30EDD，繁体「𰻞」为 U+30EDE。）*

很多关注我公众号的用户都在用 Magisk 模块的方式替换系统字体，因为它不直接改变系统文件，也可以随意刷入和卸载，比以往的 ROOT 直接替换和卡刷包替换更加方便。在酷安上已有人分享了内置天珩全字库的字体模块，以支持 Unicode 范围内所有字符的显示，但是这样会增加模块的体积。由此，作者分享了这款**「天珩全字库」外挂模块**，实现在系统字体文件夹 `\system\fonts` 内加入 [天珩全字库](http://cheonhyeong.com/Simplified/download.html) 0、1、2 平面字体，配合修改好的 fonts.xml *（需要自己修改）* ，实现全 Unicode 字符的同台显示和处理，达到补全手机字库的目的。

## 使用前要做的修改

使用前，需检查所搭配的字体模块的 **\system\etc\fonts.xml** 文件是否有以下语句：

```xml
    <family>
        <font weight="400" style="normal">TH-Tshyn-P0.ttf</font>
    </family>
    <family>
        <font weight="400" style="normal">TH-Tshyn-P1.ttf</font>
    </family>
    <family>
        <font weight="400" style="normal">TH-Tshyn-P2.ttf</font>
    </family>
```

如果没有，请在文件末尾`</familyset>`的前一行加上以上内容。保存后，将修改后的模块与本模块一同刷入，重启，即可实现补全手机字库的目的。

如果需要让系统默认字体也支持天珩全字库，则可在手机的 **\system\etc\fonts.xml** 文件上按照上面的提示修改，前提是该手机已 ROOT，并已解锁 System 分区。

以上方法适用于 Android 7.0 及以上版本的 Android，对于 Android 5.0～6.0 的用户，可参考知乎文章：[「下载并安装使用超大字库的具体步骤」](https://zhuanlan.zhihu.com/p/26524450)。

## 模块下载

 [蓝奏云，密码 alwh](https://lxgw.lanzoui.com/b0cq9ltjc) 

Magisk 目标支持版本 20.4，最低支持 19.0 版本的 Magisk。

## 注意与声明

- 请按照提示仔细修改字体模块的 fonts.xml 文件，如果是氢 11 系统还需要修改 fonts_base.xml 文件，因修改文件造成的手机故障本人概不负责。
- 请勿将本模块用于商业用途。

## 字体来源

天珩全字库由 [沈天珩](http://cheonhyeong.com/Simplified.html) 整理制作。

> 本字库属于非盈利的、学习研究型的字库，目的是为了汉字等字符的显示，不制作或出售任何商业作品。字形版权：中易、华康、Iwata、Besta、方正。本字库中字体的字形均为上述公司制作，非本软件作者制作。本字库的字体属于已经公开的字体，故本字库仅仅起到收集整理的作用，方便用户使用。作者并未对字体做出任何有意义的改动，若有任何人以本字库的名义收取任何费用，本字库作者不承担任何连带责任。

## 模块作者

- 微信公众号：霞鹜（lxgwshare）
- 微博：[孤鹜先森](https://weibo.com/lxgw/)
- 酷安/少数派：[落霞孤鹜lxgw](https://coolapk.com/u/633884)
- 酷安看看号：孤鹜字体
