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
    <li class="listing-seperator">{{ y }}</li>
  {% endif %}
  <li class="listing-item">
    <time datetime="{{ post.date | date:"%Y-%m-%d" }}">{{ post.date | date:"%m-%d" }}&emsp;&emsp;</time>
    <a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a>
  </li>
{% endfor %}
</ul>

<style type="text/css">
  .listing-seperator{
    list-style-type: none;
	line-height : 200%;
	font-weight : bold;
	font-size : 30px;
  }
  
  .listing-item{
    list-style-type: none;
  }
</style>

