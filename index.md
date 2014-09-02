---
layout: page
title: 折腾不止
---
{% include JB/setup %}

买了一堆的工具和硬件产品，芯片等等，就是还没有开始玩

准备先搞个激光雕刻机，慢慢记录吧。


<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>



