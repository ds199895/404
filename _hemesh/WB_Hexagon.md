---
navs: []
tags: [Geom,polygon]
image:
title: WB_Hexagon
title_cn:
description: 
team: [Siyuan He]
status: Doing
year: 2023
date: 2023-04-03
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
<a href="/display/hemesh" onclick="saveReferrer()">继承关系图谱display</a>
<script>
function saveReferrer() {
  var referrer ='WB_Hexagon';
  localStorage.setItem('referrer', referrer);
}
</script>

<br>

### WB_Hexagon

<br>
#### implements:   [WB_Geometry](/hemesh/wb-geometry)
<br>


- **构造方法**

| 属性   | 方法名        | 参数                                                                                                              | 返回值        | 备注   |
|:-----|:-----------|:----------------------------------------------------------------------------------------------------------------|:-----------|:-----|
|      | WB_Hexagon | final WB_Coord p1, final WB_Coord p2, final WB_Coord p3,final WB_Coord p4, final WB_Coord p5, final WB_Coord p6 | WB_Hexagon |      |

- **成员方法**

| 属性   | 方法名         | 参数               | 返回值        | 备注   |
|:-----|:------------|:-----------------|:-----------|:-----|
|      | cycle       | ()               | void       |      |
|      | cycle       | int n            | void       |      |
|      | apply2D     | WB_Transform2D T | WB_Hexagon |      |
|      | apply2DSelf | WB_Transform2D T | WB_Hexagon |      |
|      | apply       | WB_Transform3D T | WB_Hexagon |      |
|      | applySelf   | WB_Transform3D T | WB_Hexagon |      |