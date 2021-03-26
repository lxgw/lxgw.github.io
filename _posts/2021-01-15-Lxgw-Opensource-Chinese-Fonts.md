---
layout: post
title: 自制开源免费字体一览（截至 2021.2.6）
categories: 开源中文字体
description: 在原有开源字体基础上改造成的中文字体，可免费商用。
keywords: 字体, 开源字体, 中文字体, 免费商用字体
eye_catch: https://ae01.alicdn.com/kf/U4728f01b032645e0967831d3e623e5dbI.jpg
topmost: true
---

本文用于收录本人在原有开源字体基础上改造成的开源中文字体。其实如果严格一点来说，不能算「自制」，只能算「自改」。然而对这些开源字体，我也付出了很多时间和精力。本人发布的开源字体可在本文查看，也可以在右侧的开源项目目录中查找。

---

![](https://ae01.alicdn.com/kf/U4728f01b032645e0967831d3e623e5dbI.jpg)

## 自制免费字体一览

截至目前（2021.2.6），本人已改造并发布了 6 款开源中文字体，均为由开源日文字体转化。现将这 6 款字体列出如下。

| 字体                                                         | 授权方式                                                     | 风格                  | 发行时间 |
| ------------------------------------------------------------ | ------------------------------------------------------------ | --------------------- | -------- |
| [小赖字体 / Xiaolai ](https://github.com/lxgw/kose-font) ([猫啃](https://www.maoken.com/freefonts/4306.html)) | [SIL OFL](https://scripts.sil.org/OFL) ([汉译](https://www.maoken.com/ofl)) | 手写                  | 2020.5   |
| [悠哉字体 / Yozai](https://github.com/lxgw/yozai-font) ([猫啃](https://www.maoken.com/freefonts/5423.html)) | [SIL OFL](https://scripts.sil.org/OFL) ([汉译](https://www.maoken.com/ofl)) | 手写                  | 2020.6   |
| [霞鹜文楷 / LXGW WenKai ](https://github.com/lxgw/LxgwWenKai)([猫啃](https://www.maoken.com/freefonts/9704.html)) | [SIL OFL](https://scripts.sil.org/OFL) ([汉译](https://www.maoken.com/ofl)) | 楷体                  | 2021.2   |
| [霞鹜晰黑 / LXGW Clear Gothic](https://github.com/lxgw/LxgwClearGothic) ([猫啃](https://www.maoken.com/freefonts/8781.html)) | [IPA](https://moji.or.jp/ipafont/license/) ([汉译](https://www.maoken.com/ipa)) | 黑体 *（旧字形）*     | 2020.12  |
| [霞鹜新晰黑 / LXGW New Clear Gothic](https://github.com/lxgw/LxgwNewClearGothic) ([猫啃](https://www.maoken.com/freefonts/8999.html)) | [IPA](https://moji.or.jp/ipafont/license/) ([汉译](https://www.maoken.com/ipa)) | 黑体 *（大陆新字形）* | 2021.1   |
| [霞鹜漫黑 / LXGW Marker Gothic ](https://github.com/lxgw/LxgwMarkerGothic)([猫啃](https://www.maoken.com/freefonts/9523.html)) *<sup>未完成，已弃</sup>* | [SIL OFL](https://scripts.sil.org/OFL) ([汉译](https://www.maoken.com/ofl)) | POP                   | 2021.1   |

另有 3 款由思源黑体轻度改造的 **「975」系列字体**，由于做得不太好，就不在这里列出，可在 [「猫啃网」](https://www.maoken.com/?s=975) 搜索下载。

**<sup>DEMO</sup>** 表示为演示版字体，**<sup>BETA</sup>** 表示为测试版字体，仍有诸多不完善之处（如缺字，字型不规范等）。 

字体 7z 压缩包和 Magisk 模块可在 [个人网盘](http://lxgw.ys168.com) 下载，已上传前 5 个字体的 TTF 和 Magisk 模块。

## 字数等级参考

| 字体                                                     | 简体字数 | 繁体字数 | 参考字库                     |
| -------------------------------------------------------- | -------- | -------- | ---------------------------- |
| [小赖字体](https://github.com/lxgw/kose-font)            | ★★★★★    | ★★★★★    | GB18030+通规                 |
| [悠哉字体](https://github.com/lxgw/yozai-font)           | ★★★★★    | ★★★★★    | GB2312+通规+JIS+GB12345+BIG5 |
| [霞鹜晰黑](https://github.com/lxgw/LxgwClearGothic)      | ★★★★★    | ★★★★★    | GB2312+通规+JIS+GB12345+4808 |
| [霞鹜文楷](https://github.com/lxgw/LxgwWenKai)           | ★★★★★    | ★★★★☆    | GB2312+JIS+4808              |
| [霞鹜新晰黑](https://github.com/lxgw/LxgwNewClearGothic) | ★★★★★    | ☆☆☆☆☆    | GB2312+通规（仅简体）        |
| [霞鹜漫黑](https://github.com/lxgw/LxgwMarkerGothic)     | ★★★☆☆    | ★★★☆☆    | 3603+JIS                     |

**注释：**

1. GB 2312 共 6763 字（仅简体）， GB 18030 共 27533 字（简繁均有）。 GB 2312 含于 GB 18030。
2. GB 12345 是 GB 2312 对应繁体字符集，共 6866 字（包括 103 个「一简对多繁」扩充汉字）。
3. **3603** 指简体中文 3603 常用汉字，包括「现代汉语常用字表」（老 3500 字）及「义务教育语文课程常用字表」（新 3500 字，《通用规范汉字表》一级字表），新老 3500 加一起共 3603 个字（新老 3500 常用字有 103 个字不重合，详见[百度百科：现代汉语常用字表-相关比较](https://baike.baidu.com/item/%E7%8E%B0%E4%BB%A3%E6%B1%89%E8%AF%AD%E5%B8%B8%E7%94%A8%E5%AD%97%E8%A1%A8/8922402?fr=aladdin#9)）。与 GB 2312 表仅有两个字不重合（「啰」「瞭」）。
4. **4808** 指繁体中文 4808 常用字，台湾地区称「常用国字标准字体表」，含于 BIG5。
5. **BIG5** 指繁体中文地区通行的「大五码」字符集标准，共 13058 字。分常用字和次常用字，常用字表 5401 字。
6. **JIS** 指日文字体原有字库。
7. **通规** 指《通用规范汉字表》，共 8105 个字，跨越 CJK 统一汉字基本区及扩展 A～E 区，与 GB 2312 表有 6638 个字重合。（简体为主）

## 使用许可与限制

1. 对于 **SIL Open Font License 1.1** 授权字体的使用许可与限制说明如下。 *（适用于「小赖字体」「悠哉字体」「漫黑」「文楷」「975 系列字体」）*

   > #### 允许做的事：
   >
   > - 这款字体无论是个人还是企业都可以自由商用，无需付费，也无需知会或者标明原作者。
   > - 这款字体可以自由传播、分享，或者将字体安装于系统、软件或APP中也是允许的，可以与任何软件捆绑再分发以及／或一并销售。
   > - 这款字体可以自由修改、改造，制作衍生字体。修改或改造后的字体也必须同样以 [SIL OFL](https://scripts.sil.org/OFL) 公开。
   >
   > #### 注意事项：
   >
   > - 在制作衍生字体时，字体名称不可使用原有字体的「保留名称」 *（如思源黑体衍生的字体不能以「思源」「Source」等名称命名，具体见各字体的授权说明）* 。
   > - 这款字体不能用于违法行为，如因使用这款字体产生纠纷或法律诉讼，作者不承担任何责任。
   > - 根据 [SIL Open Font License 1.1](https://scripts.sil.org/OFL) 的规定，禁止单独出售字体文件(OTF/TTF文件)的行为。
   >
   > #### 简言之：
   >
   > 可以用、可以嵌、可以改、不能单独卖。

2. 对于 **IPA Font License 1.0**  授权字体的使用许可与限制说明如下。 *（适用于两款「晰黑」）*

   > #### 允许做的事：
   >
   > - 这款字体可以在任何设备上安装，可自由用于印刷物、图片、视频等 *（如手册、平面广告、影视广告、网络/新媒体广告、影视作品内用字、产品包装等）*，无需付费，也无需知会或者标明原作者。
   > - 这款字体可以自由传播、分享，或者将字体安装于系统、软件或APP中也是允许的。
   > - 这款字体可以自由修改、改造，制作衍生字体。修改或改造后的字体也必须同样以 [IPA Font License 1.0](https://moji.or.jp/ipafont/license/) 公开。
   >
   > #### 注意事项：
   >
   > - 在制作衍生字体时，字体名称不可使用原有字体的「保留名称」 *（即从 IPA 字体衍生的字体不能以「IPA」命名。）*
   >
   > #### 简言之：
   >
   > 可以用，可以嵌，可以改。

**注意：** SIL OFL 与 IPA Font License 不兼容，将这两种不同授权方式的字体混合成的字体不可公开发布。

---

以上六款字体均为开源字体，允许自由分享、下载、用于商业用途，也欢迎专业人士或业余字体爱好者在这六款字体基础上修改、优化或衍生。