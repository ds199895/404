---
title: Non-uniform offset
tags: [Graphics]
style: fill
color: dark
description: Unequally offsetting grid edges based on certain elements.
---


## 方式1 根据半边的显示的方式启发，利用偏移找交线方式
原始效果
![origin](https://archialgo-com-sources.oss-cn-hangzhou.aliyuncs.com/images/Untitled.png "origin")
偏移效果
![offset](https://archialgo-com-sources.oss-cn-hangzhou.aliyuncs.com/images/Untitled1.png "offset")
半边显示
![half_edge_ori](https://archialgo-com-sources.oss-cn-hangzhou.aliyuncs.com/images/Untitled2.png "hlfedge_ori")
![half_edge_offset](https://archialgo-com-sources.oss-cn-hangzhou.aliyuncs.com/images/Untitled3.png "halfedge_offset")

## 方法2 利用四点共圆的平面几何原型进行转化运算
计算示意
![cal](https://archialgo-com-sources.oss-cn-hangzhou.aliyuncs.com/images/Untitled4.png "cal")

据此，找到每个顶点对应的偏移后的点

特殊情况排除与处理：

![special](https://archialgo-com-sources.oss-cn-hangzhou.aliyuncs.com/images/Untitled5.png "special")

避免自相交：

1.计算三线共点阈值
![jion](https://archialgo-com-sources.oss-cn-hangzhou.aliyuncs.com/images/Untitled6.png "jion")


2.分类讨论阈值点在偏移后线的内/外侧
![out](https://archialgo-com-sources.oss-cn-hangzhou.aliyuncs.com/images/Untitled7.png "out")

同上

![like above](https://archialgo-com-sources.oss-cn-hangzhou.aliyuncs.com/images/Untitled8.png "like above")

另外一种可能：通过判断是否反向延长进行区分
![Reverse Extension Line](https://archialgo-com-sources.oss-cn-hangzhou.aliyuncs.com/images/Untitled9.png "Reverse Extension Line")
![Reverse Extension Line2](https://archialgo-com-sources.oss-cn-hangzhou.aliyuncs.com/images/Untitled10.png "Reverse Extension Line")
效果：

![Final outcome1](https://archialgo-com-sources.oss-cn-hangzhou.aliyuncs.com/images/Untitled11.png "Final outcome")
![Final outcome2](https://archialgo-com-sources.oss-cn-hangzhou.aliyuncs.com/images/Untitled12.png "Final outcome")
![Final outcome3](https://archialgo-com-sources.oss-cn-hangzhou.aliyuncs.com/images/Untitled13.png "Final outcome")
![Final outcome4](https://archialgo-com-sources.oss-cn-hangzhou.aliyuncs.com/images/Untitled14.png "Final outcome")
![Final outcome5](https://archialgo-com-sources.oss-cn-hangzhou.aliyuncs.com/images/Untitled15.png "Final outcome")
![Final outcome6](https://archialgo-com-sources.oss-cn-hangzhou.aliyuncs.com/images/Untitled16.png "Final outcome")