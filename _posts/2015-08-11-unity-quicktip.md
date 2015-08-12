---
layout: post
title: Unity Quick Tips
category: hidden
---

### Unity Quick Tips

* GetComponents<T>() & GetComponents<T>(true) 取得active与取得active/inactive的components
* 在code中使用Shader.Find()的资源，一定要添加到always include shader中，否则运行时找不到
* ios build，需要手动设置graphics api到opengl es 3/2, 否则自动启用metal后在xcode中无法抓帧
