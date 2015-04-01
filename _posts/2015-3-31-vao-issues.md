---
layout: post
title: Vertex Array Object的纠缠
category: hidden
---

### ·

前些天，把一件一直想做又没做的工作完成了！将gkRendererGL330调试通过，在OSX, WIN32上跑起来了。

顺便，还完成了另一项壮举，将GL330和GLES2的代码统一了起来。在少量的地方通过宏或者VirtualAPI的方式封装，来区隔开来。

整个过程蛮顺利的，在上安卓真机之前...

### ·

统一的过程，主要就是将近期实现的GLES2上的deferred lighting和到GL330。处理了几个纹理生成，纹理格式的错误之后。
再修改了一下shader的preprocess逻辑，GL330没有经过太多的波折就成功的跑起来了，
（除了昨天发现的一个导致GL330比GLES2画面发暗的bug）。

统一中，主要就是就Vertex Array Object的使用进行了封装。VAO主要有一下几个函数：
* glGenVertexArrays
* glBindVertexArray
* glDeleteVertexArrays
