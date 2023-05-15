---
navs: []
tags: [He_modifiers]
image:
title: HEM_MultiSlice
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
  var referrer ='HEM_MultiSlice';
  localStorage.setItem('referrer', referrer);
}
</script>

<br>

### HEM_MultiSlice

<br>
#### extends:   [HEM_Modifier]({{site.baseurl}}/hemesh/hem-modifier)
<br>


- **构造方法**

| 属性   | 方法名            | 参数   | 返回值            | 备注   |
|:-----|:---------------|:-----|:---------------|:-----|
|      | HEM_MultiSlice | ()   | HEM_MultiSlice |      |

- **成员方法**

| 属性   | 方法名            | 参数                                | 返回值            | 备注   |
|:-----|:---------------|:----------------------------------|:---------------|:-----|
|      | setOffset      | final double d                    | HEM_MultiSlice |      |
|      | setPlanes      | final Collection<WB_Plane> planes | HEM_MultiSlice |      |
|      | setPlanes      | final WB_Plane[] planes           | HEM_MultiSlice |      |
|      | setLabels      | final int[] labels                | HEM_MultiSlice |      |
|      | setReverse     | final Boolean b                   | HEM_MultiSlice |      |
|      | setCenter      | final WB_Point c                  | HEM_MultiSlice |      |
|      | setTriangulate | final boolean b                   | HEM_MultiSlice |      |
|      | setCap         | final Boolean b                   | HEM_MultiSlice |      |
|      | setOptimizeCap | final boolean b                   | HEM_MultiSlice |      |
|      | applySelf      | final HE_Mesh mesh                | HE_Mesh        |      |
|      | applySelf      | final HE_Selection selection      | HE_Mesh        |      |