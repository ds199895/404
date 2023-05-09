---
navs: []
tags: [He_creators,primitives]
image:
title: HEC_Torus
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
  var referrer ='HEC_Torus';
  localStorage.setItem('referrer', referrer);
}
</script>

<br>

### HEC_Torus

<br>
#### extends:   [HEC_Creator](/hemesh/hec-creator)
<br>


- **构造方法**

| 属性   | 方法名       | 参数                                                                                               | 返回值       | 备注   |
|:-----|:----------|:-------------------------------------------------------------------------------------------------|:----------|:-----|
|      | HEC_Torus | ()                                                                                               | HEC_Torus |      |
|      | HEC_Torus | final double Ri, final double Ro, final int tubefacets, final int torusfacets                    | HEC_Torus |      |
|      | HEC_Torus | final double Rix, final double Riz, final double Ro, final int tubefacets, final int torusfacets | HEC_Torus |      |

- **成员方法**

| 属性   | 方法名            | 参数                                                         | 返回值       | 备注   |
|:-----|:---------------|:-----------------------------------------------------------|:----------|:-----|
|      | setRadius      | final double Ri, final double Ro                           | HEC_Torus |      |
|      | setRadius      | final double Rix, final double Riz, final double Ro        | HEC_Torus |      |
|      | setTorusRadius | final double Ro                                            | HEC_Torus |      |
|      | setTubeRadius  | final double Ri                                            | HEC_Torus |      |
|      | setTubeRadius  | final double Rix, final double Riz                         | HEC_Torus |      |
|      | setTorusRadius | final WB_ScalarParameter Ro                                | HEC_Torus |      |
|      | setTubeRadius  | final WB_ScalarParameter Ri                                | HEC_Torus |      |
|      | setTubeRadius  | final WB_ScalarParameter Rix, final WB_ScalarParameter Riz | HEC_Torus |      |
|      | setTubeFacets  | final int facets                                           | HEC_Torus |      |
|      | setTorusFacets | final int facets                                           | HEC_Torus |      |
|      | setTwist       | final int t                                                | HEC_Torus |      |
|      | setTorusPhase  | final double p                                             | HEC_Torus |      |
|      | setTubePhase   | final double p                                             | HEC_Torus |      |
|      | setTubePhase   | final WB_ScalarParameter p                                 | HEC_Torus |      |
|      | createBase     | ()                                                         | HE_Mesh   |      |