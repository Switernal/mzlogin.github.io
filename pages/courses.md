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



<h1>Test1</h1>
<p class="count"></p>
  <script>
      function Timer1 () {
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
              document.querySelector(".count").innerHTML = `活动倒计时  ${d}天 ${h} 时${m} 分 ${s} 秒`;
              if (lefttime <= 0) {
                  document.querySelector(".count").innerHTML = "活动已结束";
                  return;
              }
              setTimeout(countDown, 1000);
            }
        }
    </script>

<h1>Test2</h1>
<p class="count"></p>
  <script>
      function Timer2 () {
          countDown();
          function addZero(i) {
              return i < 10 ? "0" + i: i + "";
          }
          function countDown() {
              var nowtime = new Date();
              var endtime = new Date("2020/02/24,17:57:00");
              var lefttime = parseInt((endtime.getTime() - nowtime.getTime()) / 1000);
              var d = parseInt(lefttime / (24*60*60))
              var h = parseInt(lefttime / (60 * 60) % 24);
              var m = parseInt(lefttime / 60 % 60);
              var s = parseInt(lefttime % 60);
              d = addZero(d)
              h = addZero(h);
              m = addZero(m);
              s = addZero(s);
              document.querySelector(".count").innerHTML = `活动倒计时  ${d}天 ${h} 时${m} 分 ${s} 秒`;
              if (lefttime <= 0) {
                  document.querySelector(".count").innerHTML = "活动已结束";
                  return;
              }
              setTimeout(countDown, 1000);
            }
        }  


      window.onload=function(){
      Timer1();
      Timer2();
  } 

</script>



