---
layout: post
title: "Build Fire.app"
date: 2013-03-21 14:37
comments: true
categories: [Fire.app, CSS]
---
![Alt text](https://github.com/handlino/FireApp/raw/master/lib/images/icon/256.png)		
最近看到大家大推Fire.app,	
於是就嘗試自己編譯一個來玩玩看 	
步驟為下: 	

	$ rvm install 1.9.2 // tell rvm to install ruby 
		
	$ rvm use 1.9.2 // tell rvm use ruby 1.9.2 ver. 
	
	$ rvm install jruby // install jruby 
	
	$ rvm use jruby //jruby change to default 
	
	$ jruby -S gem install rawr // get rawr gem for jruby 
	// clone latest compass source code from github 
	
	$ git clone git://github.com/handlino/FireApp.git
	
	$ cd Fireapp 
	
	$ bin/build-all.sh
	
另外，在lib/ruby/common下有兩個資料夾		
-	tka-rack-coffee 	
-	tka-serve	

如果是空的，記得再下兩個指令更新他	

	git submodule init
	git submodule updata

然後編譯	
完成就可以開始開心使用Fire.app啦!	

官方github	
<https://github.com/handlino/FireApp>	

懶得編譯也可以直接到官方網站購買囉		
<http://fireapp.handlino.com/>