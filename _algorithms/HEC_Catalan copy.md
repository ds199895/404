---
navs: [template,banner,construct]
tags: [Digital Fabrication, Installation, Project, Anren]
image: http://labaaa.org/wp-content/uploads/2020/10/640-19.jpg
title: Linpan Landscape Installation
title_cn: 南岸美村“林·盘”艺术景观装置
location: Chengdu, Sichuan, China
location_cn: 四川·成都
description: HE_Mesh 是基于Java语言的半边数据结构与几何库。该项目整理了HE_Mesh的各个类的方法与属性
team: [Biao Li, Peng Tang, Hongjian Li, Yulong Chen, Yichen Mo, Zhenyu Hu]
year: 2019
date: 2020-10-16
---

<!-- # *Linpan* Landscape Installation -->

![](http://labaaa.org/wp-content/uploads/2020/10/640.jpg)

The name “Linpan”  derives from the unique residential environment form of  Western Sichuan plain, which was an organic integration of farmyard and surrounding trees, bamboos, rivers and cultivated land.

“Linpan” is a landscape installation designed for the Nan-an-mei village. The flow of shape and the pattern of scattered light and shadow indicate the  unique rural  scenery— scattered rivers, fields and forests.


### 设计意向：川西林盘的再现

项目场地位于成都市大邑县安仁古镇南岸美村核心区的安仁绿道，北侧为锦绣安仁花卉公园与乡苑酒店，南侧为花房茶社、乡村生态博物馆以及乡村客厅等当代乡村景观设施。地块位于绿道关键节点，处于大片农田景观中。地势平坦，视野开阔，偶有几从树木自然生长。雨过天晴时，远处可见西岭雪山，白鹭飞度。杜甫的绝句“ 窗含西岭千秋雪，门泊东吴万里船”就是描写的这里。

{% capture carousel_images %}
http://labaaa.org/wp-content/uploads/2020/10/640-1-e1602847724267.jpg
http://labaaa.org/wp-content/uploads/2020/10/640-2.jpeg
http://labaaa.org/wp-content/uploads/2020/10/640-3.jpg
{% endcapture %}
{% include elements/carousel.html id=1 %}

<figcaption class="text-center">场地状况</figcaption>
<br>

原场地视野开阔，在绿道的关键节点建构一处让人们能够穿越其中大型艺术景观装置是本次设计的目标。设计结合场地上树木的形象以及2019安仁双年展的主题“共同的神话”，从地面的几个点向天空伸展出树干，在天空中连成一体，寓意文化的共通与交融。功能上，艺术装置呈现出在岔路口的三个方向上的开放性，能容纳一定人流的同时，也为观光车提供停靠位置。

![](http://labaaa.org/wp-content/uploads/2020/10/640-4.jpg)
<figcaption class="text-center">设计意向</figcaption>

### 要素规则化的数字设计

本项目从第一次场地踏勘到建造完成只有不到5个月的时间。团队选择数字链生成技术，将设计与建造无缝结合，并由建筑师完成从设计到加工到建造的全过程。团队将设计要求抽取为设计参数输入自行开发的数字链系统中。经过程序编写智能化地生成形态，并对其进行反复比对和调整。为了达到轻盈通透的效果同时又保证地方特色，装置的饰面花纹从川西地区少数民族服饰纹样，建筑装饰图案中间进行提炼。每个饰面板在模板图案的基础上，根据其所处位置和高度，基于程序产生疏密变换的效果。让人身处不同位置时，有着不同的空间感受。

{% capture carousel_images %}
http://labaaa.org/wp-content/uploads/2020/10/640-5.jpg
http://labaaa.org/wp-content/uploads/2020/10/640-6.jpg
{% endcapture %}
{% include elements/carousel.html id=2%}
<figcaption class="text-center">效果图</figcaption>

![](http://labaaa.org/wp-content/uploads/2020/10/640-7.jpg)
<figcaption class="text-center">装饰面板纹样生成设计效果对比（局部）</figcaption>

## 形态生成与结构验算的并行操作

林·盘所确定的方案，为一种完全自由曲面的空间造型。由于场地限制，整个艺术装置覆盖面积超过300平米而落地点只有4个，因此产生较多极限悬挑，最大处单向悬挑达到7米。同时为了获得优美的空中造型，每一根工字型断面的结构构件又都在空间中发生三维扭转。这些都需要在形态生成的同时进行缜密的结构计算。通过调整参数的数值和权重，程序对所有构件进行了复杂而全面的参数设定，对构件与构件的断开与连接点位的选择进行了严格的推断，并实现了伴随形态修改的实时调节。最终程序确保了每一根构件都与其相邻构件在空间上正向对接，使这些构件组成的空间形态满足结构受力条件。以上细节确定后，程序完成从形态生成到构件分解到数据输出的全过程，并附带输出所有相关材料以及零部件的
数量级成本预算，给出加工方法。

![](http://labaaa.org/wp-content/uploads/2020/10/640.gif)
<figcaption class="text-center">基于场地条件的形态生成与构件分解</figcaption>

![](http://labaaa.org/wp-content/uploads/2020/10/640-8.jpg)
<figcaption class="text-center">程序生成的面板构件（局部）</figcaption>

![](http://labaaa.org/wp-content/uploads/2020/10/640-9.jpg)
<figcaption class="text-center">程序生成的结构构件</figcaption>

### 数字链控制下的构件加工

为了能够快速建造同时保证作品的持久性，耐候钢板和铝板共同被选择作为艺术装置的材料。耐候钢板通过弯折拼接形成主要结构体骨架，铝板自重较小，作为饰面板附加在骨架上。所有构件和面板均在程序中批量生成必要数据后，经过相应CNC设备的切割、弯折、焊接后完成构件加工。最终，林盘的空间构成由140个形态各异的耐候钢结构构件（含单向构件和十字构件）和1600余块样式不同的铝板饰面板组成。

![](http://labaaa.org/wp-content/uploads/2020/10/procedure.gif)
<figcaption class="text-center">安装工序示意图</figcaption>

### 预制与安装

预制装配和现场建造过程共历时一个月。首先在Inst. AAA实验室完成了1:7完整结构模型的制作和结构检验。其次，完成了特殊十字节点构件的1:1制造与安装实验。之后，设计数据传到工厂的大型CNC设备中，进行批量数控加工与局部试安装。完成的构件经过防锈处理后运至成都安仁进行现场安装。这项艰巨的工程在预定期内圆满完成。

![](http://labaaa.org/wp-content/uploads/2020/10/640-10.jpg)
<figcaption class="text-center">1:7 实验室模型</figcaption>

{% capture carousel_images %}
http://labaaa.org/wp-content/uploads/2020/10/640-11.jpg
http://labaaa.org/wp-content/uploads/2020/10/640-12.jpg
http://labaaa.org/wp-content/uploads/2020/10/640-13.jpg
http://labaaa.org/wp-content/uploads/2020/10/640-14.jpg
http://labaaa.org/wp-content/uploads/2020/10/640-15.jpg
http://labaaa.org/wp-content/uploads/2020/10/640-16.jpg
{% endcapture %}
{% include elements/carousel.html id=3%}
<figcaption class="text-center">工厂预制到现场安装全过程</figcaption>

### 完成效果

完工时的“林 · 盘”总高近7米，占地近340平方米。如同设计师的预期那样，整个艺术装置像一朵轻盈的云漂浮在空中。

从远处眺望，“林 · 盘”的形态随着视角和观察点的不同展现出极其丰富的变化。近观“林 · 盘”，亦能感受到装饰图案的淡入淡出，欣赏田间地面上的错落光影。此为数字生成技术为川西田园所增添的异彩。

{% capture carousel_images %}
http://labaaa.org/wp-content/uploads/2020/10/640-17.jpg
http://labaaa.org/wp-content/uploads/2020/10/MG_7388.jpg
http://labaaa.org/wp-content/uploads/2020/10/MG_7376.jpg
http://labaaa.org/wp-content/uploads/2020/10/640-19.jpg
http://labaaa.org/wp-content/uploads/2020/10/640-20.jpg
http://labaaa.org/wp-content/uploads/2020/10/DJI_0050.jpg
http://labaaa.org/wp-content/uploads/2020/10/夜景合并.jpg
{% endcapture %}
{% include elements/carousel.html id=4%}
<figcaption class="text-center">建成实景</figcaption>

### 结语
数字链技术将生成设计与数控建造无缝结合，使得这一创造性的自由曲面的空间造型能够完美呈现，也使得建成形态与设计师的设计预期完全一致。同时，这一高难度的空间结构的完成，是建筑师与结构师之间相互支持，高度合作的产物。“林 · 盘”的设计与建造，是对Inst. AAA近十年来的研究积累和设计能力的检验，预示着团队有能力够迎接更多更大的挑战。

---

**项目名称** ：南岸美村乡村“林·盘”大型艺术装置

**项目地点** ：四川省成都市大邑县安仁古镇

**规 模** ：覆盖面积：约340平米；高度：最高点7米，起拱最低点4.8米

**设计单位** ：东南大学建筑运算与应用研究所（Inst. AAA），东南大学建筑设计研究院有限公司

**主持建筑师** ：李飚、唐芃

**设计团队** ：李鸿渐，陈宇龙，莫怡晨，胡震宇等

**结 构**：杨波

**数控加工** : 南京耀阳科技有限公司

**业 主** ：成都安仁华侨城文化旅游开发有限公司

**项目时间** ：2019年4月-9月

**摄 影**：许昊皓，龙灏，王笑，唐芃

---

