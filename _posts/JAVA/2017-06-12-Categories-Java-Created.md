---
layout: post
title: Java First
date: 2017-06-12
categories: Java
tags: [Java,Test]
description: java note.
---

##  Java Direct
Hello, Welcome to my blog.  
你好，欢迎来到我的博客。

这个帖子是我的第一个帖子，我会在这里进行一些简单的测试，仅仅是为了熟悉一些相关的内容，并对一些功能进行调试和优化，访客无需在意。这一次，我想看看代码高亮和分目录。

`String str = "";`
	
<code>
    /**定义变量*/
	String descrp = "Hello Java";
	
	/**转换大写*/
	String descrp-son = descrp.toUpperrCase();
</code>

`String descrp = "Hello Java";
	String descrp-son = descrp.toUpperrCase();`

{% highlight python %}

### 创建 sc
try:
    sc.stop()
    sc = SparkContext(conf=sc_conf)
except:
    sc = SparkContext(conf=sc_conf)

### 加载 hdfs 上的数据
url = 'hdfs://10.21.208.21:8020/user/mercury/minute_bar'
rdd_mkt_data = sc.wholeTextFiles(url, minPartitions=80) \
                 .setName('index_minute_bar') \
                 .cache()

{% endhighlight %}


