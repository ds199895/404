---
navs: []
tags: [Geom]
image:
title: WB_CoordOp2D
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
            


### WB_CoordOp2D

<br>


- **成员方法**

| 属性     | 方法名             | 参数                                                                                                                                    | 返回值    | 备注   |
|:-------|:----------------|:--------------------------------------------------------------------------------------------------------------------------------------|:-------|:-----|
| static | boolean         | final WB_Circle C1, final WB_Circle C2                                                                                                | final  |      |
| static | double          | final WB_Coord v1, final WB_Coord v2                                                                                                  | final  |      |
| static | double          | final double ux, final double uy, final double vx, final double vy                                                                    | final  |      |
| static | double          | final WB_Coord u, final WB_Coord v                                                                                                    | final  |      |
| static | double          | final double ux, final double uy, final double vx, final double vy                                                                    | final  |      |
| static | double          | final double cx, final double cy, final double px, final double py,final double qx, final double qy                                   | final  |      |
| static | double          | final WB_Coord u, final WB_Coord v                                                                                                    | final  |      |
| static | double          | final WB_Coord c, final WB_Coord p, final WB_Coord q                                                                                  | final  |      |
| static | double          | final double ux, final double uy, final double vx,final double vy                                                                     | final  |      |
| static | double          | final WB_Coord u, final WB_Coord v                                                                                                    | final  |      |
| static | double          | final double ux, final double uy, final double vx,final double vy                                                                     | final  |      |
| static | double          | final double cx, final double cy, final double px, final double py,final double qx, final double qy                                   | final  |      |
| static | double          | final double ux, final double uy, final double vx,final double vy                                                                     | final  |      |
| static | double          | final double px, final double py, final double qx, final double qy                                                                    | final  |      |
| static | double          | final WB_Coord p, final WB_Coord q                                                                                                    | final  |      |
| static | double          | final double ux, final double uy                                                                                                      | final  |      |
| static | double          | final WB_Coord p                                                                                                                      | final  |      |
| static | double          | final double ux, final double uy, final double vx,final double vy, final double nx, final double ny                                   | final  |      |
| static | double          | final double cx, final double cy, final double px,final double py, final double qx, final double qy, final double nx, final double ny | final  |      |
| static | double          | final double ux, final double uy, final double vx,final double vy, final double nx, final double ny                                   | final  |      |
| static | double          | final double px, final double py, final double qx, final double qy                                                                    | final  |      |
| static | double          | final WB_Coord p, final WB_Coord q                                                                                                    | final  |      |
| static | double          | final double ux, final double uy                                                                                                      | final  |      |
| static | double          | final WB_Coord p                                                                                                                      | final  |      |
| static | double[]        | final double px, final double py, final double qx, final double qy,final double t                                                     | final  |      |
| static | double[]        | final WB_Coord p, final WB_Coord q, final double t                                                                                    | final  |      |
| static | boolean         | final WB_Coord a, final WB_Coord b                                                                                                    | final  |      |
| static | boolean         | final WB_Coord o, final WB_Coord p, final WB_Coord q                                                                                  | final  |      |
| static | boolean         | final WB_Coord v0, final WB_Coord v1                                                                                                  | final  |      |
| static | boolean         | final WB_Coord v0, final WB_Coord v1, final double epsilon                                                                            | final  |      |
| static | boolean         | final WB_Coord v0, final WB_Coord v1                                                                                                  | final  |      |
| static | boolean         | final WB_Coord v0, final WB_Coord v1, final double epsilon                                                                            | final  |      |
| static | boolean         | final WB_Coord v0, final WB_Coord v1                                                                                                  | final  |      |
| static | boolean         | final WB_Coord v0, final WB_Coord v1, final double epsilon                                                                            | final  |      |
| static | boolean         | final WB_Coord v0, final WB_Coord v1                                                                                                  | final  |      |
| static | boolean         | final WB_Coord v0, final WB_Coord v1, final double epsilon                                                                            | final  |      |
| static | boolean         | final double ux, final double uy                                                                                                      | final  |      |
| static | getDistance2D   | final WB_Coord p, final WB_AABB2D AABB                                                                                                | double |      |
| static | getSqDistance2D | final WB_Coord p, final WB_AABB2D AABB                                                                                                | double |      |