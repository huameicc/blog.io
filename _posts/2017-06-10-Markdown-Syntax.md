---
layout: post
title: Markdown常用语法
date: 2017-06-10
categories: Blog
tags: Markdown
description: 关于Markdown的简明教程
---
## Markdown概述

Markdown 作为一种轻量级文本编辑语言，其宗旨是「易读易写」。
作为一种书写的格式，Markdown语法全由符号构成。
同时Markdown也能兼容HTML语法， Markdown 最终会被解释器翻译为 HTML. 
Markdown有些格式符号和正文间要空一格，如标题符号#，因此为了清晰最好都空一格。

## Markdown语法

### 段落

前后空一行，文本编辑的手动换行不会生效，若要强行换行，可以插入`<br/>`或者两个空格再回车。

	first line  
	second line

first line  
second line

### 标题

前面加上1~6个 #

### 区块引用

每段落开始前加上 > ,内部还可以嵌套Markdown语法。

	> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,
	consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.
	Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.
	>
	> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse
	id sem consectetuer libero luctus adipiscing.

> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,
consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.
Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.
>
> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse
id sem consectetuer libero luctus adipiscing.

### 列表

无序列表使用星号、加号或是减号作为列表标记：

	*   Red
	*   Green
	*   Blue	
*   Red
*   Green
*   Blue

有序列表使用数字接着一个英文句点

	1. A
	2. B
	3. C
1. A
2. B
3. C

为了避免无意产生列表，使用数字+句点+空格时，可以对句点使用反斜杠转义，

	2017\. 不是列表

2017\. 不是列表

### 代码区块

每行缩进 4 个空格或是 1 个制表符，多余的空格或制表符会被保留，首行前应留空一行。代码区块里Markdown语法通常都会无效，因而代码可以随意使用符号。

	<div class="footer">
		&copy; 2004 Foo Corporation
    </div>
	
### 行内代码

将代码用反引号包起来（`）；如果要在代码区段内插入反引号，可以用多个反引号来开启和结束代码区段；代码区段的起始和结束端还可以放入一个空白：

	``There is a literal backtick (`) here.``

	A single backtick in a code span: `` ` ``

	A backtick-delimited string in a code span: `` `foo` ``
***

``There is a literal backtick (`) here.``

A single backtick in a code span: `` ` ``

A backtick-delimited string in a code span: `` `foo` ``

### 分隔线

用三个以上的星号、减号、底线来建立一个分隔线

	分割线上
	***
	分割线下

分割线上
***
分割线下

### 区段元素

#### 强调

星号（*）或下划线（_）作为强调符号，被强调文字两边要有相同数量的星号。一个表示斜体 em,两个表示加粗 strong.
【强调字符不要加空格】

	*em*  
	**strong**

*em*  
**strong**

#### 链接

行内式： 方块括号标记链接文字，后面紧接着圆括号插入网址链接，【链接后面还可以跟着用双引号设置链接title】

	[jekyll官网](http://jekyllrb.com/)

[jekyll官网](http://jekyllrb.com/)

参考式： 用两个方块括号，第二个方块括号里添加链接标记【可以为空，这样第一个括号里的链接文字会被当成标记】；
并在其他任意地方，定义链接标记具体链接，一个方括号添加标记，跟着一个冒号，接着具体链接。

	[jekyll官网][link00]
	
	[link00]: http://jekyllrb.com/

[jekyll官网][link00]

[link00]: http://jekyllrb.com/

自动链接： 直接用一对尖括号将链接包起来

	<http://example.com/>
	<address@example.com>
	
<http://example.com/>

<address@example.com>

#### 图片

行内式： 

* 一个惊叹号 !
* 接着一个方括号，里面放上图片的替代文字
* 接着一个普通括号，里面放上图片的网址，还可以选择用双引号添加title.

	![Alt text](/path/to/img.jpg)
	![Alt text](/path/to/img.jpg "Optional title")

参考式：与链接参考式类似

	![Alt text][id]
	[id]: url/to/image  "Optional title attribute"

### 反斜杠

Markdown 支持以下特殊符号前面加上反斜杠，来表示对应的普通文本：
	\   反斜线
	`   反引号
	*   星号
	_   底线
	{}  花括号
	[]  方括号
	()  括弧
	#   井字号
	+   加号
	-   减号
	.   英文句点
	!   惊叹号
	
## 其他

可以利用Github或者其它工具预览Markdown文本效果。

更详细的关于Markdown的语法可以参考：

* [Markdown 语法说明 (简体中文版)](http://www.appinn.com/markdown/)
* [Markdown中文网](http://www.markdown.cn/)

Markdown还有相应的编辑工具，比如：

* [Markdown Pad](http://markdownpad.com/)
* [好用的Markdown编辑器一览](http://www.williamlong.info/archives/4319.html)

***
*@huameicc*


