---
navs: []
tags: [He_core]
image:
title: HE_Halfedge
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
  var referrer ='HE_Halfedge';
  localStorage.setItem('referrer', referrer);
}
</script>

<br>

### HE_Halfedge

<br>
#### extends:   [HE_MeshElement](/hemesh/he-meshelement)
<br>
#### implements:  Comparable&lt;HE_Halfedge&gt;
<br>


- **构造方法**

| 属性   | 方法名         | 参数   | 返回值         | 备注   |
|:-----|:------------|:-----|:------------|:-----|
|      | HE_Halfedge | ()   | HE_Halfedge |      |

- **成员方法**

| 属性   | 方法名                      | 参数                                             | 返回值                  | 备注   |
|:-----|:-------------------------|:-----------------------------------------------|:---------------------|:-----|
|      | getPrevInFace            | ()                                             | HE_Halfedge          |      |
|      | getPrevInFace            | final int n                                    | HE_Halfedge          |      |
|      | getNextInFace            | ()                                             | HE_Halfedge          |      |
|      | getNextInFace            | final int n                                    | HE_Halfedge          |      |
|      | getNextInVertex          | ()                                             | HE_Halfedge          |      |
|      | getNextInVertex          | final int n                                    | HE_Halfedge          |      |
|      | getPrevInVertex          | ()                                             | HE_Halfedge          |      |
|      | getPrevInVertex          | final int n                                    | HE_Halfedge          |      |
|      | getPair                  | ()                                             | HE_Halfedge          |      |
|      | setNext                  | final HE_Halfedge he                           | void                 |      |
|      | setPrev                  | final HE_Halfedge he                           | void                 |      |
|      | setPair                  | final HE_Halfedge he                           | void                 |      |
|      | getEdge                  | ()                                             | HE_Halfedge          |      |
|      | getFace                  | ()                                             | HE_Face              |      |
|      | setFace                  | final HE_Face face                             | void                 |      |
|      | getVertex                | ()                                             | HE_Vertex            |      |
|      | getPosition              | ()                                             | WB_Point             |      |
|      | getStartVertex           | ()                                             | HE_Vertex            |      |
|      | getStartPosition         | ()                                             | WB_Point             |      |
|      | setVertex                | final HE_Vertex vertex                         | void                 |      |
|      | getEndVertex             | ()                                             | HE_Vertex            |      |
|      | getEndPosition           | ()                                             | WB_Point             |      |
|      | getCenter                | ()                                             | WB_Point             |      |
|      | getEdgeNormal            | ()                                             | WB_Vector            |      |
|      | getEdgeDirection         | ()                                             | WB_Vector            |      |
|      | getHalfedgeNormal        | ()                                             | WB_Vector            |      |
|      | getHalfedgeDirection     | ()                                             | WB_Vector            |      |
|      | getAABB                  | ()                                             | WB_AABB              |      |
|      | getEdgeArea              | ()                                             | double               |      |
|      | getHalfedgeArea          | ()                                             | double               |      |
|      | getSqLength              | ()                                             | double               |      |
|      | getLength                | ()                                             | double               |      |
|      | clearNext                | ()                                             | void                 |      |
|      | clearPrev                | ()                                             | void                 |      |
|      | clearPair                | ()                                             | void                 |      |
|      | clearFace                | ()                                             | void                 |      |
|      | clearVertex              | ()                                             | void                 |      |
|      | toString                 | ()                                             | String               |      |
|      | isEdge                   | ()                                             | boolean              |      |
|      | isInnerBoundary          | ()                                             | boolean              |      |
|      | isOuterBoundary          | ()                                             | boolean              |      |
|      | copyProperties           | final HE_Halfedge el                           | void                 |      |
|      | clear                    | ()                                             | void                 |      |
|      | getUVW                   | ()                                             | HE_TextureCoordinate |      |
|      | getHalfedgeUVW           | ()                                             | HE_TextureCoordinate |      |
|      | getVertexUVW             | ()                                             | HE_TextureCoordinate |      |
|      | clearUVW                 | ()                                             | void                 |      |
|      | setUVW                   | final double u, final double v, final double w | void                 |      |
|      | setUVW                   | final WB_Coord uvw                             | void                 |      |
|      | setUVW                   | final HE_TextureCoordinate uvw                 | void                 |      |
|      | hasHalfedgeUVW           | ()                                             | boolean              |      |
|      | hasUVW                   | ()                                             | boolean              |      |
|      | hasVertexUVW             | ()                                             | boolean              |      |
|      | compareTo                | final HE_Halfedge he                           | int                  |      |
|      | hashCode                 | ()                                             | int                  |      |
|      | clearPrecomputed         | ()                                             | void                 |      |
|      | getCotan                 | ()                                             | double               |      |
|      | getEdgeCenter            | final double f                                 | WB_Point             |      |
|      | getEdgeCosDihedralAngle  | ()                                             | double               |      |
|      | getEdgeDihedralAngle     | ()                                             | double               |      |
|      | getHalfedgeCenter        | final double f                                 | WB_Point             |      |
|      | getHalfedgeDihedralAngle | ()                                             | double               |      |