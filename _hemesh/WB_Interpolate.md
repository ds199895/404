---
navs: []
tags: [Math]
image:
title: WB_Interpolate
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
            


### WB_Interpolate

<br>


- **构造方法**

| 属性   | 方法名            | 参数   | 返回值            | 备注   |
|:-----|:---------------|:-----|:---------------|:-----|
|      | WB_Interpolate | ()   | WB_Interpolate |      |

- **成员方法**

| 属性     | 方法名                          | 参数                                                                                                                                                      | 返回值    | 备注   |
|:-------|:-----------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------|:-------|:-----|
| static | linearInterpolate            | final double v1, final double v2, final double alpha                                                                                                    | double |      |
| static | cosineInterpolate            | final double v1, final double v2, final double alpha                                                                                                    | double |      |
| static | cubicInterpolate             | final double v0, final double v1, final double v2, final double v3,final double alpha                                                                   | double |      |
| static | hermiteInterpolate           | final double v0, final double v1, final double v2, final double v3,final double alpha, final double tension, final double bias                          | double |      |
| static | kochanekBartelsInterpolator  | final double v0, final double v1, final double v2, final double v3,final double alpha, final double tension, final double continuity, final double bias | double |      |
| static | quadraticBezierInterpolator  | final double v0, final double v1, final double v2,final double alpha                                                                                    | double |      |
| static | cubicBezierInterpolator      | final double v0, final double v1, final double v2, final double v3,final double alpha                                                                   | double |      |
| static | quadraticBSplineInterpolator | final double v0, final double v1, final double v2,final double alpha                                                                                    | double |      |
| static | cubicBSplineInterpolator     | final double v0, final double v1, final double v2, final double v3,final double alpha                                                                   | double |      |
| static | cubicCatmullRomInterpolator  | final double v0, final double v1, final double v2, final double v3,final double alpha                                                                   | double |      |
| static | cubicHermiteInterpolator     | final double v0, final double v1, final double v2, final double v3,final double alpha                                                                   | double |      |