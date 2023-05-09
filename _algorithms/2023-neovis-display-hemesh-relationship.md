---
navs: [news,program]
tags: [Data Analysis, Neo4j]
image: https://archialgo-com-sources.oss-cn-hangzhou.aliyuncs.com/images/neo4j.jpg
title: Extending and implementing graph using NeoVis
title_cn: 基于NeoVis的HE_Mesh类库继承图谱
year: 2023
description: Created a workflow to analyze and read the source code of the Java graphics library HE_Mesh, which was then presented in the form of a static webpage. Additionally, dynamic interaction is possible within our internal network.
team: [He Siyuan]
status: Done🙌
date: 2022-06-30
---
---
<!-- # Shopping Mall Planning Generator -->
Created a workflow to analyze and read the source code of the Java graphics library [HE_Mesh](https://github.com/wblut/HE_Mesh), which was then presented in the form of a static webpage. Additionally, dynamic interaction is possible within internal network.

### Read and arrange the source code
Read the source code of HE_Mesh package using Python. Utilize the folding code mechanism of the development platform to assign line numbers to each line of code. Use character processing to obtain all subclasses and methods of this class, as well as all methods of its subclasses.
![Display functions](https://archialgo-com-sources.oss-cn-hangzhou.aliyuncs.com/images/foldtest.jpg "Set Level")

### Display the functions of source code

![Display functions](https://archialgo-com-sources.oss-cn-hangzhou.aliyuncs.com/images/functions.jpg "Display functions")

### Embedded map page interaction
In Python, in addition to reading all the methods of this class, you can also obtain the names of all the classes that it inherits from and implements by using character splitting and searching. These names are displayed on the class's display page and recorded as an inheritance table for data output.

The inheritance table records the class name, inherited class name, and number of subclasses (which affects the size of the final node). This will be input into a Neo4j project to establish a knowledge graph. 

Additionally, a novis display window will be added to the static webpage for querying through Cypher statements. There are two ways to access this information: one is by entering through the navigation bar to display all classes directly; and another is by clicking on each class's embedded link to show its inheritance relationship with adjustable depth and icons. To facilitate deeper understanding of each class, an interactive feature has been embedded in the display window where double-clicking on a node displays its corresponding inheritance relationship.
![ALL](https://archialgo-com-sources.oss-cn-hangzhou.aliyuncs.com/images/All.jpg "Load All")
![One](https://archialgo-com-sources.oss-cn-hangzhou.aliyuncs.com/images/One.jpg "Load One")
![Interaction](https://archialgo-com-sources.oss-cn-hangzhou.aliyuncs.com/images/interaction.gif "Double Click event")

{% include elements/button-top.html %}
