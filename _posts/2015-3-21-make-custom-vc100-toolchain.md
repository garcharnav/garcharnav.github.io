---
layout: post
title: 抽离自定义vc100工具链
category: tech
---

gkEngine发布后，由于第三方库版本以及我自己是vs2010的使用者等原因，gkEngine对vs2010之后的版本基本是没有支持。由于使用的havok, toolkitpro界面库等原因，导致gkHavok, gkHavokAnimation, gkstudio无法编译。

其实解决方案相对简单，找一个vs2010安装，然后在vs2013等高版本选择vc100的工具链编译即可。不过这不免需要多下载安装一次工具链。

vs编译是经由msbuild来做的，那么理论上我们只用把msbuild系统及其依赖的sdk拷贝到相应位置即可。

所以，周末开始利用一台只安装vs2013的计算机来进行实验。
