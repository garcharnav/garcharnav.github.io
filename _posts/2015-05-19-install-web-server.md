---
layout: post
title: 在yosemite配置页面服务器
category: tech
---


### ·

目前正在办离职流程，腾讯那边的入职流程也还没搞完。最近工作压力轻松了下来，开始和老婆提前准备婚礼的事情。
请柬我们准备自己搭个网站来搞，不想用现在流行的那种微请柬。。。

刚装了win10，之前的服务器系统得重新弄。有一天偶尔发现貌似macOSX是自带apache和Php的，所以兴致来了，想在macOSX上搭建一下，
正好可以更加又bigger的来写页面了～

### ·

根据网上的教程，先找了个maverick的教程，配出来没用
又找了个yosemite的，貌似也不对
做沙发上鼓捣了半天，终于搞掂...
于是到这里记录一下，生怕耽误了今晚一晚上的宝贵时间

### ·

##### step1

确认系统版本，
我的版本目前是10.10.4

确认apache版本，
打开shell, 键入

```Shell
sudo apachectl -v

Server version: Apache/2.4.10 (Unix)
Server built:   Jan  8 2015 20:48:33
```

如果你也是和我一样的2.4.10版本的apache,可以继续往后看了，否则，可以找一下精确匹配的。这个配置感觉差别很大。

##### step2

启动apache
打开shell, 键入

```Shell
sudo apachectl start
```

测试运行
打开safari, 访问http://localhost

理论上这里会出现
It works!
那么这一步就完成了

##### step3

那么这时候，这个It works!的页面是放在/Library里的内部页面的，不方便修改。我们可以利用userdir，来设置自己的站点。
这里需要做几件事

* 修改httpd.conf配置文件
* 修改httpd-userdir.conf配置文件
* 添加<yourname>.conf配置文件 （yourname是你的用户名）
* 添加Sites文件夹，用来存放你的站点

下面一件一件来理清


