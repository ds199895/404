---
navs: []
tags: [Geom]
image:
title: WB_GeometryOp2D
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
            

<br>
<a href="/display/hemesh" onclick="saveReferrer()">继承关系图谱display</a>
<script>
function saveReferrer() {
  var referrer ='WB_GeometryOp2D';
  localStorage.setItem('referrer', referrer);
}
</script>

<br>

### WB_GeometryOp2D

<br>
#### extends:   [WB_GeometryOpGLU](/hemesh/wb-geometryopglu)
<br>


- **成员方法**

| 属性     | 方法名                   | 参数                                                                                                 | 返回值   | 备注   |
|:-------|:----------------------|:---------------------------------------------------------------------------------------------------|:------|:-----|
| static | WB_IntersectionResult | ()                                                                                                 | final |      |
| static | WB_IntersectionResult | ()                                                                                                 | final |      |
| static | void                  | final WB_Segment S1,final WB_Segment S2, final WB_IntersectionResult i                             | final |      |
| static | WB_Segment[]          | final WB_Segment S,final WB_Line L                                                                 | final |      |
| static | WB_Polygon[]          | final WB_Polygon poly,final WB_Line L                                                              | final |      |
| static | ArrayList<WB_Point>   | ()                                                                                                 | final |      |
| static | ArrayList<WB_Point>   | final WB_Line L,final WB_Circle C                                                                  | final |      |
| static | ArrayList<WB_Point>   | final WB_Ray R,final WB_Circle C                                                                   | final |      |
| static | boolean               | final WB_Coord a,final WB_Coord b, final WB_Coord c, final WB_Coord d                              | final |      |
| static | WB_Point              | final WB_Coord p,final WB_Segment S                                                                | final |      |
| static | WB_Point              | final WB_Coord p,final WB_PolyLine PL                                                              | final |      |
| static | WB_Point              | final WB_Segment S,final WB_Coord p                                                                | final |      |
| static | WB_Point              | final WB_Coord p,final WB_Coord a, final WB_Coord b                                                | final |      |
| static | WB_Point              | final WB_Coord p,final WB_Line L                                                                   | final |      |
| static | WB_Point              | final WB_Coord p,final WB_Coord a, final WB_Coord b                                                | final |      |
| static | WB_Point              | final WB_Coord p,final WB_Ray R                                                                    | final |      |
| static | WB_Point              | final WB_Coord p,final WB_Coord a, final WB_Coord b                                                | final |      |
| static | WB_IntersectionResult | ()                                                                                                 | final |      |
| static | WB_IntersectionResult | ()                                                                                                 | final |      |
| static | WB_IntersectionResult | final WB_Line L,final WB_Segment S                                                                 | final |      |
| static | WB_IntersectionResult | ()                                                                                                 | final |      |
| static | WB_Point              | final WB_Coord p,final WB_Triangle T                                                               | final |      |
| static | WB_Point              | final WB_Coord p,final WB_Coord a, final WB_Coord b, final WB_Coord c                              | final |      |
| static | WB_Point              | final WB_Coord p,final WB_Triangle T                                                               | final |      |
| static | WB_Point              | final WB_Coord p,final WB_Polygon poly                                                             | final |      |
| static | WB_Point              | final WB_Coord p,final ArrayList<? extends WB_Triangle> tris                                       | final |      |
| static | WB_Point              | final WB_Coord p,final WB_Polygon poly                                                             | final |      |
| static | WB_Point              | final WB_Coord p,final WB_Polygon poly, final ArrayList<WB_Triangle> tris                          | final |      |
| static | boolean               | final WB_Coord a, final WB_Coord b,final WB_Coord c                                                | final |      |
| static | boolean               | final WB_Coord a,final WB_Coord b, final WB_Coord c                                                | final |      |
| static | double                | final WB_Coord a,final WB_Coord b, final WB_Coord p                                                | final |      |
| static | double                | final WB_Coord p,final WB_Line L                                                                   | final |      |
| static | boolean               | final WB_Coord p,final WB_AABB2D AABB                                                              | final |      |
| static | double                | final WB_Coord p,final WB_Line L                                                                   | final |      |
| static | double                | final WB_Coord p,final WB_Coord q                                                                  | final |      |
| static | double                | final WB_Coord p,final WB_Segment S                                                                | final |      |
| static | double                | final WB_Coord p,final WB_Line L                                                                   | final |      |
| static | double                | final WB_Coord p, final WB_Ray R                                                                   | final |      |
| static | double                | final WB_Coord p,final WB_Coord a, final WB_Coord b                                                | final |      |
| static | double                | final WB_Coord p,final WB_Coord q                                                                  | final |      |
| static | double                | final WB_Coord p,final WB_Coord a, final WB_Coord b                                                | final |      |
| static | double                | final WB_Coord p,final WB_Coord a, final WB_Coord b                                                | final |      |
| static | double                | final WB_Coord p,final WB_Segment S                                                                | final |      |
| static | double                | final WB_Coord p,final WB_PolyLine PL                                                              | final |      |
| static | double                | final WB_Coord p,final WB_PolyLine PL                                                              | final |      |
| static | double                | final WB_Coord p,final WB_Line L                                                                   | final |      |
| static | double                | final WB_Coord p,final WB_Ray R                                                                    | final |      |
| static | double                | final WB_Coord p,final WB_Coord a, final WB_Coord b                                                | final |      |
| static | double                | final WB_Coord p,final WB_Line L                                                                   | final |      |
| static | double                | final WB_Coord p,final WB_Coord q                                                                  | final |      |
| static | double                | final WB_Coord p,final WB_Coord q                                                                  | final |      |
| static | double                | final WB_Coord p,final WB_Coord a, final WB_Coord b                                                | final |      |
| static | double                | final WB_Coord p,final WB_Coord a, final WB_Coord b                                                | final |      |
| static | int[]                 | ()                                                                                                 | final |      |
| static | int[]                 | ()                                                                                                 | final |      |
| static | WB_Classification     | ()                                                                                                 | final |      |
| static | WB_Classification     | ()                                                                                                 | final |      |
| static | WB_Classification     | ()                                                                                                 | final |      |
| static | WB_Classification     | ()                                                                                                 | final |      |
| static | boolean               | final WB_Coord p,final WB_Coord q, final WB_Line L                                                 | final |      |
| static | WB_Classification     | ()                                                                                                 | final |      |
| static | WB_Classification     | ()                                                                                                 | final |      |
| static | boolean               | final WB_Coord p,final WB_Polygon poly                                                             | final |      |
| static | boolean               | final WB_Coord p,final ArrayList<? extends WB_Triangle> tris                                       | final |      |
| static | boolean               | final WB_Coord p,final WB_Triangle tris                                                            | final |      |
| static | double[]              | final double u0,final double u1, final double v0, final double v1                                  | final |      |
| static | WB_Circle             | final WB_Coord[] points                                                                            | final |      |
| static | WB_Circle             | ()                                                                                                 | final |      |
| static | WB_Line               | ()                                                                                                 | final |      |
| static | ArrayList<WB_Line>    | ()                                                                                                 | final |      |
| static | ArrayList<WB_Line>    | ()                                                                                                 | final |      |
| static | WB_Point[]            | ()                                                                                                 | final |      |
| static | WB_Line               | ()                                                                                                 | final |      |
| static | WB_Line               | final WB_Line L,final WB_Coord p                                                                   | final |      |
| static | WB_Line               | final WB_Coord p,final WB_Coord q                                                                  | final |      |
| static | WB_Line[]             | final WB_Line L,final double d                                                                     | final |      |
| static | WB_Line[]             | ()                                                                                                 | final |      |
| static | WB_Sphere             | ()                                                                                                 | final |      |
| static | double                | final WB_Coord p1, final WB_Coord p2,final WB_Coord p3                                             | final |      |
| static | double                | final WB_Polygon poly                                                                              | final |      |
| static | boolean               | final WB_Coord p1, final WB_Coord p2,final WB_Coord A, final WB_Coord B                            | final |      |
| static | boolean               | final WB_Coord p,final WB_Coord A, final WB_Coord B, final WB_Coord C                              | final |      |
| static | boolean               | final WB_Coord p,final WB_Triangle T                                                               | final |      |
| static | boolean               | final WB_Coord p,final WB_Coord A, final WB_Coord B, final WB_Coord C                              | final |      |
| static | boolean               | final WB_Coord p,final WB_Triangle T                                                               | final |      |
| static | double                | final WB_Coord p1,final WB_Coord p2, final WB_Coord p3                                             | final |      |
| static | double                | final double x1,final double y1, final double x2, final double y2, final double x3,final double y3 | final |      |
| static | double                | ()                                                                                                 | final |      |
| static | double                | final WB_Coord[] coords,final int start, final int end                                             | final |      |
| static | double                | final WB_Coord p1,final WB_Coord p2, final WB_Coord p3                                             | final |      |
| static | WB_Coord              | final WB_Circle C,final WB_Coord v                                                                 | final |      |
| static | WB_Circle             | final WB_Circle C,final WB_Coord p                                                                 | final |      |
| static | WB_Polygon            | WB_Polygon poly,final double d                                                                     | final |      |
| static | WB_Polygon            | WB_Polygon poly,final double[] d                                                                   | final |      |
| static | boolean               | final WB_Coord a,final WB_Coord b, final WB_Coord p                                                | final |      |
| static | boolean               | final WB_Coord a, final WB_Coord b,final WB_Coord p                                                | final |      |
| static | boolean               | final WB_Coord a,final WB_Coord b, final WB_Coord p                                                | final |      |
| static | boolean               | final WB_Coord a, final WB_Coord b,final WB_Coord p                                                | final |      |
| static | boolean               | final WB_Coord p0, final WB_Coord p,final WB_Coord p1                                              | final |      |
| static | WB_Coord              | final WB_Coord ap1,final WB_Coord ap2, final WB_Coord bp1, final WB_Coord bp2                      | final |      |
| static | boolean               | final WB_Coord a1,final WB_Coord a2, final WB_Coord b1, final WB_Coord b2,final WB_MutableCoord p  | final |      |
| static | WB_Circle             | ()                                                                                                 | final |      |
| static | WB_Circle             | ()                                                                                                 | final |      |
| static | WB_Circle             | final WB_Circle C1,final WB_Circle C2                                                              | final |      |