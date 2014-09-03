---
layout: page
title: 性能杂谈
---
{% include JB/setup %}

做了好多性能优化相关的工作，从tps提升到rt的提升，从应用服务器成本考虑，到用户体验，从应用到网络。
不说全端性能优化，至少也可以从各个方面来个杂谈。

个人会从以下方面来写这个blog

*    请求
    *   DNS
    *   TCP 连接
    *   SSL 握手
*   服务端处理
    *   rpc调用
    *   数据库处理
    *   ...
*   客户端处理
    *   浏览器获取资源的限制
    *   浏览器渲染过程
    *   浏览器的一些限制
    *   ...


<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>



