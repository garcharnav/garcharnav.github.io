---
layout: post
title: Unity3D中的MaterialPropertyBlock
category: tech
---

背景故事
---

最近两天，在针对Unity3D做传统gpuskin的尝试。

所谓传统gpuskin，即使指利用vertexshader，通过传入的bone matrix进行蒙皮计算的方式。

而Unity3D提供的gpu skin，是一种更加鲁棒的方法：
利用"StreamOut"，在正常的vs-ps流程前，进行一次“通用”的蒙皮计算，而后stream out。因此，Unity3D的gpu skin对于用户来说是完全透明的！

然而不幸的是，这个特性，DX9享受不到，GLES2也享受不到。因此，Unity3D声明，gpu skin只能在dx11以及gles3平台才可使用。

更深入的实现细节之后再写文章详解，而今天要说的，是初次实验后的性能优化阶段... 发生的故事。

这一次的性能优化，才让我意识到了之前的一个很大的误区。

瓶颈所在
---

在
