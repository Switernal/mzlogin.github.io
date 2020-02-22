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
{% for course in site.courses %}
    <li class="listing-item">
    	<a href="{{ site.url }}{{ math.url }}">
        <h2>{{ course.title }}</h2> 
        </a>

        <p class="{{course.class}}"></p>
  <script>
      function {{course.function}}() {
          countDown();

          function addZero(i) {
              return i < 10 ? "0" + i: i + "";
          }
          function countDown() {
              var nowtime = new Date();
              var endtime = new Date("2020/02/28,17:57:00");
              var lefttime = parseInt((endtime.getTime() - nowtime.getTime()) / 1000);
              var d = parseInt(lefttime / (24*60*60))
              var h = parseInt(lefttime / (60 * 60) % 24);
              var m = parseInt(lefttime / 60 % 60);
              var s = parseInt(lefttime % 60);
              d = addZero(d)
              h = addZero(h);
              m = addZero(m);
              s = addZero(s);
              document.querySelector(".{{course.class}}").innerHTML = `活动倒计时  ${d}天 ${h} 时${m} 分 ${s} 秒`;
              if (lefttime <= 0) {
                  document.querySelector(".{{course.class}}").innerHTML = "活动已结束";
                  return;
              }
              setTimeout(countDown, 1000);
            }
        }
    </script>
    </li>
{% endfor %}


</ul>

<script>    
      window.onload=function(){
  		{% for course in site.courses %}
  		  	{{course.function}}();
		{% endfor %}
      } 

</script>





