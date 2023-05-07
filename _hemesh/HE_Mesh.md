---
navs: []
tags: [He_core]
image:
title: HE_Mesh
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
  var referrer ='HE_Mesh';
  localStorage.setItem('referrer', referrer);
}
</script>

<br>

### HE_Mesh

<br>
#### extends:   [HE_MeshElement](/hemesh/he-meshelement)
<br>
#### implements:   [WB_TriangleFactory](/hemesh/wb-trianglefactory)  [HE_HalfedgeStructure](/hemesh/he-halfedgestructure)  [WB_Geometry](/hemesh/wb-geometry)
<br>


- **构造方法**

| 属性   | 方法名     | 参数                              | 返回值     | 备注   |
|:-----|:--------|:--------------------------------|:--------|:-----|
|      | HE_Mesh | ()                              | HE_Mesh |      |
|      | HE_Mesh | final HE_Mesh mesh              | HE_Mesh |      |
|      | HE_Mesh | final HEC_Creator creator       | HE_Mesh |      |
|      | HE_Mesh | final WB_SimpleMesh mesh        | HE_Mesh |      |
|      | HE_Mesh | final WB_SimpleMeshCreator mesh | HE_Mesh |      |

- **成员方法**

| 属性   | 方法名                                    | 参数                                                                                                                           | 返回值                              | 备注   |
|:-----|:---------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------|:---------------------------------|:-----|
|      | add                                    | final HE_Element el                                                                                                          | void                             |      |
|      | add                                    | final HE_Face f                                                                                                              | void                             |      |
|      | addFaces                               | final Collection<? extends HE_Face> faces                                                                                    | void                             |      |
|      | addFaces                               | final HE_Face[] faces                                                                                                        | void                             |      |
|      | addFaces                               | final HE_HalfedgeStructure source                                                                                            | void                             |      |
|      | add                                    | final HE_Halfedge he                                                                                                         | void                             |      |
|      | addHalfedges                           | ()                                                                                                                           | void                             |      |
|      | addHalfedges                           | final HE_Halfedge[] halfedges                                                                                                | void                             |      |
|      | addHalfedges                           | final HE_HalfedgeStructure source                                                                                            | void                             |      |
|      | add                                    | final HE_Vertex v                                                                                                            | void                             |      |
|      | addVertices                            | final Collection<? extends HE_Vertex> vertices                                                                               | void                             |      |
|      | addVertices                            | final HE_HalfedgeStructure source                                                                                            | void                             |      |
|      | addVertices                            | final HE_Vertex[] vertices                                                                                                   | void                             |      |
|      | add                                    | final HE_Mesh mesh                                                                                                           | void                             |      |
|      | addSelection                           | final String name, final HE_Machine machine,final HE_Selection sel                                                           | void                             |      |
|      | addSelection                           | final String name, final HE_Selection sel                                                                                    | void                             |      |
|      | apply                                  | final WB_Transform3D T                                                                                                       | HE_Mesh                          |      |
|      | applySelf                              | final WB_Transform3D T                                                                                                       | HE_Mesh                          |      |
|      | apply2D                                | final WB_Transform2D T                                                                                                       | HE_Mesh                          |      |
|      | apply2DSelf                            | final WB_Transform2D T                                                                                                       | HE_Mesh                          |      |
|      | clean                                  | ()                                                                                                                           | void                             |      |
|      | cleanSelections                        | ()                                                                                                                           | void                             |      |
|      | cleanUnusedElementsByFace              | ()                                                                                                                           | HE_Mesh                          |      |
|      | removeUnconnectedElements              | ()                                                                                                                           | HE_Mesh                          |      |
|      | clear                                  | ()                                                                                                                           | void                             |      |
|      | clearEdges                             | ()                                                                                                                           | void                             |      |
|      | clearFace                              | final HE_Halfedge he                                                                                                         | void                             |      |
|      | clearFaces                             | ()                                                                                                                           | void                             |      |
|      | clearFacesNoSelectionCheck             | ()                                                                                                                           | void                             |      |
|      | clearHalfedge                          | final HE_Face f                                                                                                              | void                             |      |
|      | clearHalfedge                          | final HE_Vertex v                                                                                                            | void                             |      |
|      | clearHalfedges                         | ()                                                                                                                           | void                             |      |
|      | clearNext                              | final HE_Halfedge he                                                                                                         | void                             |      |
|      | clearPair                              | final HE_Halfedge he                                                                                                         | void                             |      |
|      | clearPrecomputed                       | ()                                                                                                                           | void                             |      |
|      | clearPrecomputedFaces                  | ()                                                                                                                           | void                             |      |
|      | clearPrecomputedHalfedges              | ()                                                                                                                           | void                             |      |
|      | clearPrecomputedVertices               | ()                                                                                                                           | void                             |      |
|      | clearPrev                              | final HE_Halfedge he                                                                                                         | void                             |      |
|      | clearSelections                        | ()                                                                                                                           | void                             |      |
|      | clearVertex                            | final HE_Halfedge he                                                                                                         | void                             |      |
|      | clearVertices                          | ()                                                                                                                           | void                             |      |
|      | clearVerticesNoSelectionCheck          | ()                                                                                                                           | void                             |      |
|      | clearVisitedElements                   | ()                                                                                                                           | void                             |      |
|      | contains                               | final HE_Element el                                                                                                          | boolean                          |      |
|      | contains                               | final HE_Face f                                                                                                              | boolean                          |      |
|      | contains                               | final HE_Halfedge he                                                                                                         | boolean                          |      |
|      | contains                               | final HE_Vertex v                                                                                                            | boolean                          |      |
|      | containsEdge                           | final long key                                                                                                               | boolean                          |      |
|      | containsFace                           | final long key                                                                                                               | boolean                          |      |
|      | containsHalfedge                       | final long key                                                                                                               | boolean                          |      |
|      | containsVertex                         | final long key                                                                                                               | boolean                          |      |
|      | copy                                   | ()                                                                                                                           | HE_Mesh                          |      |
|      | copySelection                          | final String from, final String to                                                                                           | HE_Selection                     |      |
|      | createThreaded                         | final HEC_Creator creator                                                                                                    | void                             |      |
|      | cutFace                                | final HE_Face f                                                                                                              | void                             |      |
|      | deleteEdge                             | final HE_Halfedge e                                                                                                          | HE_Face                          |      |
|      | deleteFace                             | final HE_Face f                                                                                                              | void                             |      |
|      | deleteFaces                            | final HE_Selection faces                                                                                                     | void                             |      |
|      | eItr                                   | ()                                                                                                                           | HE_EdgeIterator                  |      |
|      | fitInAABB                              | final WB_AABB AABB                                                                                                           | void                             |      |
|      | fitInAABB                              | final WB_AABB from, final WB_AABB to                                                                                         | void                             |      |
|      | fitInAABBConstrained                   | final WB_AABB AABB                                                                                                           | double                           |      |
|      | fitInAABBConstrained                   | final WB_AABB from, final WB_AABB to                                                                                         | double                           |      |
|      | fItr                                   | ()                                                                                                                           | HE_FaceIterator                  |      |
|      | fuse                                   | final HE_Mesh mesh                                                                                                           | void                             |      |
|      | get                                    | ()                                                                                                                           | HE_Mesh                          |      |
|      | getCenter                              | ()                                                                                                                           | WB_Point                         |      |
|      | getAllBoundaryHalfedges                | ()                                                                                                                           | List&lt;HE_Halfedge&gt;          |      |
|      | getAllBoundaryVertices                 | ()                                                                                                                           | List&lt;HE_Vertex&gt;            |      |
|      | getEdgeCenters                         | ()                                                                                                                           | WB_Point[]                       |      |
|      | getEdgeNormals                         | ()                                                                                                                           | WB_Vector[]                      |      |
|      | getEdges                               | ()                                                                                                                           | List&lt;HE_Halfedge&gt;          |      |
|      | getEdgesAsArray                        | ()                                                                                                                           | HE_Halfedge[]                    |      |
|      | getEdgesAsInt                          | ()                                                                                                                           | int[][]                          |      |
|      | getEdgeWithIndex                       | final int i                                                                                                                  | HE_Halfedge                      |      |
|      | getEdgeWithKey                         | final long key                                                                                                               | HE_Halfedge                      |      |
|      | getEulerCharacteristic                 | ()                                                                                                                           | int                              |      |
|      | getFaceCenter                          | final int id                                                                                                                 | WB_Point                         |      |
|      | getFaceCenters                         | ()                                                                                                                           | WB_Point[]                       |      |
|      | getFaceColors                          | ()                                                                                                                           | int[]                            |      |
|      | getFaceInternalLabels                  | ()                                                                                                                           | int[]                            |      |
|      | getFaceNormal                          | final int id                                                                                                                 | WB_Vector                        |      |
|      | getFaceNormals                         | ()                                                                                                                           | WB_Vector[]                      |      |
|      | getFacePlanes                          | ()                                                                                                                           | WB_Plane[]                       |      |
|      | getFaces                               | ()                                                                                                                           | List&lt;HE_Face&gt;              |      |
|      | getFacesAsArray                        | ()                                                                                                                           | HE_Face[]                        |      |
|      | getFacesAsInt                          | ()                                                                                                                           | int[][]                          |      |
|      | getFaceTextureIds                      | ()                                                                                                                           | int[]                            |      |
|      | getFaceTree                            | ()                                                                                                                           | WB_KDTree3D&lt;WB_Point,Long&gt; |      |
|      | getFaceUserLabels                      | ()                                                                                                                           | int[]                            |      |
|      | getFaceVisibility                      | ()                                                                                                                           | boolean[]                        |      |
|      | getFaceWithIndex                       | final int i                                                                                                                  | HE_Face                          |      |
|      | getFaceWithKey                         | final long key                                                                                                               | HE_Face                          |      |
|      | getHalfedgeFromTo                      | final HE_Vertex v0,final HE_Vertex v1                                                                                        | HE_Halfedge                      |      |
|      | getHalfedges                           | ()                                                                                                                           | List&lt;HE_Halfedge&gt;          |      |
|      | getHalfedgesAsArray                    | ()                                                                                                                           | HE_Halfedge[]                    |      |
|      | getHalfedgeWithIndex                   | final int i                                                                                                                  | HE_Halfedge                      |      |
|      | getHalfedgeWithKey                     | final long key                                                                                                               | HE_Halfedge                      |      |
|      | getIndex                               | final HE_Face f                                                                                                              | int                              |      |
|      | getIndex                               | final HE_Halfedge edge                                                                                                       | int                              |      |
|      | getIndex                               | final HE_Vertex v                                                                                                            | int                              |      |
|      | getKeyedEdgeCenters                    | ()                                                                                                                           | Map&lt;Long,WB_Point&gt;         |      |
|      | getKeyedEdgeNormals                    | ()                                                                                                                           | Map&lt;Long,WB_Vector&gt;        |      |
|      | getKeyedFaceCenters                    | ()                                                                                                                           | Map&lt;Long,WB_Point&gt;         |      |
|      | getKeyedFaceNormals                    | ()                                                                                                                           | Map&lt;Long,WB_Vector&gt;        |      |
|      | getKeyedVertexNormals                  | ()                                                                                                                           | Map&lt;Long,WB_Vector&gt;        |      |
|      | getMeanEdgeLength                      | ()                                                                                                                           | double                           |      |
|      | getName                                | ()                                                                                                                           | String                           |      |
|      | getNewSelection                        | ()                                                                                                                           | HE_Selection                     |      |
|      | getNewSelection                        | final String name                                                                                                            | HE_Selection                     |      |
|      | getNetwork                             | ()                                                                                                                           | WB_Network                       |      |
|      | getNumberOfEdges                       | ()                                                                                                                           | int                              |      |
|      | getNumberOfFaces                       | ()                                                                                                                           | int                              |      |
|      | getNumberOfHalfedges                   | ()                                                                                                                           | int                              |      |
|      | getNumberOfVertices                    | ()                                                                                                                           | int                              |      |
|      | getPoints                              | ()                                                                                                                           | WB_CoordCollection               |      |
|      | getPolygonList                         | ()                                                                                                                           | List&lt;WB_Polygon&gt;           |      |
|      | getPolygons                            | ()                                                                                                                           | WB_Polygon[]                     |      |
|      | getSegments                            | ()                                                                                                                           | WB_Segment[]                     |      |
|      | getSelection                           | final String name                                                                                                            | HE_Selection                     |      |
|      | getSelectionNames                      | ()                                                                                                                           | Set&lt;String&gt;                |      |
|      | selectionCheck                         | ()                                                                                                                           | void                             |      |
|      | getSharedFaces                         | final HE_Vertex v1,final HE_Vertex v2                                                                                        | List&lt;HE_Face&gt;              |      |
|      | getTriangles                           | ()                                                                                                                           | int[]                            |      |
|      | getUnpairedHalfedges                   | ()                                                                                                                           | List&lt;HE_Halfedge&gt;          |      |
|      | getVertex                              | final int i                                                                                                                  | WB_Coord                         |      |
|      | getVertexColors                        | ()                                                                                                                           | int[]                            |      |
|      | getVertexInternalLabels                | ()                                                                                                                           | int[]                            |      |
|      | getVertexKeyToIndexMap                 | ()                                                                                                                           | Map&lt;Long,Integer&gt;          |      |
|      | getVertexNormal                        | final int i                                                                                                                  | WB_Vector                        |      |
|      | getVertexNormals                       | ()                                                                                                                           | WB_Vector[]                      |      |
|      | getVertexTree                          | ()                                                                                                                           | WB_KDTree3D&lt;WB_Coord,Long&gt; |      |
|      | getVertexUserLabels                    | ()                                                                                                                           | int[]                            |      |
|      | getVertexVisibility                    | ()                                                                                                                           | boolean[]                        |      |
|      | getVertexWithIndex                     | final int i                                                                                                                  | HE_Vertex                        |      |
|      | getPositionWithIndex                   | final int i                                                                                                                  | WB_Point                         |      |
|      | getVertexWithKey                       | final long key                                                                                                               | HE_Vertex                        |      |
|      | getVertices                            | ()                                                                                                                           | List&lt;HE_Vertex&gt;            |      |
|      | getVerticesAsArray                     | ()                                                                                                                           | HE_Vertex[]                      |      |
|      | getVerticesAsCoord                     | ()                                                                                                                           | List&lt;WB_Coord&gt;             |      |
|      | getVerticesAsDouble                    | ()                                                                                                                           | double[][]                       |      |
|      | getVerticesAsFloat                     | ()                                                                                                                           | float[][]                        |      |
|      | heItr                                  | ()                                                                                                                           | HE_HalfedgeIterator              |      |
|      | isFinished                             | ()                                                                                                                           | boolean                          |      |
|      | isNeighbor                             | final HE_RAS<HE_Face> partition1,final HE_RAS<HE_Face> partition2                                                            | boolean                          |      |
|      | isSurface                              | ()                                                                                                                           | boolean                          |      |
|      | modify                                 | final HEM_Modifier modifier                                                                                                  | HE_Mesh                          |      |
|      | modifyThreaded                         | final HEM_Modifier modifier                                                                                                  | void                             |      |
|      | move                                   | final double x, final double y, final double z                                                                               | HE_Mesh                          |      |
|      | move                                   | final WB_Coord v                                                                                                             | HE_Mesh                          |      |
|      | moveSelf                               | final double x, final double y, final double z                                                                               | HE_Mesh                          |      |
|      | moveSelf                               | final WB_Coord v                                                                                                             | HE_Mesh                          |      |
|      | moveTo                                 | final double x, final double y, final double z                                                                               | HE_Mesh                          |      |
|      | moveTo                                 | final WB_Coord v                                                                                                             | HE_Mesh                          |      |
|      | moveToSelf                             | final double x, final double y, final double z                                                                               | HE_Mesh                          |      |
|      | moveToSelf                             | final WB_Coord v                                                                                                             | HE_Mesh                          |      |
|      | remove                                 | final HE_Face f                                                                                                              | void                             |      |
|      | remove                                 | final HE_Halfedge he                                                                                                         | void                             |      |
|      | remove                                 | final HE_Vertex v                                                                                                            | void                             |      |
|      | removeEdges                            | final Collection<? extends HE_Halfedge> edges                                                                                | void                             |      |
|      | removeEdges                            | final HE_Halfedge[] edges                                                                                                    | void                             |      |
|      | removeFaces                            | final Collection<? extends HE_Face> faces                                                                                    | void                             |      |
|      | removeFaces                            | final HE_Face[] faces                                                                                                        | void                             |      |
|      | removeHalfedges                        | ()                                                                                                                           | void                             |      |
|      | removeHalfedges                        | final HE_Halfedge[] halfedges                                                                                                | void                             |      |
|      | removeNoSelectionCheck                 | final HE_Halfedge he                                                                                                         | void                             |      |
|      | removeSelection                        | final String name                                                                                                            | HE_Selection                     |      |
|      | removeVertices                         | final Collection<? extends HE_Vertex> vertices                                                                               | void                             |      |
|      | removeVertices                         | final HE_Vertex[] vertices                                                                                                   | void                             |      |
|      | renameSelection                        | final String from, final String to                                                                                           | boolean                          |      |
|      | replaceFaces                           | final HE_Mesh mesh                                                                                                           | void                             |      |
|      | replaceHalfedges                       | final HE_Mesh mesh                                                                                                           | void                             |      |
|      | replaceSelection                       | final String name, final HE_Machine machine,final HE_Selection sel                                                           | HE_Selection                     |      |
|      | replaceSelection                       | final String name,final HE_Selection sel                                                                                     | HE_Selection                     |      |
|      | replaceVertices                        | final HE_Mesh mesh                                                                                                           | void                             |      |
|      | resetEdgeInternalLabels                | ()                                                                                                                           | void                             |      |
|      | resetEdgeUserLabels                    | ()                                                                                                                           | void                             |      |
|      | resetFaceInternalLabels                | ()                                                                                                                           | void                             |      |
|      | resetFaceUserLabels                    | ()                                                                                                                           | void                             |      |
|      | resetHalfedgeInternalLabels            | ()                                                                                                                           | void                             |      |
|      | resetHalfedgeUserLabels                | ()                                                                                                                           | void                             |      |
|      | resetInternalLabels                    | ()                                                                                                                           | void                             |      |
|      | resetUserLabels                        | ()                                                                                                                           | void                             |      |
|      | resetVertexInternalLabels              | ()                                                                                                                           | void                             |      |
|      | resetVertexUserLabels                  | ()                                                                                                                           | void                             |      |
|      | rotateAboutAxis                        | final double angle, final double px,final double py, final double pz, final double ax, final double ay,final double az       | HE_Mesh                          |      |
|      | rotateAboutAxis                        | final double angle, final WB_Coord p,final WB_Coord a                                                                        | HE_Mesh                          |      |
|      | rotateAboutAxis2P                      | final double angle, final double p1x,final double p1y, final double p1z, final double p2x,final double p2y, final double p2z | HE_Mesh                          |      |
|      | rotateAboutAxis2P                      | final double angle, final WB_Coord p1,final WB_Coord p2                                                                      | HE_Mesh                          |      |
|      | rotateAboutAxis2PSelf                  | final double angle, final double p1x,final double p1y, final double p1z, final double p2x,final double p2y, final double p2z | HE_Mesh                          |      |
|      | rotateAboutAxis2PSelf                  | final double angle, final WB_Coord p1,final WB_Coord p2                                                                      | HE_Mesh                          |      |
|      | rotateAboutAxisSelf                    | final double angle, final double px,final double py, final double pz, final double ax, final double ay,final double az       | HE_Mesh                          |      |
|      | rotateAboutAxisSelf                    | final double angle, final WB_Coord p,final WB_Coord a                                                                        | HE_Mesh                          |      |
|      | rotateAboutCenter                      | final double angle, final double ax,final double ay, final double az                                                         | HE_Mesh                          |      |
|      | rotateAboutCenter                      | final double angle, final WB_Coord a                                                                                         | HE_Mesh                          |      |
|      | rotateAboutCenterSelf                  | final double angle, final double ax,final double ay, final double az                                                         | HE_Mesh                          |      |
|      | rotateAboutCenterSelf                  | final double angle, final WB_Coord a                                                                                         | HE_Mesh                          |      |
|      | rotateAboutOrigin                      | final double angle, final double ax,final double ay, final double az                                                         | HE_Mesh                          |      |
|      | rotateAboutOrigin                      | final double angle, final WB_Coord a                                                                                         | HE_Mesh                          |      |
|      | rotateAboutOriginSelf                  | final double angle, final double ax,final double ay, final double az                                                         | HE_Mesh                          |      |
|      | rotateAboutOriginSelf                  | final double angle, final WB_Coord a                                                                                         | HE_Mesh                          |      |
|      | scale                                  | final double scaleFactor                                                                                                     | HE_Mesh                          |      |
|      | scale                                  | final double scaleFactorx, final double scaleFactory,final double scaleFactorz                                               | HE_Mesh                          |      |
|      | scale                                  | final double scaleFactorx, final double scaleFactory,final double scaleFactorz, final WB_Coord c                             | HE_Mesh                          |      |
|      | scale                                  | final double scaleFactor, final WB_Coord c                                                                                   | HE_Mesh                          |      |
|      | scaleSelf                              | final double scaleFactor                                                                                                     | HE_Mesh                          |      |
|      | scaleSelf                              | final double scaleFactorx,final double scaleFactory, final double scaleFactorz                                               | HE_Mesh                          |      |
|      | scaleSelf                              | final double scaleFactorx,final double scaleFactory, final double scaleFactorz,final WB_Coord c                              | HE_Mesh                          |      |
|      | scaleSelf                              | final double scaleFactor, final WB_Coord c                                                                                   | HE_Mesh                          |      |
|      | selectAll                              | ()                                                                                                                           | HE_Selection                     |      |
|      | selectAll                              | final String name                                                                                                            | HE_Selection                     |      |
|      | selectAllEdges                         | ()                                                                                                                           | HE_Selection                     |      |
|      | selectAllEdges                         | final String name                                                                                                            | HE_Selection                     |      |
|      | selectAllFaces                         | ()                                                                                                                           | HE_Selection                     |      |
|      | selectAllFaces                         | final String name                                                                                                            | HE_Selection                     |      |
|      | selectFaces                            | int start, int stop                                                                                                          | HE_Selection                     |      |
|      | selectFaces                            | final String name, int start, int stop                                                                                       | HE_Selection                     |      |
|      | selectAllHalfedges                     | ()                                                                                                                           | HE_Selection                     |      |
|      | selectAllHalfedges                     | final String name                                                                                                            | HE_Selection                     |      |
|      | selectAllInnerBoundaryHalfedges        | ()                                                                                                                           | HE_Selection                     |      |
|      | selectAllInnerBoundaryHalfedges        | final String name                                                                                                            | HE_Selection                     |      |
|      | selectAllOuterBoundaryHalfedges        | ()                                                                                                                           | HE_Selection                     |      |
|      | selectAllOuterBoundaryHalfedges        | final String name                                                                                                            | HE_Selection                     |      |
|      | selectAllVertices                      | ()                                                                                                                           | HE_Selection                     |      |
|      | selectAllVertices                      | final String name                                                                                                            | HE_Selection                     |      |
|      | selectBackEdges                        | final String name, final WB_Plane P                                                                                          | HE_Selection                     |      |
|      | selectBackEdges                        | final WB_Plane P                                                                                                             | HE_Selection                     |      |
|      | selectBackFaces                        | final String name, final WB_Plane P                                                                                          | HE_Selection                     |      |
|      | selectBackFaces                        | final WB_Plane P                                                                                                             | HE_Selection                     |      |
|      | selectBackVertices                     | final String name,final WB_Plane P                                                                                           | HE_Selection                     |      |
|      | selectBackVertices                     | final WB_Plane P                                                                                                             | HE_Selection                     |      |
|      | selectBoundaryEdges                    | ()                                                                                                                           | HE_Selection                     |      |
|      | selectBoundaryEdges                    | final String name                                                                                                            | HE_Selection                     |      |
|      | selectBoundaryFaces                    | ()                                                                                                                           | HE_Selection                     |      |
|      | selectBoundaryFaces                    | final String name                                                                                                            | HE_Selection                     |      |
|      | selectBoundaryVertices                 | ()                                                                                                                           | HE_Selection                     |      |
|      | selectBoundaryVertices                 | final String name                                                                                                            | HE_Selection                     |      |
|      | selectCrossingEdges                    | final String name,final WB_Plane P                                                                                           | HE_Selection                     |      |
|      | selectCrossingEdges                    | final WB_Plane P                                                                                                             | HE_Selection                     |      |
|      | selectCrossingFaces                    | final String name,final WB_Plane P                                                                                           | HE_Selection                     |      |
|      | selectCrossingFaces                    | final WB_Plane P                                                                                                             | HE_Selection                     |      |
|      | selectEdgesWithLabel                   | final int label                                                                                                              | HE_Selection                     |      |
|      | selectEdgesWithLabel                   | final String name,final int label                                                                                            | HE_Selection                     |      |
|      | selectEdgesWithOtherInternalLabel      | final int label                                                                                                              | HE_Selection                     |      |
|      | selectEdgesWithOtherInternalLabel      | final String name,final int label                                                                                            | HE_Selection                     |      |
|      | selectEdgesWithOtherLabel              | final int label                                                                                                              | HE_Selection                     |      |
|      | selectEdgesWithOtherLabel              | final String name,final int label                                                                                            | HE_Selection                     |      |
|      | selectEdgesWithInternalLabel           | final int label                                                                                                              | HE_Selection                     |      |
|      | selectEdgesWithInternalLabel           | final String name,final int label                                                                                            | HE_Selection                     |      |
|      | selectFacesWithInternalLabel           | final int label                                                                                                              | HE_Selection                     |      |
|      | selectFacesWithInternalLabel           | final String name,final int label                                                                                            | HE_Selection                     |      |
|      | selectFacesWithLabel                   | final int label                                                                                                              | HE_Selection                     |      |
|      | selectFacesWithLabel                   | final String name,final int label                                                                                            | HE_Selection                     |      |
|      | selectFacesWithNormal                  | final String name,final WB_Coord v                                                                                           | HE_Selection                     |      |
|      | selectFacesWithNormal                  | final String name,final WB_Coord n, final double ta                                                                          | HE_Selection                     |      |
|      | selectFacesWithNormal                  | final WB_Coord v                                                                                                             | HE_Selection                     |      |
|      | selectFacesWithNormal                  | final WB_Coord n,final double ta                                                                                             | HE_Selection                     |      |
|      | selectFacesWithOtherInternalLabel      | final int label                                                                                                              | HE_Selection                     |      |
|      | selectFacesWithOtherInternalLabel      | final String name,final int label                                                                                            | HE_Selection                     |      |
|      | selectFacesWithOtherLabel              | final int label                                                                                                              | HE_Selection                     |      |
|      | selectFacesWithOtherLabel              | final String name,final int label                                                                                            | HE_Selection                     |      |
|      | selectFrontEdges                       | final String name, final WB_Plane P                                                                                          | HE_Selection                     |      |
|      | selectFrontEdges                       | final WB_Plane P                                                                                                             | HE_Selection                     |      |
|      | selectFrontFaces                       | final String name, final WB_Plane P                                                                                          | HE_Selection                     |      |
|      | selectFrontFaces                       | final WB_Plane P                                                                                                             | HE_Selection                     |      |
|      | selectFrontVertices                    | final String name,final WB_Plane P                                                                                           | HE_Selection                     |      |
|      | selectFrontVertices                    | final WB_Plane P                                                                                                             | HE_Selection                     |      |
|      | selectHalfedgesWithLabel               | final int label                                                                                                              | HE_Selection                     |      |
|      | selectHalfedgesWithLabel               | final String name,final int label                                                                                            | HE_Selection                     |      |
|      | selectHalfedgesWithOtherInternalLabel  | final int label                                                                                                              | HE_Selection                     |      |
|      | selectHalfedgesWithOtherInternalLabel  | final String name,final int label                                                                                            | HE_Selection                     |      |
|      | selectHalfedgesWithOtherLabel          | final int label                                                                                                              | HE_Selection                     |      |
|      | selectHalfedgesWithOtherLabel          | final String name,final int label                                                                                            | HE_Selection                     |      |
|      | selectHalfedgeWithInternalLabel        | final int label                                                                                                              | HE_Selection                     |      |
|      | selectHalfedgeWithInternalLabel        | final String name,final int label                                                                                            | HE_Selection                     |      |
|      | selectOnVertices                       | final String name, final WB_Plane P                                                                                          | HE_Selection                     |      |
|      | selectOnVertices                       | final WB_Plane P                                                                                                             | HE_Selection                     |      |
|      | selectRandomEdges                      | final double r                                                                                                               | HE_Selection                     |      |
|      | selectRandomEdges                      | final double r, final long seed                                                                                              | HE_Selection                     |      |
|      | selectRandomEdges                      | final String name, final double r                                                                                            | HE_Selection                     |      |
|      | selectRandomEdges                      | final String name, final double r,final long seed                                                                            | HE_Selection                     |      |
|      | selectRandomFaces                      | final double r                                                                                                               | HE_Selection                     |      |
|      | selectRandomFaces                      | final double r, final long seed                                                                                              | HE_Selection                     |      |
|      | selectRandomFaces                      | final String name, final double r                                                                                            | HE_Selection                     |      |
|      | selectRandomFaces                      | final String name, final double r,final long seed                                                                            | HE_Selection                     |      |
|      | selectRandomVertices                   | final double r                                                                                                               | HE_Selection                     |      |
|      | selectRandomVertices                   | final double r, final long seed                                                                                              | HE_Selection                     |      |
|      | selectRandomVertices                   | final String name,final double r                                                                                             | HE_Selection                     |      |
|      | selectRandomVertices                   | final String name, final double r,final long seed                                                                            | HE_Selection                     |      |
|      | selectVerticesWithInternalLabel        | final int label                                                                                                              | HE_Selection                     |      |
|      | selectVerticesWithInternalLabel        | final String name,final int label                                                                                            | HE_Selection                     |      |
|      | selectVerticesWithLabel                | final int label                                                                                                              | HE_Selection                     |      |
|      | selectVerticesWithLabel                | final String name,final int label                                                                                            | HE_Selection                     |      |
|      | selectVerticesWithOtherInternalLabel   | final int label                                                                                                              | HE_Selection                     |      |
|      | selectVerticesWithOtherInternalLabel   | final String name,final int label                                                                                            | HE_Selection                     |      |
|      | selectVerticesWithOtherLabel           | final int label                                                                                                              | HE_Selection                     |      |
|      | selectVerticesWithOtherLabel           | final String name,final int label                                                                                            | HE_Selection                     |      |
|      | set                                    | final HE_Mesh target                                                                                                         | void                             |      |
|      | setEdgeInternalLabels                  | final int label                                                                                                              | void                             |      |
|      | setEdgeUserLabels                      | final int label                                                                                                              | void                             |      |
|      | setFace                                | final HE_Halfedge he, final HE_Face f                                                                                        | void                             |      |
|      | setFaceColor                           | final int color                                                                                                              | void                             |      |
|      | setFaceColorWithInternalLabel          | final int color, final int i                                                                                                 | void                             |      |
|      | setFaceColorWithOtherInternalLabel     | final int color,final int i                                                                                                  | void                             |      |
|      | setFaceColorWithOtherUserLabel         | final int color, final int i                                                                                                 | void                             |      |
|      | setFaceColorWithUserLabel              | final int color, final int i                                                                                                 | void                             |      |
|      | setFaceInternalLabels                  | final int label                                                                                                              | void                             |      |
|      | setFaceUserLabels                      | final int label                                                                                                              | void                             |      |
|      | setHalfedge                            | final HE_Face f, final HE_Halfedge he                                                                                        | void                             |      |
|      | setHalfedge                            | final HE_Vertex v, final HE_Halfedge he                                                                                      | void                             |      |
|      | setHalfedgeColor                       | final int color                                                                                                              | void                             |      |
|      | setHalfedgeColorWithInternalLabel      | final int color,final int i                                                                                                  | void                             |      |
|      | setHalfedgeColorWithOtherInternalLabel | final int color,final int i                                                                                                  | void                             |      |
|      | setHalfedgeColorWithOtherUserLabel     | final int color,final int i                                                                                                  | void                             |      |
|      | setHalfedgeColorWithUserLabel          | final int color, final int i                                                                                                 | void                             |      |
|      | setHalfedgeInternalLabels              | final int label                                                                                                              | void                             |      |
|      | setHalfedgeUserLabels                  | final int label                                                                                                              | void                             |      |
|      | setName                                | final String name                                                                                                            | void                             |      |
|      | setNext                                | final HE_Halfedge he, final HE_Halfedge hen                                                                                  | void                             |      |
|      | setNoCopy                              | final HE_Mesh target                                                                                                         | void                             |      |
|      | setPair                                | final HE_Halfedge he1, final HE_Halfedge he2                                                                                 | void                             |      |
|      | setPairNoSelectionCheck                | final HE_Halfedge he1,final HE_Halfedge he2                                                                                  | void                             |      |
|      | setVertex                              | final HE_Halfedge he, final HE_Vertex v                                                                                      | void                             |      |
|      | setVertex                              | final HE_Vertex v, final double x, final double y                                                                            | void                             |      |
|      | setVertex                              | final HE_Vertex v, final double x, final double y,final double z                                                             | void                             |      |
|      | setVertex                              | final HE_Vertex v, final WB_Coord c                                                                                          | void                             |      |
|      | setVertexColor                         | final int color                                                                                                              | void                             |      |
|      | setVertexColorWithInternalLabel        | final int color, final int i                                                                                                 | void                             |      |
|      | setVertexColorWithOtherInternalLabel   | final int color,final int i                                                                                                  | void                             |      |
|      | setVertexColorWithOtherUserLabel       | final int color, final int i                                                                                                 | void                             |      |
|      | setVertexColorWithUserLabel            | final int color, final int i                                                                                                 | void                             |      |
|      | setVertexInternalLabels                | final int label                                                                                                              | void                             |      |
|      | setVertexUserLabels                    | final int label                                                                                                              | void                             |      |
|      | setVertexWithIndex                     | final int index, final double x,final double y                                                                               | void                             |      |
|      | setVertexWithIndex                     | final int index, final double x,final double y, final double z                                                               | void                             |      |
|      | setVertexWithIndex                     | final int index, final WB_Coord c                                                                                            | void                             |      |
|      | setVertexWithKey                       | final long key, final double x,final double y                                                                                | void                             |      |
|      | setVertexWithKey                       | final long key, final double x, final double y,final double z                                                                | void                             |      |
|      | setVertexWithKey                       | final long key, final WB_Coord c                                                                                             | void                             |      |
|      | setVerticesFromDouble                  | final double[][] values                                                                                                      | void                             |      |
|      | setVerticesFromFloat                   | final double[] values                                                                                                        | void                             |      |
|      | setVerticesFromFloat                   | final float[] values                                                                                                         | void                             |      |
|      | setVerticesFromFloat                   | final float[][] values                                                                                                       | void                             |      |
|      | setVerticesFromFloat                   | final int[] values                                                                                                           | void                             |      |
|      | setVerticesFromInt                     | final int[][] values                                                                                                         | void                             |      |
|      | setVerticesFromPoint                   | final List<? extends WB_Coord> values                                                                                        | void                             |      |
|      | setVerticesFromPoint                   | final WB_Coord[] values                                                                                                      | void                             |      |
|      | simplify                               | final HES_Simplifier simplifier                                                                                              | HE_Mesh                          |      |
|      | simplifyThreaded                       | final HES_Simplifier simplifier                                                                                              | void                             |      |
|      | smooth                                 | ()                                                                                                                           | void                             |      |
|      | smooth                                 | final int rep                                                                                                                | void                             |      |
|      | sort                                   | ()                                                                                                                           | void                             |      |
|      | sort                                   | final HE_FaceSort faceSort,final HE_VertexSort vertexSort                                                                    | void                             |      |
|      | subdivide                              | final HES_Subdividor subdividor                                                                                              | HE_Mesh                          |      |
|      | subdivide                              | final HES_Subdividor subdividor, final int rep                                                                               | HE_Mesh                          |      |
|      | subdivideThreaded                      | final HES_Subdividor subdividor                                                                                              | void                             |      |
|      | subdivideThreaded                      | final HES_Subdividor subdividor,final int rep                                                                                | void                             |      |
|      | toSimpleMesh                           | ()                                                                                                                           | WB_SimpleMesh                    |      |
|      | toString                               | ()                                                                                                                           | String                           |      |
|      | transform                              | final WB_Transform3D T                                                                                                       | HE_Mesh                          |      |
|      | transformSelf                          | final WB_Transform3D T                                                                                                       | HE_Mesh                          |      |
|      | uncapBoundaryHalfedges                 | ()                                                                                                                           | void                             |      |
|      | update                                 | ()                                                                                                                           | void                             |      |
|      | validate                               | ()                                                                                                                           | boolean                          |      |
|      | vItr                                   | ()                                                                                                                           | HE_VertexIterator                |      |
|      | stats                                  | ()                                                                                                                           | void                             |      |
|      | getAABB                                | ()                                                                                                                           | WB_AABB                          |      |
|      | triangulate                            | ()                                                                                                                           | void                             |      |

