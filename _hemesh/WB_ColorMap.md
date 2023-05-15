---
navs: []
tags: [Processing]
image:
title: WB_ColorMap
title_cn:
description: 
team: [Siyuan He]
status: Doing
year: 2023
date: 2023-05-15
---
<style>
table th:first-of-type {
width:5%;
}
table th:nth-of-type(2) {
width:20%;
}
table th:nth-of-type(3) {
width:30%;
}
table th:nth-of-type(4) {
width:30%;
}
table th:nth-of-type(5) {
width:8cm;
}
table th {
color: rgba(0,0,0)!important;
font-weight: bold; /*加粗*/
/* text-align: center !important; 内容居中，加上 !important 避免被 Markdown 样式覆盖 */
background: rgba(224,229,223,10)!important; /*背景色*/
}
</style>
            


### WB_ColorMap

<br>

该类无方法，需自行确认

### AbstractColorMap

<br>
#### implements:   [WB_ColorMap]({{site.baseurl}}/hemesh/wb-colormap)
<br>


- **成员方法**

| 属性   | 方法名       | 参数                                                | 返回值    | 备注   |
|:-----|:----------|:--------------------------------------------------|:-------|:-----|
|      | color     | int v1, int v2, int v3                            | int    |      |
|      | normColor | final double v1, final double v2, final double v3 | int    |      |
|      | lookup    | final double x, final double[][] values           | double |      |
|      | gfunc0    | final double x                                    | double |      |
|      | gfunc1    | final double x                                    | double |      |
|      | gfunc2    | final double x                                    | double |      |
|      | gfunc3    | final double x                                    | double |      |
|      | gfunc4    | final double x                                    | double |      |
|      | gfunc5    | final double x                                    | double |      |
|      | gfunc6    | final double x                                    | double |      |
|      | gfunc7    | final double x                                    | double |      |
|      | gfunc8    | final double x                                    | double |      |
|      | gfunc9    | final double x                                    | double |      |
|      | gfunc10   | final double x                                    | double |      |
|      | gfunc11   | final double x                                    | double |      |
|      | gfunc12   | final double x                                    | double |      |
|      | gfunc13   | final double x                                    | double |      |
|      | gfunc14   | final double x                                    | double |      |
|      | gfunc15   | final double x                                    | double |      |
|      | gfunc16   | final double x                                    | double |      |
|      | gfunc17   | final double x                                    | double |      |
|      | gfunc18   | final double x                                    | double |      |
|      | gfunc19   | final double x                                    | double |      |
|      | gfunc20   | final double x                                    | double |      |
|      | gfunc21   | final double x                                    | double |      |
|      | gfunc22   | final double x                                    | double |      |
|      | gfunc23   | final double x                                    | double |      |
|      | gfunc24   | final double x                                    | double |      |
|      | gfunc25   | final double x                                    | double |      |
|      | gfunc26   | final double x                                    | double |      |
|      | gfunc27   | final double x                                    | double |      |
|      | gfunc28   | final double x                                    | double |      |
|      | gfunc29   | final double x                                    | double |      |
|      | gfunc30   | final double x                                    | double |      |
|      | gfunc31   | final double x                                    | double |      |
|      | gfunc32   | final double x                                    | double |      |
|      | gfunc33   | final double x                                    | double |      |
|      | gfunc34   | final double x                                    | double |      |
|      | gfunc35   | final double x                                    | double |      |
|      | gfunc36   | final double x                                    | double |      |

### Binary

<br>
#### extends:  AbstractColorMap
<br>


- **成员方法**

| 属性   | 方法名      | 参数             | 返回值   | 备注   |
|:-----|:---------|:---------------|:------|:-----|
|      | getColor | final double f | int   |      |

### Autumn

<br>
#### extends:  AbstractColorMap
<br>


- **成员方法**

| 属性   | 方法名      | 参数             | 返回值   | 备注   |
|:-----|:---------|:---------------|:------|:-----|
|      | getColor | final double f | int   |      |

### Winter

<br>
#### extends:  AbstractColorMap
<br>


- **成员方法**

| 属性   | 方法名      | 参数             | 返回值   | 备注   |
|:-----|:---------|:---------------|:------|:-----|
|      | getColor | final double f | int   |      |

### Spring

<br>
#### extends:  AbstractColorMap
<br>


- **成员方法**

| 属性   | 方法名      | 参数             | 返回值   | 备注   |
|:-----|:---------|:---------------|:------|:-----|
|      | getColor | final double f | int   |      |

### Summer

<br>
#### extends:  AbstractColorMap
<br>


- **成员方法**

| 属性   | 方法名      | 参数             | 返回值   | 备注   |
|:-----|:---------|:---------------|:------|:-----|
|      | getColor | final double f | int   |      |

### Bone

<br>
#### extends:  AbstractColorMap
<br>


- **成员方法**

| 属性   | 方法名      | 参数             | 返回值   | 备注   |
|:-----|:---------|:---------------|:------|:-----|
|      | getColor | final double f | int   |      |

### Cool

<br>
#### extends:  AbstractColorMap
<br>


- **成员方法**

| 属性   | 方法名      | 参数             | 返回值   | 备注   |
|:-----|:---------|:---------------|:------|:-----|
|      | getColor | final double f | int   |      |

### Copper

<br>
#### extends:  AbstractColorMap
<br>


- **成员方法**

| 属性   | 方法名      | 参数             | 返回值   | 备注   |
|:-----|:---------|:---------------|:------|:-----|
|      | getColor | final double f | int   |      |

### Flag

<br>
#### extends:  AbstractColorMap
<br>


- **成员方法**

| 属性   | 方法名      | 参数             | 返回值   | 备注   |
|:-----|:---------|:---------------|:------|:-----|
|      | getColor | final double f | int   |      |

### Prism

<br>
#### extends:  AbstractColorMap
<br>


- **成员方法**

| 属性   | 方法名      | 参数             | 返回值   | 备注   |
|:-----|:---------|:---------------|:------|:-----|
|      | getColor | final double f | int   |      |

### GnuPlot

<br>
#### extends:  AbstractColorMap
<br>


- **成员方法**

| 属性   | 方法名      | 参数             | 返回值   | 备注   |
|:-----|:---------|:---------------|:------|:-----|
|      | getColor | final double f | int   |      |

### GnuPlot2

<br>
#### extends:  AbstractColorMap
<br>


- **成员方法**

| 属性   | 方法名      | 参数             | 返回值   | 备注   |
|:-----|:---------|:---------------|:------|:-----|
|      | getColor | final double f | int   |      |

### Ocean

<br>
#### extends:  AbstractColorMap
<br>


- **成员方法**

| 属性   | 方法名      | 参数             | 返回值   | 备注   |
|:-----|:---------|:---------------|:------|:-----|
|      | getColor | final double f | int   |      |

### Afmhot

<br>
#### extends:  AbstractColorMap
<br>


- **成员方法**

| 属性   | 方法名      | 参数             | 返回值   | 备注   |
|:-----|:---------|:---------------|:------|:-----|
|      | getColor | final double f | int   |      |

### Rainbow

<br>
#### extends:  AbstractColorMap
<br>


- **成员方法**

| 属性   | 方法名      | 参数             | 返回值   | 备注   |
|:-----|:---------|:---------------|:------|:-----|
|      | getColor | final double f | int   |      |

### Seismic

<br>
#### extends:  AbstractColorMap
<br>


- **成员方法**

| 属性   | 方法名      | 参数             | 返回值   | 备注   |
|:-----|:---------|:---------------|:------|:-----|
|      | getColor | final double f | int   |      |