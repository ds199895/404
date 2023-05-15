---
navs: []
tags: [Processing]
image:
title: WB_Color
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
            


### WB_Color

<br>


- **成员方法**

| 属性     | 方法名                   | 参数                                                | 返回值       | 备注   |
|:-------|:----------------------|:--------------------------------------------------|:----------|:-----|
| static | color                 | int v1, int v2, int v3                            | int       |      |
| static | normColor             | final double v1, final double v2, final double v3 | int       |      |
| static | clamp                 | final double x                                    | double    |      |
| static | bump3y                | final WB_Vector x, final WB_Vector yoffset        | WB_Vector |      |
| static | spectralColorZucconi6 | final double wavelength                           | int       |      |