---
layout: tasks_bar
title: 任务
description: 主要为近期作业
date: 2020-02-23 16:05:24 +0800
keywords: 任务, tasks
comments: true
menu: 任务
permalink: /tasks/
deadline: 2020-02-23 08:00:00
---

# 颜色说明

------

#### 深红色：截止时间 ≤ 3小时



#### 红色：3小时 < 截止时间 ≤ 24小时



#### 橙色：24小时 < 截止时间 ≤ 48小时



#### 黄色：48小时 < 截止时间 ≤ 72小时



#### 绿色：截止时间 > 72小时



#### 白色：任务尚未开始



#### 灰色：任务已截止



### 如有作业未列出可在下方评论或在QQ中告知。



<div class="btn-inline">
    <h1><button onclick="viewArchivedTasks()" class="btn btn-outline" type="button">查看已截止的任务</button></h1>
</div>
<script>
    function viewArchivedTasks() {
        window.location.href="https://switernal.cn/ArchivedTasks/";
    }
</script>



  <div class="comment">
      {% include comments.html %}
  </div>

