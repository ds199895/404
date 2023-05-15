---
navs: []
tags: [Geom]
image:
title: WB_CoordOp
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
            


### WB_CoordOp

<br>


- **构造方法**

| 属性   | 方法名        | 参数   | 返回值        | 备注   |
|:-----|:-----------|:-----|:-----------|:-----|
|      | WB_CoordOp | ()   | WB_CoordOp |      |

- **成员方法**

| 属性     | 方法名                    | 参数                                                                                                                                                     | 返回值        | 备注   |
|:-------|:-----------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------|:-----------|:-----|
| static | cross                  | final double ux, final double uy, final double uz, final double vx, final double vy,final double vz                                                    | double[]   |      |
| static | cross                  | final double cx, final double cy, final double cz, final double px, final double py,final double pz, final double qx, final double qy, final double qz | double[]   |      |
| static | dot                    | final double ux, final double uy, final double uz, final double vx, final double vy,final double vz                                                    | double     |      |
| static | getAngleBetween        | final double ux, final double uy, final double uz, final double vx,final double vy, final double vz                                                    | double     |      |
| static | getAngleBetween        | final double cx, final double cy, final double cz, final double px,final double py, final double pz, final double qx, final double qy, final double qz | double     |      |
| static | getAngleBetweenNorm    | final double ux, final double uy, final double uz, final double vx,final double vy, final double vz                                                    | double     |      |
| static | getCosAngleBetween     | final double ux, final double uy, final double uz, final double vx,final double vy, final double vz                                                    | double     |      |
| static | getCosAngleBetween     | final double cx, final double cy, final double cz, final double px,final double py, final double pz, final double qx, final double qy, final double qz | double     |      |
| static | getCosAngleBetweenNorm | final double ux, final double uy, final double uz, final double vx,final double vy, final double vz                                                    | double     |      |
| static | getDistance3D          | final double px, final double py, final double pz, final double qx,final double qy, final double qz                                                    | double     |      |
| static | getDistance3D          | final WB_Coord p, final WB_Coord q                                                                                                                     | double     |      |
| static | getLength3D            | final double ux, final double uy, final double uz                                                                                                      | double     |      |
| static | getLength3D            | final WB_Coord p                                                                                                                                       | double     |      |
| static | getSqDistance3D        | final double px, final double py, final double pz, final double qx,final double qy, final double qz                                                    | double     |      |
| static | getSqDistance3D        | final WB_Coord p, final WB_Coord q                                                                                                                     | double     |      |
| static | getSqLength3D          | final double ux, final double uy, final double uz                                                                                                      | double     |      |
| static | getSqLength3D          | final WB_Coord p                                                                                                                                       | double     |      |
| static | interpolate            | final double px, final double py, final double qx, final double qy,final double t                                                                      | double[]   |      |
| static | interpolate            | final double px, final double py, final double pz, final double qx,final double qy, final double qz, final double t                                    | double[]   |      |
| static | isCollinear            | final WB_Coord o, final WB_Coord p, final WB_Coord q                                                                                                   | boolean    |      |
| static | isOrthogonal           | final WB_Coord v0, final WB_Coord v1                                                                                                                   | boolean    |      |
| static | isOrthogonal           | final WB_Coord v0, final WB_Coord v1, final double epsilon                                                                                             | boolean    |      |
| static | isOrthogonalNorm       | final WB_Coord v0, final WB_Coord v1                                                                                                                   | boolean    |      |
| static | isOrthogonalNorm       | final WB_Coord v0, final WB_Coord v1, final double epsilon                                                                                             | boolean    |      |
| static | isParallel             | final WB_Coord v0, final WB_Coord v1                                                                                                                   | boolean    |      |
| static | isParallel             | final WB_Coord v0, final WB_Coord v1, final double epsilon                                                                                             | boolean    |      |
| static | isParallelNorm         | final WB_Coord v0, final WB_Coord v1                                                                                                                   | boolean    |      |
| static | isParallelNorm         | final WB_Coord v0, final WB_Coord v1, final double epsilon                                                                                             | boolean    |      |
| static | isParallelNormX        | final WB_Coord o, final WB_Coord p                                                                                                                     | boolean    |      |
| static | isParallelNormX        | final WB_Coord o, final WB_Coord p, final double t                                                                                                     | boolean    |      |
| static | isParallelX            | final WB_Coord o, final WB_Coord p                                                                                                                     | boolean    |      |
| static | isParallelX            | final WB_Coord o, final WB_Coord p, final double t                                                                                                     | boolean    |      |
| static | isZero3D               | final double ux, final double uy, final double uz                                                                                                      | boolean    |      |
| static | scalarTriple           | final double ux, final double uy, final double uz, final double vx,final double vy, final double vz, final double wx, final double wy, final double wz | double     |      |
| static | tensor3D               | final double ux, final double uy, final double uz, final double vx,final double vy, final double vz                                                    | double[][] |      |
| static | getDistance3D          | final WB_Coord p, final WB_AABB AABB                                                                                                                   | double     |      |
| static | getSqDistance3D        | final WB_Coord p, final WB_AABB AABB                                                                                                                   | double     |      |