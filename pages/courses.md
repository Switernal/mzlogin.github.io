---
layout: post
title: 课程
description: 近期课程
keywords: 课程，courses
comments: false
menu: 课程
permalink: /courses/
deadline: 2020-02-22 08:00:00
---

<ul class="listing">
{% for math in site.courses %}
    <li class="listing-item">
        <a href="{{ site.url }}{{ math.url }}">
        	<h2>{{ math.title }}</h2> 
        </a>

    	{% include time.html %}
    </li>
{% endfor %}
</ul>