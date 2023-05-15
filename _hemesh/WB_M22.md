---
navs: []
tags: [Math]
image:
title: WB_M22
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
            


### WB_M22

<br>


- **构造方法**

| 属性   | 方法名    | 参数                                                                                                                                                              | 返回值    | 备注   |
|:-----|:-------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------|:-------|:-----|
|      | WB_M22 | ()                                                                                                                                                              | WB_M22 |      |
|      | WB_M22 | final double[][] matrix33                                                                                                                                       | WB_M22 |      |
|      | WB_M22 | final double m11, final double m12, final double m13, final double m21, final double m22,final double m23, final double m31, final double m32, final double m33 | WB_M22 |      |

- **成员方法**

| 属性     | 方法名              | 参数                                                                                                                                                                                                       | 返回值        | 备注   |
|:-------|:-----------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-----------|:-----|
|        | set              | final double[][] matrix33                                                                                                                                                                                | void       |      |
|        | set              | final float[][] matrix33                                                                                                                                                                                 | void       |      |
|        | set              | final int[][] matrix33                                                                                                                                                                                   | void       |      |
|        | set              | final double m11, final double m12, final double m13, final double m21, final double m22,final double m23, final double m31, final double m32, final double m33                                          | void       |      |
|        | set              | final WB_M22 m                                                                                                                                                                                           | void       |      |
|        | get              | ()                                                                                                                                                                                                       | WB_M22     |      |
|        | row              | final int i                                                                                                                                                                                              | WB_Vector  |      |
|        | rowInto          | final int i, final WB_MutableCoord result                                                                                                                                                                | void       |      |
|        | col              | final int i                                                                                                                                                                                              | WB_Vector  |      |
|        | colInto          | final int i, final WB_MutableCoord result                                                                                                                                                                | void       |      |
|        | add              | final WB_M22 m                                                                                                                                                                                           | void       |      |
|        | sub              | final WB_M22 m                                                                                                                                                                                           | void       |      |
|        | mul              | final double f                                                                                                                                                                                           | void       |      |
|        | div              | final double f                                                                                                                                                                                           | void       |      |
|        | addInto          | final WB_M22 m, final WB_M22 result                                                                                                                                                                      | void       |      |
|        | subInto          | final WB_M22 m, final WB_M22 result                                                                                                                                                                      | void       |      |
|        | multInto         | final double f, final WB_M22 result                                                                                                                                                                      | void       |      |
|        | divInto          | final double f, final WB_M22 result                                                                                                                                                                      | void       |      |
| static | mul              | final WB_M22 m, final WB_M22 n                                                                                                                                                                           | WB_M22     |      |
| static | mulInto          | final WB_M22 m, final WB_M22 n, final WB_M22 result                                                                                                                                                      | void       |      |
|        | mul              | final WB_M22 n                                                                                                                                                                                           | WB_M22     |      |
|        | multInto         | final WB_M22 n, final WB_M22 result                                                                                                                                                                      | void       |      |
| static | mulInto          | final WB_M22 m, final WB_Coord v, final WB_MutableCoord result                                                                                                                                           | void       |      |
| static | mulInto          | final WB_Coord v, final WB_M22 m, final WB_MutableCoord result                                                                                                                                           | void       |      |
| static | mulToPoint       | final WB_M22 m, final WB_Coord v                                                                                                                                                                         | WB_Point   |      |
| static | mulToPoint       | final WB_Coord v, final WB_M22 m                                                                                                                                                                         | WB_Point   |      |
| static | mulToVector      | final WB_M22 m, final WB_Coord v                                                                                                                                                                         | WB_Vector  |      |
| static | mulToVector      | final WB_Coord v, final WB_M22 m                                                                                                                                                                         | WB_Vector  |      |
|        | det              | ()                                                                                                                                                                                                       | double     |      |
|        | transpose        | ()                                                                                                                                                                                                       | void       |      |
|        | getTranspose     | ()                                                                                                                                                                                                       | WB_M22     |      |
|        | transposeInto    | final WB_M22 result                                                                                                                                                                                      | void       |      |
|        | inverse          | ()                                                                                                                                                                                                       | WB_M22     |      |
| static | Cramer3          | final double a1, final double b1, final double c1, final double d1, final double a2,final double b2, final double c2, final double d2, final double a3, final double b3, final double c3,final double d3 | WB_Vector  |      |
|        | symSchur2        | final int p, final int q, final double[][] m                                                                                                                                                             | double[]   |      |
|        | Jacobi           | ()                                                                                                                                                                                                       | WB_M22     |      |
|        | toArray          | ()                                                                                                                                                                                                       | double[][] |      |
| static | covarianceMatrix | final WB_Coord[] points                                                                                                                                                                                  | WB_M22     |      |
|        | equals           | final Object o                                                                                                                                                                                           | boolean    |      |