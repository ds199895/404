---
navs: []
tags: [He_core]
image:
title: HE_MeshOp
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
            


### HE_MeshOp

<br>


- **构造方法**

| 属性   | 方法名       | 参数   | 返回值       | 备注   |
|:-----|:----------|:-----|:----------|:-----|
|      | HE_MeshOp | ()   | HE_MeshOp |      |

- **成员方法**

| 属性     | 方法名                                       | 参数                                                                                          | 返回值                                 | 备注   |
|:-------|:------------------------------------------|:--------------------------------------------------------------------------------------------|:------------------------------------|:-----|
| static | splitEdge                                 | final HE_Mesh mesh, final HE_Halfedge edge                                                  | HE_Selection                        |      |
| static | splitEdge                                 | final HE_Mesh mesh, final HE_Halfedge edge, final double f                                  | HE_Selection                        |      |
| static | splitEdge                                 | final HE_Mesh mesh, final HE_Halfedge edge, final double x, final double y,final double z   | void                                |      |
| static | splitEdge                                 | final HE_Mesh mesh, final HE_Halfedge edge, final double[] f                                | void                                |      |
| static | splitEdge                                 | final HE_Mesh mesh, final HE_Halfedge edge, final float[] f                                 | void                                |      |
| static | splitEdge                                 | final HE_Mesh mesh, final HE_Halfedge edge, final WB_Coord v                                | HE_Selection                        |      |
| static | splitEdge                                 | final HE_Mesh mesh, final HE_Halfedge edge, final HE_Vertex v                               | HE_Selection                        |      |
| static | splitEdge                                 | final HE_Mesh mesh, final long key                                                          | HE_Selection                        |      |
| static | splitEdge                                 | final HE_Mesh mesh, final long key, final double f                                          | HE_Selection                        |      |
| static | splitEdge                                 | final HE_Mesh mesh, final long key, final double x, final double y, final double z          | void                                |      |
| static | splitEdge                                 | final HE_Mesh mesh, final long key, final double[] f                                        | void                                |      |
| static | splitEdge                                 | final HE_Mesh mesh, final long key, final float[] f                                         | void                                |      |
| static | splitEdge                                 | final HE_Mesh mesh, final Long key, final WB_Point v                                        | HE_Selection                        |      |
| static | splitEdges                                | final HE_Mesh mesh                                                                          | HE_Selection                        |      |
| static | splitEdges                                | final HE_Mesh mesh, final double offset                                                     | HE_Selection                        |      |
| static | splitEdges                                | final HE_Selection selection                                                                | HE_Selection                        |      |
| static | splitEdges                                | final HE_Selection selection, final double offset                                           | HE_Selection                        |      |
| static | divideEdge                                | final HE_Mesh mesh, final HE_Halfedge origE, final int n                                    | void                                |      |
| static | divideEdge                                | final HE_Mesh mesh, final long key, final int n                                             | void                                |      |
| static | splitFace                                 | final HE_Mesh mesh, final HE_Face face, final HE_Vertex vi,final HE_Vertex vj               | HE_Selection                        |      |
| static | splitFace                                 | final HE_Mesh mesh, final long fkey, final long vkeyi, final long vkeyj                     | HE_Selection                        |      |
| static | splitFacesCenter                          | final HE_Mesh mesh                                                                          | HE_Selection                        |      |
| static | splitFacesCenter                          | final HE_Mesh mesh, final double d                                                          | HE_Selection                        |      |
| static | splitFacesCenter                          | final HE_Mesh mesh, final double d, final double c                                          | HE_Selection                        |      |
| static | splitFacesCenter                          | final HE_Selection faces                                                                    | HE_Selection                        |      |
| static | splitFacesCenter                          | final HE_Selection faces, final double d                                                    | HE_Selection                        |      |
| static | splitFacesCenter                          | final HE_Selection faces, final double d, final double c                                    | HE_Selection                        |      |
| static | splitFacesCenterHole                      | final HE_Mesh mesh                                                                          | HE_Selection                        |      |
| static | splitFacesCenterHole                      | final HE_Mesh mesh, final double d                                                          | HE_Selection                        |      |
| static | splitFacesCenterHole                      | final HE_Mesh mesh, final double d, final double c                                          | HE_Selection                        |      |
| static | splitFacesCenterHole                      | final HE_Selection faces                                                                    | HE_Selection                        |      |
| static | splitFacesCenterHole                      | final HE_Selection faces, final double d                                                    | HE_Selection                        |      |
| static | splitFacesCenterHole                      | final HE_Selection faces, final double d, final double c                                    | HE_Selection                        |      |
| static | splitFacesHybrid                          | final HE_Mesh mesh                                                                          | HE_Selection                        |      |
| static | splitFacesHybrid                          | final HE_Selection sel                                                                      | HE_Selection                        |      |
| static | splitFacesMidEdge                         | final HE_Mesh mesh                                                                          | HE_Selection                        |      |
| static | splitFacesMidEdge                         | final HE_Selection selection                                                                | HE_Selection                        |      |
| static | splitFacesMidEdgeHole                     | final HE_Mesh mesh                                                                          | HE_Selection                        |      |
| static | splitFacesMidEdgeHole                     | final HE_Selection selection                                                                | HE_Selection                        |      |
| static | splitFacesQuad                            | final HE_Mesh mesh                                                                          | HE_Selection                        |      |
| static | splitFacesQuad                            | final HE_Mesh mesh, final double d                                                          | HE_Selection                        |      |
| static | splitFacesQuad                            | final HE_Selection sel                                                                      | HE_Selection                        |      |
| static | splitFacesQuad                            | final HE_Selection sel, final double d                                                      | HE_Selection                        |      |
| static | splitFacesTri                             | final HE_Mesh mesh                                                                          | HE_Selection                        |      |
| static | splitFacesTri                             | final HE_Mesh mesh, final double d                                                          | HE_Selection                        |      |
| static | splitFacesTri                             | final HE_Selection selection                                                                | HE_Selection                        |      |
| static | splitFacesTri                             | final HE_Selection selection, final double d                                                | HE_Selection                        |      |
| static | triangulate                               | final HE_Mesh mesh                                                                          | HE_Selection                        |      |
| static | triangulate                               | final HE_Mesh mesh, final HE_Face face                                                      | HE_Selection                        |      |
| static | triangulate                               | final HE_Selection sel                                                                      | HE_Selection                        |      |
| static | triangulate                               | final HE_Mesh mesh, final long key                                                          | HE_Selection                        |      |
| static | triangulateConcaveFace                    | final HE_Mesh mesh, final HE_Face face                                                      | HE_Selection                        |      |
| static | triangulateConcaveFace                    | final HE_Mesh mesh, final long key                                                          | HE_Selection                        |      |
| static | triangulateConcaveFaces                   | final HE_Mesh mesh                                                                          | HE_Selection                        |      |
| static | triangulateConcaveFaces                   | final HE_Mesh mesh, final List<HE_Face> sel                                                 | HE_Selection                        |      |
| static | triangulateFaceStar                       | final HE_Mesh mesh, final HE_Vertex v                                                       | HE_Selection                        |      |
| static | triangulateFaceStar                       | final HE_Mesh mesh, final long vertexkey                                                    | HE_Selection                        |      |
| static | createFaceFromHalfedgeLoop                | final HE_Mesh mesh, final HE_Halfedge he                                                    | HE_Face                             |      |
| static | createFaceFromHalfedgeLoop                | final HE_Mesh mesh, final List<HE_Halfedge> hes                                             | List&lt;HE_Face&gt;                 |      |
| static | selectAllFacesConnectedToUnpairedHalfedge | final HE_Mesh mesh,final HE_Halfedge unpairedHalfedge                                       | HE_RAS&lt;HE_Face&gt;               |      |
| static | flipFaces                                 | final HE_Mesh mesh                                                                          | HE_Mesh                             |      |
| static | flipFaces                                 | final HE_Selection sel                                                                      | HE_Mesh                             |      |
| static | flipEdge                                  | final HE_Mesh mesh, final HE_Halfedge he                                                    | boolean                             |      |
| static | flipEdgeConditional                       | final HE_Mesh mesh, final HE_Halfedge he                                                    | boolean                             |      |
| static | flipPlanarEdgeConditional                 | final HE_Mesh mesh, final HE_Halfedge he, final double cosa                                 | boolean                             |      |
| static | flipPlanarEdgeConditional                 | final HE_Mesh mesh, final HE_Halfedge he                                                    | boolean                             |      |
| static | improveTriangulation                      | final HE_Mesh mesh, final HE_Selection triangles                                            | void                                |      |
| static | improveTriangulation                      | final HE_Mesh mesh                                                                          | void                                |      |
| static | improveTriangulation                      | final HE_Mesh mesh, final double cosa                                                       | void                                |      |
| static | improveTriangulation                      | final HE_Mesh mesh, final HE_Selection triangles, final double cosa                         | void                                |      |
| static | cleanUnusedElementsByFace                 | final HE_Mesh mesh                                                                          | HE_Mesh                             |      |
| static | removeUnconnectedElements                 | final HE_Mesh mesh                                                                          | HE_Mesh                             |      |
| static | assignFaceToLoop                          | final HE_Mesh mesh, final HE_Face face, final HE_Halfedge halfedge                          | void                                |      |
| static | getIntersection                           | final HE_Face face, final WB_Line line                                                      | HE_FaceLineIntersection             |      |
| static | getIntersection                           | final HE_Face face, final WB_Ray ray                                                        | HE_FaceLineIntersection             |      |
| static | getIntersection                           | final HE_Face face, final WB_Segment segment                                                | HE_FaceLineIntersection             |      |
| static | getIntersection                           | final HE_Halfedge e, final WB_Plane P                                                       | double                              |      |
| static | getIntersection                           | final WB_AABBTree3D tree, final WB_Ray ray                                                  | List&lt;HE_FaceLineIntersection&gt; |      |
| static | getIntersectionNoOrigin                   | final WB_AABBTree3D tree, final WB_Ray ray                                                  | List&lt;HE_FaceLineIntersection&gt; |      |
| static | isInside                                  | final HE_Mesh mesh, final WB_Coord p                                                        | boolean                             |      |
| static | isInside                                  | final WB_AABBTree3D tree, final WB_Coord p                                                  | boolean                             |      |
| static | getIntersection                           | final WB_AABBTree3D tree, final WB_Segment segment                                          | List&lt;HE_FaceLineIntersection&gt; |      |
| static | getIntersection                           | final WB_AABBTree3D tree, final WB_Line line                                                | List&lt;HE_FaceLineIntersection&gt; |      |
| static | getIntersection                           | final WB_AABBTree3D tree, final WB_Plane P                                                  | List&lt;WB_Segment&gt;              |      |
| static | getPotentialIntersectedFaces              | final WB_AABBTree3D tree, final WB_Plane P                                                  | List&lt;HE_Face&gt;                 |      |
| static | getPotentialIntersectedFaces              | final WB_AABBTree3D tree, final WB_Triangle T                                               | List&lt;HE_Face&gt;                 |      |
| static | getPotentialIntersectedFaces              | final WB_AABBTree3D tree, final WB_AABB AABB                                                | List&lt;HE_Face&gt;                 |      |
| static | getPotentialIntersectedFaces              | final WB_AABBTree3D tree, final WB_Coord p                                                  | List&lt;HE_Face&gt;                 |      |
| static | getPotentialIntersectedFaces              | final WB_AABBTree3D tree, final WB_Ray R                                                    | List&lt;HE_Face&gt;                 |      |
| static | getPotentialIntersectedFaces              | final WB_AABBTree3D tree, final WB_Line L                                                   | List&lt;HE_Face&gt;                 |      |
| static | getPotentialIntersectedFaces              | final WB_AABBTree3D tree, final WB_Segment segment                                          | List&lt;HE_Face&gt;                 |      |
| static | getClosestIntersection                    | final WB_AABBTree3D tree, final WB_Ray ray                                                  | HE_FaceLineIntersection             |      |
| static | getFurthestIntersection                   | final WB_AABBTree3D tree, final WB_Ray ray                                                  | HE_FaceLineIntersection             |      |
| static | getClosestIntersection                    | final WB_AABBTree3D tree, final WB_Line line                                                | HE_FaceLineIntersection             |      |
| static | getFurthestIntersection                   | final WB_AABBTree3D tree, final WB_Line line                                                | HE_FaceLineIntersection             |      |
| static | getClosestIntersection                    | final WB_AABBTree3D tree, final WB_Segment segment                                          | HE_FaceLineIntersection             |      |
| static | getFurthestIntersection                   | final WB_AABBTree3D tree, final WB_Segment segment                                          | HE_FaceLineIntersection             |      |
| static | getIntersection                           | final HE_Mesh mesh, final WB_Ray ray                                                        | List&lt;HE_FaceLineIntersection&gt; |      |
| static | getIntersection                           | final HE_Mesh mesh, final WB_Segment segment                                                | List&lt;HE_FaceLineIntersection&gt; |      |
| static | getIntersection                           | final HE_Mesh mesh, final WB_Line line                                                      | List&lt;HE_FaceLineIntersection&gt; |      |
| static | getIntersection                           | final HE_Mesh mesh, final WB_Plane P                                                        | List&lt;WB_Segment&gt;              |      |
| static | getPotentialIntersectedFaces              | final HE_Mesh mesh, final WB_Plane P                                                        | List&lt;HE_Face&gt;                 |      |
| static | getPotentialIntersectedFaces              | final HE_Mesh mesh, final WB_Ray R                                                          | List&lt;HE_Face&gt;                 |      |
| static | getPotentialIntersectedFaces              | final HE_Mesh mesh, final WB_Line L                                                         | List&lt;HE_Face&gt;                 |      |
| static | getPotentialIntersectedFaces              | final HE_Mesh mesh, final WB_Segment segment                                                | List&lt;HE_Face&gt;                 |      |
| static | getClosestIntersection                    | final HE_Mesh mesh, final WB_Ray ray                                                        | HE_FaceLineIntersection             |      |
| static | getFurthestIntersection                   | final HE_Mesh mesh, final WB_Ray ray                                                        | HE_FaceLineIntersection             |      |
| static | getClosestIntersection                    | final HE_Mesh mesh, final WB_Line line                                                      | HE_FaceLineIntersection             |      |
| static | getFurthestIntersection                   | final HE_Mesh mesh, final WB_Line line                                                      | HE_FaceLineIntersection             |      |
| static | getClosestIntersection                    | final HE_Mesh mesh, final WB_Segment segment                                                | HE_FaceLineIntersection             |      |
| static | getFurthestIntersection                   | final HE_Mesh mesh, final WB_Segment segment                                                | HE_FaceLineIntersection             |      |
| static | classifyFaceToPlane3D                     | final HE_Face f, final WB_Plane P                                                           | WB_Classification                   |      |
| static | classifyEdgeToPlane3D                     | final HE_Halfedge edge, final WB_Plane P                                                    | WB_Classification                   |      |
| static | classifyVertexToPlane3D                   | final HE_Vertex v, final WB_Plane P                                                         | WB_Classification                   |      |
| static | getNormalOffsetPosition                   | HE_Vertex v, final double d                                                                 | WB_Point                            |      |
| static | getVertexType                             | final HE_Vertex vertex                                                                      | WB_Classification                   |      |
| static | getVertexCS                               | final HE_Vertex v                                                                           | WB_CoordinateSystem                 |      |
| static | getVertexNormal                           | final HE_Vertex v                                                                           | WB_Vector                           |      |
| static | getVertexNormalAverage                    | final HE_Vertex v                                                                           | WB_Vector                           |      |
| static | getVertexNormalArea                       | final HE_Vertex v                                                                           | WB_Vector                           |      |
| static | getVertexNormalAngle                      | final HE_Vertex v                                                                           | WB_Vector                           |      |
| static | getVertexNormalGaussianCurvature          | final HE_Vertex v                                                                           | WB_Vector                           |      |
| static | getVertexNormalMeanCurvature              | final HE_Vertex v                                                                           | WB_Vector                           |      |
| static | getVertexNormalSphereInscribed            | final HE_Vertex v                                                                           | WB_Vector                           |      |
| static | getUmbrellaAngle                          | final HE_Vertex v                                                                           | double                              |      |
| static | getAngleDefect                            | final HE_Vertex v                                                                           | double                              |      |
| static | getAngleDefect                            | final HE_Mesh mesh                                                                          | double                              |      |
| static | getScalarGaussianCurvature                | final HE_Vertex v                                                                           | double                              |      |
| static | getScalarMeanCurvature                    | final HE_Vertex v                                                                           | double                              |      |
| static | getVertexArea                             | final HE_Vertex v                                                                           | double                              |      |
| static | getBarycentricDualVertexArea              | final HE_Vertex v                                                                           | double                              |      |
| static | getCircumcentricDualVertexArea            | final HE_Vertex v                                                                           | double                              |      |
| static | getPrincipalCurvatures                    | final HE_Vertex v                                                                           | double[]                            |      |
| static | getGaussianCurvature                      | final HE_Vertex vertex, final WB_Vector meanCurvatureVector                                 | double                              |      |
| static | getGaussianCurvature                      | final HE_Vertex vertex                                                                      | double                              |      |
| static | getCurvatureDirections                    | final HE_Vertex v                                                                           | WB_CoordinateSystem                 |      |
| static | findOptimalSolution                       | final HE_Vertex v, final WB_Vector normal, final WB_Vector t1,final WB_Vector t2            | WB_Vector                           |      |
| static | getFaceCenter                             | HE_Face f                                                                                   | WB_Point                            |      |
| static | getNormalOffsetFaceCenter                 | HE_Face f, final double d                                                                   | WB_Point                            |      |
| static | getTriangle                               | HE_Face f                                                                                   | WB_Triangle                         |      |
| static | getPolygon                                | HE_Face f                                                                                   | WB_Polygon                          |      |
| static | getOrthoPolygon                           | HE_Face f                                                                                   | WB_Polygon                          |      |
| static | getPlanarPolygon                          | HE_Face f                                                                                   | WB_Polygon                          |      |
| static | getFaceNormal                             | final HE_Face face                                                                          | WB_Vector                           |      |
| static | getFaceNormalNotNormalized                | final HE_Face face                                                                          | WB_Vector                           |      |
| static | getPlane                                  | HE_Face f                                                                                   | WB_Plane                            |      |
| static | getNormalOffsetPlane                      | HE_Face f, final double d                                                                   | WB_Plane                            |      |
| static | getFaceArea                               | final HE_Face face                                                                          | double                              |      |
| static | getFaceType                               | final HE_Face face                                                                          | WB_Classification                   |      |
| static | getFaceCS                                 | HE_Face f                                                                                   | WB_CoordinateSystem                 |      |
| static | collapseHalfedge                          | final HE_Mesh mesh, final HE_Halfedge he                                                    | boolean                             |      |
| static | collapseHalfedgeBoundaryPreserving        | final HE_Mesh mesh, final HE_Halfedge he                                                    | boolean                             |      |
| static | collapseEdge                              | final HE_Mesh mesh, final HE_Halfedge e                                                     | boolean                             |      |
| static | collapseEdgeBoundaryPreserving            | final HE_Mesh mesh, final HE_Halfedge e,final boolean strict                                | boolean                             |      |
| static | pointIsInFace                             | final WB_Coord p, final HE_Face f                                                           | boolean                             |      |
| static | pointIsStrictlyInFace                     | final WB_Coord p, final HE_Face f                                                           | boolean                             |      |
| static | expandVertexToEdge                        | final HE_Mesh mesh, final HE_Vertex v, final HE_Face f1, final HE_Face f2,final WB_Coord vn | void                                |      |
| static | getVolume                                 | final HE_Mesh mesh                                                                          | double                              |      |
| static | signedVolume                              | final HE_Face f, final WB_Coord center                                                      | double                              |      |
| static | getClosestPointToTriangleFace             | final WB_Coord p, final HE_Face T                                                           | WB_Coord[]                          |      |
| static | getClosestPointToTriangleMesh             | final WB_Coord p, final HE_Mesh mesh                                                        | WB_Coord[]                          |      |
| static | liftEdges                                 | final HE_Selection edges, final double d                                                    | void                                |      |
| static | getCotan                                  | final HE_Halfedge he                                                                        | double                              |      |
| static | getMassArray                              | final HE_Mesh mesh                                                                          | double[]                            |      |
| static | getIntersection                           | final HE_Mesh mesh1, final HE_Mesh mesh2                                                    | List&lt;HE_FaceFaceIntersection&gt; |      |
|        | processIntersectedFaces                   | List<HE_FaceFaceIntersection> intersections                                                 | Map&lt;Long,HE_IntersectedFace&gt;  |      |
| static | fuseCoplanarFaces                         | final HE_Mesh mesh                                                                          | void                                |      |
| static | fuseCoplanarFaces                         | final HE_Mesh mesh, final double a                                                          | void                                |      |
| static | fuseCoplanarFaces                         | final HE_Selection sel                                                                      | void                                |      |
| static | fuseCoplanarFaces                         | final HE_Selection sel, final double a                                                      | void                                |      |
| static | deleteEdge                                | final HE_Mesh mesh, final HE_Halfedge e                                                     | HE_Face                             |      |
| static | getClosestPoint                           | HE_Face f, final WB_Coord p                                                                 | WB_Point                            |      |
| static | getHalfedgeType                           | HE_Halfedge he                                                                              | WB_Classification                   |      |
| static | getHalfedgeVector                         | HE_Halfedge he                                                                              | WB_Vector                           |      |
| static | getHalfedgeTangent                        | HE_Halfedge he                                                                              | WB_Vector                           |      |
| static | getEdgeTangent                            | HE_Halfedge he                                                                              | WB_Vector                           |      |
| static | getHalfedgeCenter                         | HE_Halfedge he                                                                              | WB_Point                            |      |
| static | getHalfedgeCenter                         | HE_Halfedge he, final double f                                                              | WB_Point                            |      |
| static | getEdgeCenter                             | HE_Halfedge he                                                                              | WB_Point                            |      |
| static | getEdgeCenter                             | HE_Halfedge he, final double f                                                              | WB_Point                            |      |
| static | getEdgeNormal                             | HE_Halfedge he                                                                              | WB_Vector                           |      |
| static | getHalfedgeNormal                         | HE_Halfedge he                                                                              | WB_Vector                           |      |
| static | getHalfedgeArea                           | HE_Halfedge he                                                                              | double                              |      |
| static | getHalfedgeDihedralAngle                  | HE_Halfedge he                                                                              | double                              |      |
| static | getEdgeArea                               | HE_Halfedge he                                                                              | double                              |      |
| static | getEdgeDihedralAngle                      | HE_Halfedge he                                                                              | double                              |      |
| static | getEdgeCosDihedralAngle                   | HE_Halfedge he                                                                              | double                              |      |
| static | getLength                                 | HE_Halfedge he                                                                              | double                              |      |
| static | getSqLength                               | HE_Halfedge he                                                                              | double                              |      |
| static | getAngle                                  | HE_Halfedge he                                                                              | double                              |      |
| static | getAABB                                   | HE_Face f                                                                                   | WB_AABB                             |      |
| static | getAABB                                   | HE_Halfedge he                                                                              | WB_AABB                             |      |
| static | getAABB                                   | HE_Mesh mesh                                                                                | WB_AABB                             |      |
| static | getBoundingSphere                         | HE_Mesh mesh                                                                                | WB_Sphere                           |      |
| static | WB_AABB                                   | HE_Selection sel                                                                            | final                               |      |
| static | WB_Sphere                                 | HE_Selection sel                                                                            | final                               |      |
| static | getLimits                                 | HE_HalfedgeStructure hes                                                                    | double[]                            |      |
| static | addPointInClosestFace                     | HE_Mesh mesh, final WB_Coord p,final WB_KDTree3D<WB_Coord, Long> vertexTree                 | void                                |      |
| static | createPathFromIndices                     | HE_Mesh mesh, final int[] vertices, final boolean loop                                      | HE_Path                             |      |
| static | getArea                                   | HE_Mesh mesh                                                                                | double                              |      |
| static | getClosestPoint                           | HE_Mesh mesh, final WB_Coord p, final WB_KDTree3D<WB_Coord, Long> vertexTree                | WB_Point                            |      |
| static | getClosestVertex                          | HE_Mesh mesh, final WB_Coord p,final WB_KDTree3D<WB_Coord, Long> vertexTree                 | HE_Vertex                           |      |
| static | getCenter                                 | HE_Mesh mesh                                                                                | WB_Point                            |      |
| static | cycleHalfedges                            | HE_Mesh mesh, final List<HE_Halfedge> halfedges                                             | void                                |      |
| static | cycleHalfedgesReverse                     | HE_Mesh mesh, final List<HE_Halfedge> halfedges                                             | void                                |      |
| static | orderHalfedges                            | HE_Mesh mesh, final List<HE_Halfedge> halfedges, final boolean loop                         | void                                |      |
| static | orderHalfedgesReverse                     | HE_Mesh mesh, final List<HE_Halfedge> halfedges, final boolean loop                         | void                                |      |
| static | capHalfedges                              | HE_Mesh mesh                                                                                | void                                |      |
| static | pairHalfedges                             | HE_Mesh mesh                                                                                | void                                |      |
| static | pairHalfedges                             | HE_Mesh mesh, final List<HE_Halfedge> unpairedHalfedges                                     | void                                |      |
| static | pairHalfedgesOnePass                      | HE_Mesh mesh                                                                                | List&lt;HE_Halfedge&gt;             |      |

