---
layout: page
title : tag列表
---
{% include JB/setup %}

<ul>
  {% for tag in site.tags %} 
    <li><a href="{{ BASE_PATH }}{{ site.JB.tags_path }}#{{ tag[0] }}-ref">{{ tag[0] }} <span>{{ tag[1].size }}</span></a></li>
  {% endfor %}
</ul>


