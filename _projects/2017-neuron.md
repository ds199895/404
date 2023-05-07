---
navs: [news, banner,construct]
tags: [Digital Fabrication, Installation, Robotic Timber]
image: http://labaaa.org/wp-content/uploads/2019/10/现场照片6.jpg
title: Robotic Timber Construction
year: 2017
location: Nanjing, Jiangsu, China
location_cn: 江苏·南京
description: The Neuron project built a novel thin-shell structure with advanced methods of computational design & robotic fabrication.
image: http://labaaa.org/wp-content/uploads/2017/09/neu3.jpg
team: [Biao Li, Hao Hua, Peng Tang, ..., Yichen Mo, ..., etc.]
date: 2017-09-21
---

<!-- # ROBOTIC TIMBER CONSTRUCTION -->


The Neuron project built a novel thin-shell structure with advanced methods of computational design & robotic fabrication. The wood pavilion, located in the campus at Nanjing University, spans about seven meters. The entire installation is made of 61 pieces of irregular plywood panels connected by their own “fingers”, without any nails or glue.

![](http://labaaa.org/wp-content/uploads/2017/09/neu3.jpg)

The team developed an iterative algorithm in Java programming language to generate a compression-only shell structure. The shell’s openings are associated with the settings of the courtyard. The geometries of the plywood panels are concerned with structural stability, tectonic feasibility, manufacture constraints, and visual effects. Each neuron-shaped panel has several “synapses” which bear the pressure between the panels. The boundaries of synapses from adjacent panels make a continuous outline of a hole. These holes endow the entire surface with a unique pattern.

The panels are manufactured by Computer Numeric Control (CNC) machines. First, a milling machine cuts the panels out of the rectangular plywood sheets (25mm). Second, a Kuka 6-axis robot creates the “fingers” on the synapses of each panel, so that the adjacent panels can be firmly connect with their fingers. The design of fingers are tailored for robotic milling and pavilion’s in situ assembly. Both the G-code for driving the milling machine and the KRL sources files for driving the Kuka robot are created by the same Java program that generates the shell’s geometry. An open-source library http://javakuka.org is also published for programming Kuka robot in Java.

The Neuron pavilion shows the advantages of integrating computational design and digital fabrication. It features a continuous digital chain from early-stage design, form finding, structural optimization, to manufacture.

![](http://labaaa.org/wp-content/uploads/2017/09/neu2.jpg)

{% include elements/video.html id="jR8ESaD2EG8" %}

Neuron木构结合了运算化设计（Computational Design）和机器人制造（Robotic Fabrication）技术，在南京大学校园内建成了约7米跨度的新型木质构筑物。构件之间的连接完全由榫卯实现，无需钉子、胶水或螺栓固定。

设计团队在Java编程语言下开发了迭代优化算法，生成纯压力（表面无剪力）薄壳曲面，并结合现场庭院内的人流为构筑物设置了合理的开口位置与大小。整个曲面由61个形似神经元细胞（Neuron）的异形木构件组成。构件的设计充分考虑了力学性能、构造合理性、可加工性、视觉效果等因素。每个构件的“触角”用来传递构件之间的压力，而触角之间形成的孔洞在整个曲面上体现出独特的韵律。

![](http://labaaa.org/wp-content/uploads/2017/09/hua2.jpg)

所有木构件的制造都由数控加工完成：先由CNC（Computer Numeric Control）木工机从25mm桦木胶合板上切割出构件的轮廓，再由Kuka六轴机器人完成每个构件“触角”处的榫卯加工。全新的榫卯构造设计，一方面确保了连接的有效性和便捷性，另一方面充分结合了机器人铣削加工的特性。设计团队用Java程序输出木工机的G-code代码和Kuka机器人的KRL代码，并发布了http://javakuka.org开源代码库，完全实现了机器人运动编程的自主化。

Neuron木构的建成体现了数字化设计与智能制造相结合的优势，预示着建筑设计智能化和建造智能化的未来。该项目从头至尾无需任何（纸质或数字化）图纸，而是构建了从形态设计、结构优化、构筑设计到加工建造的数字化链条。

---

**指导：**[李飚](/people/libiao)，华好，唐芃

**助教：**梅琳丽，王嘉城， 刘宁琳，郭翰宸，李鸿渐

**学员：**王浩哲，徐沙，谢江涛，刘上，[莫怡晨](/people/moyichen)，吴帆，文涵，陈硕，熊攀

**视频：**王笑，陈今子

**技术支持：**南京耀阳科技有限公司，上海欣志机器人系统有限公司

---


{% include elements/button-top.html %}
