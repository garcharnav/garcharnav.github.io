---
layout: post
title: Unity Quick Tips
category: hidden
---

### Unity Quick Tips

* GetComponents<T>() & GetComponents<T>(true) 取得active与取得active/inactive的components
* 在code中使用Shader.Find()的资源，一定要添加到always include shader中，否则运行时找不到
* ios build，需要手动设置graphics api到opengl es 3/2, 否则自动启用metal后在xcode中无法抓帧
* 

### Unity Optimize Room | version 4.6.3

* skybox使用了6个drawcall,并且有overdraw,可优化为一个全屏quad.
* canvas group控制的下层空间，alpha为0之后并不清除
* 

### Trap in Unity

* 一旦在运行时修改了material的属性，哪怕修改为一样的，unity也不会帮你自动做合并。每一个都变为了完全独立的material instance。
  * 因此在运行时的material修改要十分谨慎
* unity3d在获取depth texture的时候，虽然manmal里提到如果能获取到system z buffer，则直接使用，但实际情况是几乎都需要重新绘制一遍场景来获得depth texture, 性能炸弹。
