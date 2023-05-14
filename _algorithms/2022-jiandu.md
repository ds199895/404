---
navs: [news,program,banner]
tags: [OpenCV, python,OCR]
image: https://archialgo-com-sources.oss-cn-hangzhou.aliyuncs.com/images/jiandu3.jpg
title: Search and original text processing of ancient book library based on web crawler and OpenCV
title_cn: 基于爬虫与OpenCV的古籍库搜索与原文处理
year: 2022
description: 通过爬虫爬取古籍库关键词搜索结果，下载图片，然后通过opencv进行图像分割，将文字切块分好，然后再进行组合，成为“简牍”，然后调用合合信息api进行OCR识别，获取原文。
team: [He Siyuan]
status: Done🙌
date: 2022-06-20
---
---

### 源起
项目缘起于一门课：建筑史研究入门，是以词条研究形式展开。以古籍库和各类已有数据库中对某词条的查询结果为数据来源，进行文献梳理与研究。所以如何快速获取词条以及所在古籍信息成为首要任务。

### 爬取图片
首先通过对古籍库网页的研究，进行词条搜索页面的爬取。
获得的图片示例如下：
![](https://archialgo-com-sources.oss-cn-hangzhou.aliyuncs.com/images/jiandu1.jpg)

<center>爬取图片示例</center>
<br>
这一步完成之后，就可以进行OCR识别与分析，但是得到的原始图片带有的信息比较复杂，识别精度无法满足需求。
另外，因为后续需要对文本进行研究分析，词条当页文字并不够，故而同时下载上下文两页图片。为了精度尽量高和调用api次数尽量少，需要对三张图片进行文字分割与重组。

### OpenCV图像分割与重组
在原始图片基础上，进行openCV分割与重组。
通过将图片nparray水平与垂直拍平的像素信息进行文字与空白的区分，然后对像素进行分割，将所有文字分割成一个一个小块存储。然后再按照顺序将三张图片中的文字合并，扔掉多余信息，成为简牍一样的形式。
![](https://archialgo-com-sources.oss-cn-hangzhou.aliyuncs.com/images/jiandu2.jpg)
<center>openCV分割：文字块</center>
<br>
![](https://archialgo-com-sources.oss-cn-hangzhou.aliyuncs.com/images/jiandu3.jpg)
<center>文字块重组：简牍</center>
<br>
在此基础上调用合合api进行OCR文字识别。几乎能够保证100%的识别精度。

### GUI用户界面
在完成以上程序的主体内容之后，设计了程序的GUI界面，将之前实现的功能：xls合并与分析，古籍库词条搜索，古籍库词条下载与识别整合在一起。
![](https://archialgo-com-sources.oss-cn-hangzhou.aliyuncs.com/images/jiandu5.png)
<center>搜索</center>
<br>
![](https://archialgo-com-sources.oss-cn-hangzhou.aliyuncs.com/images/jiandu6.png)
<center>词条下载</center>
<br>
![](https://archialgo-com-sources.oss-cn-hangzhou.aliyuncs.com/images/jiandu7.png)
<center>词条分析</center>
<br>

{% include elements/button-top.html %}
