---

layout: post
title: 如何实现 TTF 字体时间冒号居中？
categories: 字体修改教程
description: 利用 OpenType 特性，实现半角冒号在阿拉伯数字间居中显示，便于显示时间。
keywords: 冒号, OpenType, 居中

---

由于英文排版的原因，大多数英文字体的冒号、分号等标点符号都和小写的英文字母平齐。因此当它和阿拉伯数字搭配的时候，就会显得偏下。由于时间出现的次数特别多，一般人已经习惯了，只有少数人觉得不适应。

 

2019年10月31日，锤子科技带来了全新的产品——坚果Pro 3，随着这部手机亮相的还有全新的系统界面：Smartisan OS 7.0，以及全新的系统界面字体：Smartisan T黑。这款字体有很多亮点，比如：“ 、《等符号的间距调整，以及数字之间的冒号居中。

 

实现这个效果的，是 OpenType 特性。但是目前很多中文 TTF 字体，都没有这样的 OpenType 特性。下面为大家讲解如何利用 OpenType 特性实现 TTF 字体的时间冒号居中。由于不是专业的，所以可能会有疏漏或晦涩之处，欢迎指正。

 

【注意】由于本人使用的是英文版 FontCreator，所以有很多中英夹杂的表述，如有不适请点左上角，不喜勿喷。

1. 首先，用 FontCreator 打开一个 TTF 字体文件。（这里以公众号「霞鹜」里分享的“苹方 Pro”字体、FontCreator 11.5 英文版为例，原字体不含任何的 OpenType 特性信息）。

   ![](\images\posts\colon-between-digits\s01.png)

2. 点击菜单栏上的 Insert -> Glyphs，在字体的最后插入一个空白的字形。

   ![](\images\posts\colon-between-digits\s02.png)

3. 找到 $3A，也就是西文冒号。

   ![](\images\posts\colon-between-digits\s03.png)

4. 复制西文冒号到空白字符，然后将这个字符更名为“colon.alt”（或一个你能记得住的名字）。

   ![](\images\posts\colon-between-digits\s04.png)

5. 点击菜单栏 Tools -> Glyph Transform，然后在左面的列表里选择 Outlines -> Move，这里填写 (0, 100)，这个值因字体而异，需要自己找感觉。

   ![](\images\posts\colon-between-digits\s05.png)

6. 点击菜单栏 Font -> OpenType Designer。弹出这个窗口。

   ![](\images\posts\colon-between-digits\s06.png)

7. 点击下图红圈所示的图标，进入 Class Manager。

   ![](\images\posts\colon-between-digits\s07.png)

8. 点击对话框左上角绿色的加号，在弹出的对话框里选择数字 0-9。（建议在操作之前，先用 Tools -> Sort Glyphs -> Unicode Codepoints 对字符进行排序，以免在有些字体中找不着）。然后点击确定。

   ![](\images\posts\colon-between-digits\s08.png)

9. 给这个组合起一个名字，这里取名为 Numbers。

   ![](\images\posts\colon-between-digits\s09.png)

10. 可以看到一个新的 Class 建立成功了，里面包含着阿拉伯数字 0-9。但是还是 Not Used。这时点击确定。

    ![](\images\posts\colon-between-digits\s10.png)

11. 点击 OpenType 左侧列表的 Lookups，点击加号，新建一个 Lookups。选择 Single substitution（单个字符替换）。

    ![](\images\posts\colon-between-digits\s11.png)

12. 然后点击列表右面的加号，弹出一个对话框。按照图示选择字符。

    ![](\images\posts\colon-between-digits\s12.png)

13. 这时候，一个名为 “SingleSubstitution1” 的替换参照就定义好了（如果打开的 TTF 文件已有 OpenType 特性，则是最排在最后的 SingleSubstitution。）。然后再点击列表的加号，再新建一个 Lookup。

    ![](\images\posts\colon-between-digits\s13.png)

14. 选择“Chained Context Substitution”（根据上下文替换）。

    ![](\images\posts\colon-between-digits\s14.png)

15. 然后按照图示，在 Blacktrack 里选择 @Numbers 这个组合。

    ![](\images\posts\colon-between-digits\s15.png)

16. 按照图示操作，这里不再赘述。

    ![](\images\posts\colon-between-digits\s16.png)

17. 然后在点击左侧列表的 Features。点击加号，弹出 Add Feature。点击 Custom，命名 “calt”。

    ![](\images\posts\colon-between-digits\s17.png)

18. 在新建的 calt 特性中点击右键 选择 New Item，然后在 Existing Lookup 里选择 “ChainingContext1”，也就是 14 步骤新建的参照（如果打开的 TTF 文件已有 OpenType 特性，则是最排在最后的 Chaining Context。）

    ![](\images\posts\colon-between-digits\s18.png)

19. 可以看到 ChainingContext1 的参照已经加进了 calt 特性里，但还是 not used。

    ![](\images\posts\colon-between-digits\s19.png)

20. 点击左侧列表的 Scripts，点击加号，新建一个脚本。首先添加已知的脚本，Latin，因为主要是用于拉丁字母。

    ![](\images\posts\colon-between-digits\s20.png)

21. 右击 Latin，点击 New Item，在弹出的窗口中选择 Default，设置在拉丁语言下的默认状态。

    ![](\images\posts\colon-between-digits\s21.png)

22. 右击Default，新增“calt”特性。

    ![](\images\posts\colon-between-digits\s22.png)

23. 这时，calt 特性已经成功加进去了。不过这还不算完。

    ![](\images\posts\colon-between-digits\s23.png)

24. 再次点击 Script，点击加号，新增一个默认语言的脚本。

    ![](\images\posts\colon-between-digits\s24.png)

25. 接下来的操作和步骤 22 相似。

    ![](\images\posts\colon-between-digits\s25.png)

26. 默认语言的 calt 的特性也成功添加了。

    ![](\images\posts\colon-between-digits\s26.png)

27. 点击 OK 保存，可以看到 calt 特性已经成功应用，并处于默认打开状态。

    ![](\images\posts\colon-between-digits\s27.png)

28. 点击菜单栏 File -> Export Font As，导出字体。

    ![](\images\posts\colon-between-digits\s28.png)

至此，教程结束。

有些人可能就要问了，要这么繁琐干什么？，直接将西文冒号上移，这么做是让冒号居中了吗？这么做确实简单，但也影响了英文排版的整齐和美观。

鸽了那么久，终于在个人博客上发布了。