---
navs: []
tags: [Nurbs]
image:
title: WB_NurbsFactory
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
            


### WB_NurbsFactory

<br>


- **成员方法**

| 属性     | 方法名                        | 参数                                                                             | 返回值                | 备注   |
|:-------|:---------------------------|:-------------------------------------------------------------------------------|:-------------------|:-----|
| static | getSurfaceOfRevolution     | final WB_BSpline C, final WB_Coord p, final WB_Coord axis,double theta         | WB_RBSplineSurface |      |
| static | getFullSurfaceOfRevolution | final WB_BSpline C, final WB_Coord p,final WB_Coord axis                       | WB_RBSplineSurface |      |
| static | getSurfaceOfRevolution     | final WB_RBSpline C, final WB_Coord p, final WB_Coord axis,double theta        | WB_RBSplineSurface |      |
| static | getFullSurfaceOfRevolution | final WB_RBSpline C, final WB_Coord p,final WB_Coord axis                      | WB_RBSplineSurface |      |
| static | getRuledSurface            | WB_BSpline CA, WB_BSpline CB                                                   | WB_BSplineSurface  |      |
| static | getRuledSurface            | WB_RBSpline CA, WB_RBSpline CB                                                 | WB_RBSplineSurface |      |
| static | getSwungSurface            | final WB_BSpline xzprofile, final WB_BSpline xytrajectory,final double alpha   | WB_BSplineSurface  |      |
| static | getSwungSurface            | final WB_BSpline xzprofile, final WB_RBSpline xytrajectory,final double alpha  | WB_RBSplineSurface |      |
| static | getSwungSurface            | final WB_RBSpline xzprofile, final WB_BSpline xytrajectory,final double alpha  | WB_RBSplineSurface |      |
| static | getSwungSurface            | final WB_RBSpline xzprofile, final WB_RBSpline xytrajectory,final double alpha | WB_RBSplineSurface |      |
| static | getLineSweep               | final WB_BSpline C, final WB_Coord v, final double f                           | WB_BSplineSurface  |      |
| static | getLineSweep               | final WB_RBSpline C, final WB_Coord v, final double f                          | WB_RBSplineSurface |      |