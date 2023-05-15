---
navs: []
tags: [Nurbs]
image:
title: WB_NurbsKnot
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
            


### WB_NurbsKnot

<br>


- **构造方法**

| 属性   | 方法名          | 参数                                                  | 返回值          | 备注   |
|:-----|:-------------|:----------------------------------------------------|:-------------|:-----|
|      | WB_NurbsKnot | final int ncp, final int degree                     | WB_NurbsKnot |      |
|      | WB_NurbsKnot | final int ncp, final int degree, final double[] val | WB_NurbsKnot |      |
|      | WB_NurbsKnot | final int degree, final double[] val                | WB_NurbsKnot |      |
|      | WB_NurbsKnot | final WB_NurbsKnot knot                             | WB_NurbsKnot |      |

- **成员方法**

| 属性     | 方法名               | 参数                                           | 返回值          | 备注   |
|:-------|:------------------|:---------------------------------------------|:-------------|:-----|
|        | p                 | ()                                           | int          |      |
|        | n                 | ()                                           | int          |      |
|        | m                 | ()                                           | int          |      |
|        | s                 | ()                                           | int          |      |
|        | toString          | ()                                           | String       |      |
|        | values            | ()                                           | double[]     |      |
|        | value             | final int i                                  | double       |      |
|        | setValue          | final int i, final double k                  | void         |      |
|        | span              | final double u                               | int          |      |
|        | multiplicity      | final double u                               | int          |      |
|        | multiplicity      | final double u, final int span               | int          |      |
|        | basisFunctions    | final int span, final double u               | double[]     |      |
|        | allBasisFunctions | final int span, final double u, final int p  | double[][]   |      |
|        | normalize         | ()                                           | void         |      |
| static | merge             | final WB_NurbsKnot UA, final WB_NurbsKnot UB | WB_NurbsKnot |      |
|        | multVal           | ()                                           | double[][]   |      |