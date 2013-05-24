---
layout: page
title: 缸中之脑!
---
{% include JB/setup %}

[缸中之脑](http://zh.wikipedia.org/wiki/%E7%BC%B8%E4%B8%AD%E4%B9%8B%E8%84%91)是一个著名的思想实验

> 它假设将我们的脑部放入一个装有营养液的桶內，并用超级计算机连接脑的神经末梢，而计算机可以向大脑传递各种信息，大脑所体验到的世界其实是计算机制造的一种幻觉，则此大脑該如何验证本身的存在。

当然这里不是来介绍这个思想实验,而是考虑,如果我们可以对应用系统做这么一个事情,模拟应用的外围调用,让应用以为自己在一个真实的环境中,从而对应用做各种不同的功能性验证,性能验证。并且环境的模拟内容也代码化，和代码一起管理，方便任何时候回溯相关的功能。

目前我们关注的是jvm上的应用，一方面是因为jvm现在应用的量比较大，另一个方面jvm提供了相应的字节码功能，给做这个事情提供了一些便利。


<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>



