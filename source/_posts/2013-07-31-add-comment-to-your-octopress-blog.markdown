---
layout: post
title: "给Octopress博客加上评论"
date: 2013-07-31 15:17
comments: true
categories: Octopress
---

作为一个博客，一个评论系统必不可少。评论系统是你和读者互动的一个途径，除非你只想写给自己看。Octopress默认支持Disqus作为评论系统，但没有开启。
Disqus是一个非常出名的第三方评论平台，可以非常方便的嵌入到你的网站中。

按照下面的步骤开启Disqus评论：

*	首先在[Disqus][]官网注册一个账号，然后在首页上点击”Add Disqus to your site"，填写你的站点信息，最后并获得一个短号（short number）, 
	这个短号将用于你的网站和Disqus交互的凭证。
*	编辑_config.yml，修改下面两行

		#Disqus Comments
		disqus_short_name: XXXXXXXXX
		disqus_show_comment_count: true
*	新建一篇博客，将其 comments 设置为true， 意思就是允许评论。

一切就这么简单，简单的几步就拥有了一个强大的评论系统。这里再提及一句，Disqus可以再评论前加入广告，如果你的站点访问量很大，那么你可以利用Disqus来赚钱！
当然如果你不喜欢广告，可以将其去掉。

[disqus]:	http://disqus.com/	"Disqus"