### HE_FaceLineIntersection

<br>


- **构造方法**

| 属性   | 方法名                     | 参数                                | 返回值                     | 备注   |
|:-----|:------------------------|:----------------------------------|:------------------------|:-----|
|      | HE_FaceLineIntersection | final HE_Face f, final WB_Point p | HE_FaceLineIntersection |      |

- **成员方法**

| 属性   | 方法名      | 参数   | 返回值      | 备注   |
|:-----|:---------|:-----|:---------|:-----|
|      | getFace  | ()   | HE_Face  |      |
|      | getPoint | ()   | WB_Point |      |

### HE_FaceFaceIntersection

<br>


- **构造方法**

| 属性   | 方法名                     | 参数                                                       | 返回值                     | 备注   |
|:-----|:------------------------|:---------------------------------------------------------|:------------------------|:-----|
|      | HE_FaceFaceIntersection | final HE_Face f1, final HE_Face f2, final WB_Segment seg | HE_FaceFaceIntersection |      |

- **成员方法**

| 属性   | 方法名        | 参数    | 返回值        | 备注   |
|:-----|:-----------|:------|:-----------|:-----|
|      | getFace1   | ()    | HE_Face    |      |
|      | getFace2   | ()    | HE_Face    |      |
|      | getSegment | ()    | WB_Segment |      |
|      |            | coord | switch     |      |