### CreatorThread

<br>
#### implements:  Callable&lt;HE_Mesh&gt;
<br>


- **构造方法**

| 属性   | 方法名           | 参数                        | 返回值           | 备注   |
|:-----|:--------------|:--------------------------|:--------------|:-----|
|      | CreatorThread | final HEC_Creator creator | CreatorThread |      |

- **成员方法**

| 属性   | 方法名   | 参数   | 返回值     | 备注   |
|:-----|:------|:-----|:--------|:-----|
|      | call  | ()   | HE_Mesh |      |

### ModifierThread

<br>
#### implements:  Callable&lt;HE_Mesh&gt;
<br>


- **构造方法**

| 属性   | 方法名            | 参数                                             | 返回值            | 备注   |
|:-----|:---------------|:-----------------------------------------------|:---------------|:-----|
|      | ModifierThread | final HEM_Modifier machine, final HE_Mesh mesh | ModifierThread |      |

- **成员方法**

| 属性   | 方法名   | 参数   | 返回值     | 备注   |
|:-----|:------|:-----|:--------|:-----|
|      | call  | ()   | HE_Mesh |      |

### SimplifierThread

<br>
#### implements:  Callable&lt;HE_Mesh&gt;
<br>


- **构造方法**

| 属性   | 方法名              | 参数                                               | 返回值              | 备注   |
|:-----|:-----------------|:-------------------------------------------------|:-----------------|:-----|
|      | SimplifierThread | final HES_Simplifier machine, final HE_Mesh mesh | SimplifierThread |      |

- **成员方法**

| 属性   | 方法名   | 参数   | 返回值     | 备注   |
|:-----|:------|:-----|:--------|:-----|
|      | call  | ()   | HE_Mesh |      |

### SubdividorThread

<br>
#### implements:  Callable&lt;HE_Mesh&gt;
<br>


- **构造方法**

| 属性   | 方法名              | 参数                                               | 返回值              | 备注   |
|:-----|:-----------------|:-------------------------------------------------|:-----------------|:-----|
|      | SubdividorThread | final HES_Subdividor machine, final HE_Mesh mesh | SubdividorThread |      |
|      | setNoCopy        | new HE_Mesh                                      | setNoCopy        |      |

- **成员方法**

| 属性   | 方法名   | 参数   | 返回值          | 备注   |
|:-----|:------|:-----|:-------------|:-----|
|      | call  | ()   | HE_Mesh      |      |
|      |       | this | synchronized |      |