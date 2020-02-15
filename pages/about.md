---
layout: page
title: About
date: 2020-02-15 18:47:30
description: 打码改变世界
keywords: Switernal, Sanders
comments: true
menu: 关于
permalink: /about/
---

## · 谈谈这个博客。

Switernal，即Swift（快捷）、Interconnect（互联）& Terminal（终端）。

这是一个个人博客，虽然简洁但访问快捷，并且面向互联网开放，希望能够提供近乎终端的阅览体验。


## · 开设初衷？

希望记录一些学习过程中遇到的问题，打造成一个便携的笔记本。

------


## · 个人

暂且可以称呼我为Sanders

目前就读于南京某郊区高校计算机相关专业

## 联系

{% for website in site.data.social %}
* {{ website.sitename }}：[@{{ website.name }}]({{ website.url }})
{% endfor %}


## 目前正在学习的技术

{% for category in site.data.skills %}
### {{ category.name }}
<div class="btn-inline">
{% for keyword in category.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}

