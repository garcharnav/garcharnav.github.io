---
layout: post
title: 构建MacOSX工具链
category: tech
---

### ·

最近两天，利用晚上的时间，为gkENGINE构建了原生的MacOSX工具链。此时可以完全脱离windows及windows虚拟机，
直接在一台纯净的Mac机上clone, build, package, deploy，直接发布iOS App以及直接在MacOSX中运行gkENGINE了。

### ·

其实这是一个比较复杂的过程，大概的步骤有以下几点

* 改写bat到sh
* 编译gkResourceCompiler
* 寻找或替换MacOSX上的纹理转换工具
* 重新打包
