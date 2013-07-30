---
layout: post
title: "使用Octopres写博客"
date: 2013-07-28 23:14
comments: true
categories: Octopress
---
一直以来都想找一个合适的博客编写网站，试过csdn,iteye，都不满意。就在冲动准备租一个VPS用wordpress搭建自己
的博客的时候，发现了Octopress。就是它了！免费的github托管，基于markdown的文本编写方式，可以使用自己喜欢的
文本编辑器，随意定制自己喜欢的样式，丰富的第三方插件，Octopress真是专为IT程序猿而生！

首先是搭建环境，花了两天时间。因为没有ruby背景，幸好[Octopress](http://octopress.org   "Octopress官网") 
的教程很完善，一步一步照做就可以了。这里说几点心得和注意事项：

1. 安装ruby以及相关的软件，一定要严格按照官网的版本，不可以高，不可以低。如果是在windows，直接使用安装包。
我在Mac下使用rvm安装ruby 1.9.3，需要安装gcc依赖，这里推荐使用打包好的pkg包。可以从这里下载：
[GCC For MacOS](https://github.com/kennethreitz/osx-gcc-installer)

2. 在开始写自己的博客之前，先熟悉markdown语法。这里推荐一个[学习链接](http://wowubuntu.com/markdown/)

3. 解决中文问题。在mac下没有遇到中文问题，但是在windows下很可能会有，特别是英文的windows操作系统。解决办法
只需要加上两个环境变量
	*	set LC_ALL=en_US.UTF-8
	*	set LANG=en_US.UTF-8

4. 如果要在多台机器上写博客，或者多个人合作，则可以按照以下的步骤(以tucao的博客为例）

	1. git clone https://github.com/tucao/tucao.github.com.git
	2. cd tucao.github.com
	3. git checkout source
	4. sudo gem install bundler
	5. bundle install
	6. mkdir _deploy && cd _deploy
	7. git init
	8. git remote add origin https://github.com/tucao/tucao.github.com.git
	9. git pull origin master
	10. cd ..
	
在完成以上10步之后，就可以按照官网的教程进行博客编写了。
