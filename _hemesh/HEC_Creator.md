---
navs: []
tags: [He_creators]
image:
title: HEC_Creator
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
  var referrer ='HEC_Creator';
  localStorage.setItem('referrer', referrer);
}
</script>

<br>

### HEC_Creator

<br>
#### extends:   [HE_Machine]({{site.baseurl}}/hemesh/he-machine)
<br>


- **构造方法**

| 属性   | 方法名         | 参数   | 返回值         | 备注   |
|:-----|:------------|:-----|:------------|:-----|
|      | HEC_Creator | ()   | HEC_Creator |      |

- **成员方法**

| 属性   | 方法名                          | 参数                                                                                                        | 返回值         | 备注   |
|:-----|:-----------------------------|:----------------------------------------------------------------------------------------------------------|:------------|:-----|
|      | getCenter                    | ()                                                                                                        | WB_Point    |      |
|      | getZAxis                     | ()                                                                                                        | WB_Vector   |      |
|      | getVerticalAxis              | ()                                                                                                        | WB_Vector   |      |
|      | getRotationAngle             | ()                                                                                                        | double      |      |
|      | getScale                     | ()                                                                                                        | double      |      |
|      | getModelView                 | ()                                                                                                        | boolean     |      |
|      | getHome                      | ()                                                                                                        | PApplet     |      |
|      | getCheckManifold             | ()                                                                                                        | boolean     |      |
|      | getOverride                  | ()                                                                                                        | boolean     |      |
|      | getModelViewOverride         | ()                                                                                                        | boolean     |      |
|      | getCheckNormals              | ()                                                                                                        | boolean     |      |
|      | getCleanUnconnectedElements  | ()                                                                                                        | boolean     |      |
|      | getRemoveUnconnectedElements | ()                                                                                                        | boolean     |      |
|      | setCenter                    | final double x, final double y, final double z                                                            | HEC_Creator |      |
|      | setCenter                    | final WB_Coord c                                                                                          | HEC_Creator |      |
|      | setScale                     | final double s                                                                                            | HEC_Creator |      |
|      | setZAngle                    | final double a                                                                                            | HEC_Creator |      |
|      | setZAxis                     | final double x, final double y, final double z                                                            | HEC_Creator |      |
|      | setZAxis                     | final double p0x, final double p0y, final double p0z, final double p1x,final double p1y, final double p1z | HEC_Creator |      |
|      | setZAxis                     | final WB_Coord p                                                                                          | HEC_Creator |      |
|      | setZAxis                     | final WB_Coord p0, final WB_Coord p1                                                                      | HEC_Creator |      |
|      | setVerticalAxis              | final double x, final double y, final double z                                                            | HEC_Creator |      |
|      | setVerticalAxis              | final double p0x, final double p0y, final double p0z, final double p1x,final double p1y, final double p1z | HEC_Creator |      |
|      | setVerticalAxis              | WB_Coord axis                                                                                             | HEC_Creator |      |
|      | setVerticalAxis              | final WB_Coord p0, final WB_Coord p1                                                                      | HEC_Creator |      |
|      | setToModelview               | final PApplet home                                                                                        | HEC_Creator |      |
|      | setToModelview               | final WB_Transform3D T                                                                                    | HEC_Creator |      |
|      | setToModelview               | final WB_CoordinateSystem CS                                                                              | HEC_Creator |      |
|      | setToWorldview               | ()                                                                                                        | HEC_Creator |      |
|      | setCheckManifold             | final boolean b                                                                                           | HEC_Creator |      |
|      | setOverride                  | final boolean b                                                                                           | HEC_Creator |      |
|      | setModelViewOverride         | final boolean b                                                                                           | HEC_Creator |      |
|      | setCheckNormals              | final boolean b                                                                                           | HEC_Creator |      |
|      | setRemoveUnconnectedElements | final boolean b                                                                                           | HEC_Creator |      |
|      | HE_Mesh                      | ()                                                                                                        | final       |      |
|      | apply                        | final HE_Mesh mesh                                                                                        | HE_Mesh     |      |
|      | apply                        | final HE_Selection sel                                                                                    | HE_Mesh     |      |