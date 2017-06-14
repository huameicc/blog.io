---
layout: page
title: "Category"
description: "文章分类"
header-img: "img/facebook.jpg"
---

<div id='category_cloud'>
{% for category in site.categories %}
<a href="#{{ category[0] }}" title="{{ category[0] }}" rel="{{ category[1].size }}">{{ category[0] }}</a><br/>
{% endfor %}
</div>

<ul class="listing">
{% for category in site.categories %}
  <li class="listing-seperator" id="{{ category[0] }}">{{ category[0] }}</li>
{% for post in category[1] %}
  <li class="listing-item">
  <time datetime="{{ post.date | date:"%Y-%m-%d" }}">{{ post.date | date:"%Y-%m-%d" }}</time>&emsp;&emsp;
  <a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a>
  </li>
{% endfor %}
{% endfor %}
</ul>

<!-- categories 和 tags 功能相似 -->
<script src="/media/js/jquery.tagcloud.js" type="text/javascript" charset="utf-8"></script> 
<script language="javascript">
$.fn.tagcloud.defaults = {
    size: {start: 1, end: 1, unit: 'em'},
      color: {start: '#f8e0e6', end: '#ff3333'}
};

$(function () {
    $('#category_cloud a').tagcloud();
});
</script>

<style type="text/css">
.listing-seperator{
  list-style-type: none;
  line-height : 200%;
  font-weight : bold;
  font-size : 18px;
}
  
.listing-item{
  list-style-type: none;
}

#category_cloud{
	font-size: 22px;
}
</style>
