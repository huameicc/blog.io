---
layout: page
title: "TimeLine"
description: "时间轴"
header-img: "img/orange.jpg"
---


<ul class="listing">
{% for post in site.posts %}
  {% capture y %}{{post.date | date:"%Y"}}{% endcapture %}
  {% if year != y %}
    {% assign year = y %}
	<p/>
    <li class="listing-seperator">{{ y }}</li>
  {% endif %}
  <li class="listing-item">
    <a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a>
    <time datetime="{{ post.date | date:"%Y-%m-%d" }}">{{ post.date | date:"%m-%d" }}</time>
  </li>
{% endfor %}
</ul>


