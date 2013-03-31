---
layout: post
title: "安裝Octopress"
date: 2013-03-25 22:31
comments: true
categories: Octopress
---

看到很多大大用Octopress來寫Blog	
覺得蠻酷的，於是也來玩玩看		
在這裡紀錄一下怎麼安裝以免我之後忘記		
先到github開一個repo	
名稱是username.github.com		
然後從git下載檔案到自己電腦裡

	git://github.com/imathis/octopress.git myblog
	cd myblog/
	
記得去修改設定檔_config.yml	 
因為新版本需要ruby 1.9.3	
所以我又安裝了1.9.3

	rvm install ruby-1.9.3-p374
	rvm use ruby 1.9.3

然後進入myblog目錄下指令

	gem update --system
	gem install bundler
	bundle install
	rake install
	rake setup_github_pages
	git@github.com:your_username/your_username.github.com
	git add .
	git commit -m 'first commit'
	git push origin source
	rake generate
	rake deploy
	
這樣你就可以在你的網址看到你的blog啦

	rake new_post["Title"]
	
發篇新文章吧!	

發現有大大寫的更好，大家也可以看看		
<http://wwssllabcd.github.com/blog/2012/08/01/how-to-install-octopress-on-window/>

Markdown語法可以參考	
<http://markdown.tw/>

Markdown的軟體我是用Markdown Pro	
<http://www.markdownpro.com/>