### FaceSegmentBin

<br>


- **构造方法**

| 属性   | 方法名            | 参数           | 返回值            | 备注   |
|:-----|:---------------|:-------------|:---------------|:-----|
|      | FaceSegmentBin | HE_Face face | FaceSegmentBin |      |

- **成员方法**

| 属性   | 方法名        | 参数                 | 返回值   | 备注   |
|:-----|:-----------|:-------------------|:------|:-----|
|      | addSegment | WB_Segment segment | void  |      |

### HE_IntersectedFace

<br>


- **构造方法**

| 属性   | 方法名                | 参数                                                     | 返回值                | 备注   |
|:-----|:-------------------|:-------------------------------------------------------|:-------------------|:-----|
|      | HE_IntersectedFace | HE_Face face, List<WB_Coord> points, int[] constraints | HE_IntersectedFace |      |

### VertexInfo

<br>


- **构造方法**

| 属性   | 方法名        | 参数   | 返回值        | 备注   |
|:-----|:-----------|:-----|:-----------|:-----|
|      | VertexInfo | ()   | VertexInfo |      |
|      | VertexInfo | ()   | VertexInfo |      |

- **成员方法**

| 属性   | 方法名   | 参数    | 返回值    | 备注   |
|:-----|:------|:------|:-------|:-----|
|      |       | coord | switch |      |

### VertexInfo

<br>


- **构造方法**

| 属性   | 方法名        | 参数   | 返回值        | 备注   |
|:-----|:-----------|:-----|:-----------|:-----|
|      | VertexInfo | ()   | VertexInfo |      |
|      | VertexInfo | ()   | VertexInfo |      |

- **成员方法**

| 属性   | 方法名   | 参数    | 返回值    | 备注   |
|:-----|:------|:------|:-------|:-----|
|      |       | coord | switch |      |