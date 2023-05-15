---
navs: []
tags: [He_creators,primitives]
image:
title: HEC_Cylinder
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
  var referrer ='HEC_Cylinder';
  localStorage.setItem('referrer', referrer);
}
</script>

<br>

### HEC_Cylinder

<br>
#### extends:   [HEC_Creator]({{site.baseurl}}/hemesh/hec-creator)
<br>


- **构造方法**

| 属性   | 方法名          | 参数                                                                                  | 返回值          | 备注   |
|:-----|:-------------|:------------------------------------------------------------------------------------|:-------------|:-----|
|      | HEC_Cylinder | ()                                                                                  | HEC_Cylinder |      |
|      | HEC_Cylinder | final double Ri, final double Ro, final double H, final int facets, final int steps | HEC_Cylinder |      |

- **成员方法**

| 属性   | 方法名            | 参数                                             | 返回值          | 备注   |
|:-----|:---------------|:-----------------------------------------------|:-------------|:-----|
|      | setRadius      | final double R                                 | HEC_Cylinder |      |
|      | setRadius      | final double Ri, final double Ro               | HEC_Cylinder |      |
|      | setHeight      | final double H                                 | HEC_Cylinder |      |
|      | setSteps       | final int steps                                | HEC_Cylinder |      |
|      | setFacets      | final int facets                               | HEC_Cylinder |      |
|      | setCap         | final boolean topcap, final boolean bottomcap  | HEC_Cylinder |      |
|      | setProfile     | final WB_ScalarParameter t                     | HEC_Cylinder |      |
|      | setTaper       | final WB_ScalarParameter t                     | HEC_Cylinder |      |
|      | setPhase       | final double p                                 | HEC_Cylinder |      |
|      | setHeightTaper | final WB_ScalarParameter t                     | HEC_Cylinder |      |
|      | align          | final WB_Coord direction                       | HEC_Cylinder |      |
|      | align          | final WB_Coord origin, final WB_Coord endpoint | HEC_Cylinder |      |
|      | align          | final WB_Segment segment                       | HEC_Cylinder |      |
|      | createBase     | ()                                             | HE_Mesh      |      |