---
layout: post
title: JAVA运行环境
date: 2017-07-06
categories: Java
tags: Java
description: Java开发和学习环境准备
---

## 基本概念：
* JDK：开发者使用，低版本曾叫SDK
* JRE：运行时环境，有虚拟机，没有编译器
* SE： 桌面或简单服务器应用平台
* EE：复杂服务器应用平台
* ME：手机等小型设备平台

## Java开发工具箱下载：
<http://www.oracle.com/technetwork/java/javase/downloads>

## 环境变量：
	PATH = C:\Java\jdk1.7.0_79\bin

路径若有空格，整个路径加双引号

## 库源文件和文档：
文档-->点击中间进入-->选择版本-->左边下载转入（偶尔会转不到正确的地址，多试试）

<http://www.oracle.com/technetwork/java/javase/documentation/java-se-7-doc-download-435117.htmlhttp://www.oracle.com/technetwork/java/javase/documentation/java-se-7-doc-download-435117.html>

src.zip：公共类库，无编译器、虚拟机、本地方法等

	jar xvf ../src.zip

	jar xvf jdk-7u79-docs-all.zip

## JAVA Core 示例：
<http://horstmann.com/corejava>

	jar xvf ../corejava.zip

使用JDK开发：

	javac Welcome.java
	Java Welcome
	appletviewer WelcomeApplet.html
	
***
*@huameicc Apr.20 2016*