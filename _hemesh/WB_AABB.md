---
navs: []
tags: [Geom,spatial]
image:
title: WB_AABB
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
            


### WB_AABB

<br>


- **构造方法**

| 属性   | 方法名     | 参数                                                                                                              | 返回值     | 备注   |
|:-----|:--------|:----------------------------------------------------------------------------------------------------------------|:--------|:-----|
|      | WB_AABB | final WB_Coord p                                                                                                | WB_AABB |      |
|      | WB_AABB | ()                                                                                                              | WB_AABB |      |
|      | WB_AABB | final WB_Coord[] points                                                                                         | WB_AABB |      |
|      | WB_AABB | final Collection<? extends WB_Coord> points                                                                     | WB_AABB |      |
|      | WB_AABB | final double[] min, final double[] max                                                                          | WB_AABB |      |
|      | WB_AABB | final float[] min, final float[] max                                                                            | WB_AABB |      |
|      | WB_AABB | final int[] min, final int[] max                                                                                | WB_AABB |      |
|      | WB_AABB | final WB_Coord min, final WB_Coord max                                                                          | WB_AABB |      |
|      | WB_AABB | final double minx, final double miny, final double maxx,final double maxy                                       | WB_AABB |      |
|      | WB_AABB | final double minx, final double miny, final double minz,final double maxx, final double maxy, final double maxz | WB_AABB |      |
|      | WB_AABB | final double[] values                                                                                           | WB_AABB |      |
|      | WB_AABB | final int[] values                                                                                              | WB_AABB |      |
|      | WB_AABB | final float[] values                                                                                            | WB_AABB |      |

- **成员方法**

| 属性     | 方法名               | 参数                                                                        | 返回值                  | 备注   |
|:-------|:------------------|:--------------------------------------------------------------------------|:---------------------|:-----|
|        | getSize           | final int i                                                               | double               |      |
|        | minOrdinate       | ()                                                                        | int                  |      |
|        | maxOrdinate       | ()                                                                        | int                  |      |
|        | expandToInclude   | final WB_Coord p                                                          | void                 |      |
|        | add               | final WB_Coord p                                                          | void                 |      |
|        | expandBy          | final double distance                                                     | void                 |      |
|        | expandBy          | final double[] delta                                                      | void                 |      |
|        | expandBy          | final double dx, final double dy, final double dz                         | void                 |      |
|        | expandToInclude   | final double[] p                                                          | void                 |      |
|        | expandToInclude   | final double x, final double y,final double z                             | void                 |      |
|        | expandToInclude   | final WB_AABB other                                                       | void                 |      |
|        | add               | final WB_AABB other                                                       | void                 |      |
|        | translate         | final double[] d                                                          | void                 |      |
|        | intersects        | final WB_AABB other                                                       | boolean              |      |
|        | intersects        | final WB_Coord p                                                          | boolean              |      |
|        | intersects        | final double[] x                                                          | boolean              |      |
|        | intersects        | final double x, final double y, final double z                            | boolean              |      |
|        | intersects        | final WB_Sphere sphere                                                    | boolean              |      |
|        | contains          | final WB_AABB other                                                       | boolean              |      |
|        | contains          | final WB_Coord p                                                          | boolean              |      |
|        | contains          | final double[] x                                                          | boolean              |      |
|        | covers            | final double[] x                                                          | boolean              |      |
|        | covers            | final double x, final double y, final double z                            | boolean              |      |
|        | covers            | final WB_Coord p                                                          | boolean              |      |
|        | covers            | final WB_AABB other                                                       | boolean              |      |
|        | getDistance       | final WB_AABB other                                                       | double               |      |
|        | getDistanceSquare | final WB_AABB other                                                       | double               |      |
|        | getDistance       | final WB_Coord tuple                                                      | double               |      |
|        | getDistanceSquare | final WB_Coord tuple                                                      | double               |      |
|        | equals            | final WB_AABB other                                                       | boolean              |      |
|        | toString          | ()                                                                        | String               |      |
|        | numberOfPoints    | ()                                                                        | int                  |      |
|        | numberOfSegments  | ()                                                                        | int                  |      |
|        | numberOfTriangles | ()                                                                        | int                  |      |
|        | numberOfFaces     | ()                                                                        | int                  |      |
|        | getCoords         | ()                                                                        | List&lt;double[]&gt; |      |
|        | getCorners        | ()                                                                        | WB_Point[]           |      |
|        | getSegments       | ()                                                                        | List&lt;int[]&gt;    |      |
|        | getId             | ()                                                                        | int                  |      |
|        | setId             | final int id                                                              | void                 |      |
|        | isDegenerate      | ()                                                                        | boolean              |      |
|        | set               | final WB_AABB src                                                         | void                 |      |
|        | init              | ()                                                                        | void                 |      |
|        | get               | ()                                                                        | WB_AABB              |      |
|        | getUnion          | final WB_AABB aabb                                                        | WB_AABB              |      |
|        | getIntersection   | final WB_AABB other                                                       | WB_AABB              |      |
| static | intersects        | final WB_Coord p1, final WB_Coord p2,final WB_Coord q                     | boolean              |      |
| static | intersects        | final WB_Coord p1, final WB_Coord p2,final WB_Coord q1, final WB_Coord q2 | boolean              |      |
|        | getWidth          | ()                                                                        | double               |      |
|        | getHeight         | ()                                                                        | double               |      |
|        | getDepth          | ()                                                                        | double               |      |
|        | getMin            | final int i                                                               | double               |      |
|        | getMax            | final int i                                                               | double               |      |
|        | getCenter         | final int i                                                               | double               |      |
|        | getMinX           | ()                                                                        | double               |      |
|        | getMaxX           | ()                                                                        | double               |      |
|        | getCenterX        | ()                                                                        | double               |      |
|        | getMinY           | ()                                                                        | double               |      |
|        | getMaxY           | ()                                                                        | double               |      |
|        | getCenterY        | ()                                                                        | double               |      |
|        | getMinZ           | ()                                                                        | double               |      |
|        | getMaxZ           | ()                                                                        | double               |      |
|        | getCenterZ        | ()                                                                        | double               |      |
|        | getVolume         | ()                                                                        | double               |      |
|        | getArea           | ()                                                                        | double               |      |
|        | minExtent         | ()                                                                        | double               |      |
|        | maxExtent         | ()                                                                        | double               |      |
|        | translate         | final double x, final double y, final double z                            | void                 |      |
|        | getTriangles      | ()                                                                        | List&lt;int[]&gt;    |      |
|        | getFaces          | ()                                                                        | int[][]              |      |
|        | getMin            | ()                                                                        | WB_Point             |      |
|        | getMax            | ()                                                                        | WB_Point             |      |
|        | getCenter         | ()                                                                        | WB_Point             |      |
|        | getDim            | ()                                                                        | int                  |      |
|        | getTrueDim        | ()                                                                        | int                  |      |
|        | pad               | final double factor                                                       | void                 |      |
|        | hashCode          | ()                                                                        | int                  |      |
|        | hashCode          | final double v                                                            | int                  |      |
|        | setToNull         | ()                                                                        | void                 |      |
|        | isNull            | ()                                                                        | boolean              |      |
|        | isValid           | ()                                                                        | boolean              |      |