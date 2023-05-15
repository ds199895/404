---
navs: []
tags: [Geom,primitives]
image:
title: WB_Arc
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
            

<br>
<a href="{{site.baseurl}}/display/hemesh" onclick="saveReferrer()">继承关系图谱display</a>
<script>
function saveReferrer() {
  var referrer ='WB_Arc';
  localStorage.setItem('referrer', referrer);
}
</script>

<br>

### WB_Arc

<br>
#### implements:   [WB_Curve]({{site.baseurl}}/hemesh/wb-curve)
<br>


- **构造方法**

| 属性   | 方法名    | 参数                                            | 返回值    | 备注   |
|:-----|:-------|:----------------------------------------------|:-------|:-----|
|      | WB_Arc | WB_Coord start, WB_Coord end, WB_Coord center | WB_Arc |      |

- **成员方法**

| 属性   | 方法名                 | 参数                                             | 返回值        | 备注   |
|:-----|:--------------------|:-----------------------------------------------|:-----------|:-----|
|      | getRadius           | ()                                             | double     |      |
|      | getCenter           | ()                                             | WB_Coord   |      |
|      | getStart            | ()                                             | WB_Coord   |      |
|      | getEnd              | ()                                             | WB_Coord   |      |
|      | getNormal           | ()                                             | WB_Coord   |      |
|      | set                 | final WB_Arc c                                 | void       |      |
|      | setCenter           | final double x, final double y                 | void       |      |
|      | setCenter           | final double x, final double y, final double z | void       |      |
|      | setCenter           | final WB_Coord c                               | void       |      |
|      | setNormal           | final double x, final double y, final double z | void       |      |
|      | setNormal           | final WB_Coord c                               | void       |      |
|      | equals              | final Object o                                 | boolean    |      |
|      | hashCode            | ()                                             | int        |      |
|      | hashCode            | final double v                                 | int        |      |
|      | getPoints           | final int n, final double phase                | WB_Point[] |      |
|      | getPoints           | final int n                                    | WB_Point[] |      |
|      | getPointsAsArray    | final int n                                    | double[]   |      |
|      | getPlane            | ()                                             | WB_Plane   |      |
|      | getPlane            | final double d                                 | WB_Plane   |      |
|      | getPointOnCurve     | double u                                       | WB_Point   |      |
|      | getDirectionOnCurve | double u                                       | WB_Vector  |      |
|      | getDerivative       | double u                                       | WB_Vector  |      |
|      | getLowerU           | ()                                             | double     |      |
|      | getUpperU           | ()                                             | double     |      |