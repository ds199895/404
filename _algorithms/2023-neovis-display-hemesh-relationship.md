---
navs: [news,program,banner]
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
创建了一个分析和阅读程序类库的工作流。以Java图形库[HE_Mesh](https://github.com/wblut/HE_Mesh)的源代码为例，读取源码，进行分类，以静态网页的形式呈现。此外，在内部网络中还可以进行动态交互。
Created a workflow to analyze and read the source code of the Java graphics library [HE_Mesh](https://github.com/wblut/HE_Mesh), which was then presented in the form of a static webpage. Additionally, dynamic interaction is possible within internal network.


### 阅读并整理源代码

### Read and arrange the source code

使用Python阅读HE_Mesh包的源代码。利用开发平台的折叠代码机制为每行代码分配行号。使用字符处理获取该类的所有子类和方法，以及其子类的所有方法。
Read the source code of HE_Mesh package using Python. Utilize the folding code mechanism of the development platform to assign line numbers to each line of code. Use character processing to obtain all subclasses and methods of this class, as well as all methods of its subclasses.
![Display functions](https://archialgo-com-sources.oss-cn-hangzhou.aliyuncs.com/images/foldtest.jpg "Set Level")
<center>设置层级 Set Level</center>
### 显示源代码的功能

### Display the functions of source code

![Display functions](https://archialgo-com-sources.oss-cn-hangzhou.aliyuncs.com/images/functions.jpg "Display functions")

<center>显示函数 Display functions</center>
### 嵌入地图页面交互

### Embedded map page interaction

在Python中，除了读取该类的所有方法外，还通过字符拆分和搜索获取它继承和实现的所有类的名称。这些名称显示在类的专属页面上，并记录为数据输出的继承表。
In Python, in addition to reading all the methods of this class, you can also obtain the names of all the classes that it inherits from and implements by using character splitting and searching. These names are displayed on the class's display page and recorded as an inheritance table for data output.

继承表记录了类名、继承的类名以及子类数量（这会影响最终节点的大小）。这将被输入到 Neo4j 项目中，以建立知识图谱。
The inheritance table records the class name, inherited class name, and number of subclasses (which affects the size of the final node). This will be input into a Neo4j project to establish a knowledge graph. 

此外，静态网页将添加一个新的显示窗口，用于通过Cypher语句进行查询。有两种访问该页面的方式：一种是通过导航栏输入以直接显示所有类；另一种是单击每个类页面中的嵌入链接以显示与其他类的继承关系，渲染画布中的节点与箭头的形式可供修改，另外搜索的深度也可以进行调节。并且为了促进对每个类别的更深入理解，在显示窗口中嵌入了交互式功能，双击节点会显示其相应的继承关系。
Additionally, a novis display window will be added to the static webpage for querying through Cypher statements. There are two ways to access this information: one is by entering through the navigation bar to display all classes directly; and another is by clicking on each class's embedded link to show its inheritance relationship with adjustable depth and icons. To facilitate deeper understanding of each class, an interactive feature has been embedded in the display window where double-clicking on a node displays its corresponding inheritance relationship.
![ALL](https://archialgo-com-sources.oss-cn-hangzhou.aliyuncs.com/images/All.jpg "Load All")
<center>载入所有 Load All</center>
![One](https://archialgo-com-sources.oss-cn-hangzhou.aliyuncs.com/images/One.jpg "Load One")
<center>显示单个 Load One</center>
![Interaction](https://archialgo-com-sources.oss-cn-hangzhou.aliyuncs.com/images/interaction.gif "Double Click event")
<center>交互设计 Interaction</center>

{% include elements/button-top.html %}
