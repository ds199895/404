---
navs: []
tags: [He_core]
image:
title: HE_Face
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
  var referrer ='HE_Face';
  localStorage.setItem('referrer', referrer);
}
</script>

<br>

### HE_Face

<br>
#### extends:   [HE_MeshElement](/hemesh/he-meshelement)
<br>
#### implements:  Comparable&lt;HE_Face&gt;  [WB_TriangleFactory](/hemesh/wb-trianglefactory)
<br>


- **构造方法**

| 属性   | 方法名     | 参数   | 返回值     | 备注   |
|:-----|:--------|:-----|:--------|:-----|
|      | HE_Face | ()   | HE_Face |      |

- **成员方法**

| 属性   | 方法名                        | 参数                         | 返回值                               | 备注   |
|:-----|:---------------------------|:---------------------------|:----------------------------------|:-----|
|      | getHalfedge                | ()                         | HE_Halfedge                       |      |
|      | setHalfedge                | final HE_Halfedge halfedge | void                              |      |
|      | clearHalfedge              | ()                         | void                              |      |
|      | getHalfedge                | final HE_Vertex v          | HE_Halfedge                       |      |
|      | getHalfedge                | final HE_Face f            | HE_Halfedge                       |      |
|      | getFaceCenter              | ()                         | WB_Point                          |      |
|      | getFaceNormal              | ()                         | WB_Vector                         |      |
|      | getFaceArea                | ()                         | double                            |      |
|      | getFaceDegree              | ()                         | int                               |      |
|      | feCrc                      | ()                         | HE_FaceEdgeCirculator             |      |
|      | ffCrc                      | ()                         | HE_FaceFaceCirculator             |      |
|      | fvCrc                      | ()                         | HE_FaceVertexCirculator           |      |
|      | fheiCrc                    | ()                         | HE_FaceHalfedgeInnerCirculator    |      |
|      | fheoCrc                    | ()                         | HE_FaceHalfedgeOuterCirculator    |      |
|      | feRevCrc                   | ()                         | HE_FaceEdgeRevCirculator          |      |
|      | ffRevCrc                   | ()                         | HE_FaceFaceRevCirculator          |      |
|      | fheiRevCrc                 | ()                         | HE_FaceHalfedgeInnerRevCirculator |      |
|      | fheoRevCrc                 | ()                         | HE_FaceHalfedgeOuterRevCirculator |      |
|      | fvRevCrc                   | ()                         | HE_FaceVertexRevCirculator        |      |
|      | getFaceVertices            | ()                         | List&lt;HE_Vertex&gt;             |      |
|      | getUniqueFaceVertices      | ()                         | List&lt;HE_Vertex&gt;             |      |
|      | getFaceHalfedges           | ()                         | List&lt;HE_Halfedge&gt;           |      |
|      | getFaceHalfedgesTwoSided   | ()                         | List&lt;HE_Halfedge&gt;           |      |
|      | getFaceEdges               | ()                         | List&lt;HE_Halfedge&gt;           |      |
|      | getNeighborFaces           | ()                         | List&lt;HE_Face&gt;               |      |
|      | getFaceUVWs                | ()                         | List&lt;HE_TextureCoordinate&gt;  |      |
|      | move                       | final WB_Coord c           | void                              |      |
|      | compareTo                  | final HE_Face f            | int                               |      |
|      | getTriangles               | ()                         | int[]                             |      |
|      | getTriangles               | final boolean optimize     | int[]                             |      |
|      | getAABB                    | ()                         | WB_AABB                           |      |
|      | toString                   | ()                         | String                            |      |
|      | isPlanar                   | ()                         | boolean                           |      |
|      | isBoundary                 | ()                         | boolean                           |      |
|      | isDegenerate               | ()                         | boolean                           |      |
|      | copyProperties             | final HE_Face el           | void                              |      |
|      | clear                      | ()                         | void                              |      |
|      | getTextureId               | ()                         | int                               |      |
|      | setTextureId               | final int i                | void                              |      |
|      | isNeighbor                 | final HE_Face f            | boolean                           |      |
|      | getPoints                  | ()                         | WB_CoordCollection                |      |
|      | clearPrecomputed           | ()                         | void                              |      |
|      | getFaceCS                  | ()                         | WB_CoordinateSystem               |      |
|      | getFaceNormalNotNormalized | ()                         | WB_Vector                         |      |
|      | getFaceType                | ()                         | WB_Classification                 |      |
|      | getNormalOffsetFaceCenter  | ()                         | WB_Vector                         |      |
|      | getNormalOffsetPlane       | final double d             | WB_Plane                          |      |
|      | getOrthoPolygon            | ()                         | WB_Polygon                        |      |
|      | getPlanarPolygon           | ()                         | WB_Polygon                        |      |
|      | getPlane                   | ()                         | WB_Plane                          |      |
|      | getPolygon                 | ()                         | WB_Polygon                        |      |
|      | getTriangle                | ()                         | WB_Triangle                       |      |