---
navs: [news,algorithm,banner]
tags: [Java, HalfEdge Data, Program]
image: https://archialgo-com-sources.oss-cn-hangzhou.aliyuncs.com/images/HEC_Catalan.png
title: HE_Mesh Library
title_cn: HE_Mesh程序包整理
description: HE_Mesh, a Java library for creating and manipulating polygonal meshes. Aimed primarily at Processing.  HE_Mesh 是基于Java语言的半边数据结构与几何库。该项目整理了HE_Mesh的各个类的方法与属性
team: [Biao Li, Siyuan He, Xuelu Zhang, Bei Wang, Jiajun Li]
status: Doing
year: 2019
date: 2020-10-16
types: [Geom,He_core,He_creators,He_modifiers,He_subdividors,He_tools,Core,Processing,Math,Nurbs,Other]
distype: Geom
---
### Due to internal research requirements, it has not been officially open-sourced yet. Therefore, only partial results are displayed.

{% assign carousel_items = site.hemesh| where:"navs","banner" %}
{% assign carousel_items = carousel_items | sort: "date" | reverse %}
{% include elements/project-carousel.html %}
{% include hemesh/project-search.html %}
{% include hemesh/index.html %}
