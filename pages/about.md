---
layout: page
title: About
description: 
keywords: 
comments: true
menu: 关于
permalink: /about/
---



## 个人简介
### 几句话简介
- 某双非高校安全工程专业毕业生，目前在东北地区某高铁项目部工作；
- 一个 **所谓的** 「电脑爱好者」；
- ~~(曾经是)~~ 一个玩机爱好者；
- 一个~~即将退坑的~~ DIY 字体爱好者；
- 一个 2016 年加入酷安的酷友；
- 一个懒癌患者（至少目前是）；
- 一个讨厌「伸手党」的分享者；
- ……

### 联系方式
- **Gmail：** [calxgw2018@gmail.com](mailto:calxgw2018@gmail.com)
- **QQ 邮箱：** [lxgw1999@qq.com](mailto:lxgw1999@qq.com)

## 精品资源
- [自制开源字体一览]({% link _posts/2021-01-15-Lxgw-Opensource-Chinese-Fonts.md %})
- [Magisk 字体模块套用包 *（跳转到少数派）*](https://sspai.com/post/58049)
- [个人网盘（永硕）](http://lxgw.ys168.com)

## 社交帐号

<ul>
{% for website in site.data.social %}
<li>{{website.sitename }}：<a href="{{ website.url }}" target="_blank">@{{ website.name }}</a></li>
{% endfor %}
{% if site.url contains 'lxgw.github.io' %}
<li>
微信公众号：<br />
<img style="height:192px;width:192px;border:1px solid lightgrey;" src="{{ assets_base_url }}/assets/images/qrcode.jpg" alt="霞鹜" />
</li>
{% endif %}
</ul>



##  

{% for skill in site.data.skills %}
### {{ skill.name }}
<div class="btn-inline">
{% for keyword in skill.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}
