---
navs: []
tags: [He_creators,primitives]
image:
title: HEC_Ring
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
  var referrer ='HEC_Ring';
  localStorage.setItem('referrer', referrer);
}
</script>

<br>

### HEC_Ring

<br>
#### extends:   [HEC_Creator](/hemesh/hec-creator)
<br>


- **构造方法**

| 属性   | 方法名      | 参数   | 返回值      | 备注   |
|:-----|:---------|:-----|:---------|:-----|
|      | HEC_Ring | ()   | HEC_Ring |      |

- **成员方法**

| 属性   | 方法名          | 参数                               | 返回值      | 备注   |
|:-----|:-------------|:---------------------------------|:---------|:-----|
|      | setRadius    | final double ir, final double or | HEC_Ring |      |
|      | setPhase     | final double phase               | HEC_Ring |      |
|      | setN         | final int N                      | HEC_Ring |      |
|      | setCenter    | final WB_Coord center            | HEC_Ring |      |
|      | setNormal    | final WB_Coord normal            | HEC_Ring |      |
|      | setThickness | final double thickness           | HEC_Ring |      |
|      | setOffset    | final double offset              | HEC_Ring |      |
|      | createBase   | ()                               | HE_Mesh  |      |