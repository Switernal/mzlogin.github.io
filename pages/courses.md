---
layout: post
title: 课程
description: 近期课程
keywords: 课程，courses
comments: false
menu: 课程
permalink: /courses/
deadline: 2020-02-23 08:00:00
---

<ul class="listing">
{% for math in site.courses %}
    <li class="listing-item">
        <a href="{{ site.url }}{{ math.url }}">
        	<h2>{{ math.title }}</h2> 
        	<div id="countdown18" class="ClassyCountdownDemo"></div>

<script type="text/javascript">
$(document).ready(function() {
	
	var deadLine = "{{page.deadline}}".substr(0,19);
	var date=new Date(deadLine);
	var unixTime = parseInt((date.valueOf() - $.now()) / 1000);

	$('#countdown18').ClassyCountdown({
		theme: "flat-colors-black",
		end: $.now() + unixTime
	});
});
</script>
        </a>	
    </li>
{% endfor %}
</ul>
{% include time.html %}
