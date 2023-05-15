---
navs: []
tags: [He_creators,primitives]
image:
title: HEC_Cube
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
  var referrer ='HEC_Cube';
  localStorage.setItem('referrer', referrer);
}
</script>

<br>

### HEC_Cube

<br>
#### extends:   [HEC_Creator]({{site.baseurl}}/hemesh/hec-creator)
<br>


- **构造方法**

| 属性   | 方法名      | 参数                                                    | 返回值      | 备注   |
|:-----|:---------|:------------------------------------------------------|:---------|:-----|
|      | HEC_Cube | ()                                                    | HEC_Cube |      |
|      | HEC_Cube | final double W, final int L, final int M, final int N | HEC_Cube |      |

- **成员方法**

| 属性   | 方法名               | 参数             | 返回值      | 备注   |
|:-----|:------------------|:---------------|:---------|:-----|
|      | setEdge           | final double E | HEC_Cube |      |
|      | setWidthSegments  | final int L    | HEC_Cube |      |
|      | setHeightSegments | final int M    | HEC_Cube |      |
|      | setDepthSegments  | final int N    | HEC_Cube |      |
|      | setRadius         | final double R | HEC_Cube |      |
|      | setInnerRadius    | final double R | HEC_Cube |      |
|      | setOuterRadius    | final double R | HEC_Cube |      |
|      | setMidRadius      | final double R | HEC_Cube |      |
|      | createBase        | ()             | HE_Mesh  |      |