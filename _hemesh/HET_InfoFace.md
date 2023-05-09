---
navs: []
tags: [He_tools]
image:
title: HET_InfoFace
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
            


### HET_InfoFace

<br>

该类无方法，需自行确认

### HET_FaceNormal

<br>
#### implements:  HET_InfoFace&lt;WB_Vector&gt;
<br>


- **成员方法**

| 属性   | 方法名      | 参数                 | 返回值       | 备注   |
|:-----|:---------|:-------------------|:----------|:-----|
|      | retrieve | final HE_Face face | WB_Vector |      |

### HET_FaceCenter

<br>
#### implements:  HET_InfoFace&lt;WB_Point&gt;
<br>


- **成员方法**

| 属性   | 方法名      | 参数                 | 返回值      | 备注   |
|:-----|:---------|:-------------------|:---------|:-----|
|      | retrieve | final HE_Face face | WB_Point |      |

### HET_FaceArea

<br>
#### implements:  HET_InfoFace&lt;Double&gt;
<br>


- **成员方法**

| 属性   | 方法名      | 参数                 | 返回值    | 备注   |
|:-----|:---------|:-------------------|:-------|:-----|
|      | retrieve | final HE_Face face | Double |      |

### HET_FaceTriangles

<br>
#### implements:  HET_InfoFace&lt;int[]&gt;
<br>


- **成员方法**

| 属性   | 方法名      | 参数              | 返回值   | 备注   |
|:-----|:---------|:----------------|:------|:-----|
|      | retrieve | final HE_Face f | int[] |      |