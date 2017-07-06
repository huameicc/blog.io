---
layout: post
title: Git常用命令
date: 2017-07-01
categories: Blog
tags: Git
description: Git笔记
---
## 设置

生成SSH Key
	$ ssh-keygen -t rsa -C "youremail@example.com"

设置 git 全局用户名和邮箱
	$ git config --global user.name 名字
	$ git config --global user.email 邮箱


## 远程库

#### 先有本地项目

添加远程库

	git remote add [shortname] [url]

	$ echo "readme init" >> README.md
	$ git init                                  # 初始化
	$ git add README.md                         # 添加文件
	$ git commit -m "添加 README.md 文件"        # 提交并备注信息
	
	$ git remote add origin git@github.com:tianqixin/runoob-git-test.git	#需要先在Github建立仓库
	$ git push -u origin master					# 提交到 Github，注意 -u
	
查看远程仓库
	$ git remote -v
	origin  git@github.com:huameicc/blog.io.git (fetch)
	origin  git@github.com:huameicc/blog.io.git (push)

删除远程仓库
	$ git remote rm [别名]

从远端仓库提取数据并尝试合并到当前分支
	$ git pull

先提取，再手动合并到当前分支
	$ git fetch [alias]
	$ git merge [alias]/[branch] 
	
	$ git fetch origin
	$ git merge origin/master

推送到远程仓库
	$ git push [alias] [branch]
	$ git push
	$ git push origin master

#### 直接从远程库克隆
	$ git clone 版本库地址
	
	$ git clone http[s]://example.com/path/to/repo.git/
	$ git clone ssh://example.com/path/to/repo.git/
	$ git clone git://example.com/path/to/repo.git/
		
## Git本地操作
	
添加更新
	$ git add 文件名
	$ git add --all

Commit到本地仓库
	$ git commit -m "提交内容说明"
	
查看修改
	$ git differ 文件名

查看当前状态
	$ git status
	$ git status -s			#简短
	
查看commit日志
	$ git log
	$ git log --oneline --graph
	
## 分支
查看分支
	$ git branch
创建分支
	$ git branch 分支名
切换分支
	$ git checkout 分支名
创建并切换分支
	$ git checkout -b 分支名
删除分支
	$ git branch -D 分支名
重命名分支
	$ git branch -m 分支名 新分支名
合并分支到当前分支
	$ git merge 待合并分支名
	
##其他

更详细的关于Git的内容，可以参考以下教程：

* [Git菜鸟教程](http://www.runoob.com/git/git-tutorial.html)
* [廖雪峰Git教程](http://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000/)
	
