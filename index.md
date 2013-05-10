---
layout: page
title: 缸中的大脑!
tagline: jvm应用外围调用隔离
---
{% include JB/setup %}

[缸中的大脑](http://zh.wikipedia.org/wiki/%E7%BC%B8%E4%B8%AD%E4%B9%8B%E8%84%91)是一个著名的思想实验

它假设将我们的脑部放入一个裝有营养液的桶內，并用超级计算机连接脑的神经末梢，而计算机可以向大脑传递各种信息，大脑所体验到的世界其实是计算机制造的一种幻觉，则此大脑該如何验证本身的存在。

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>



