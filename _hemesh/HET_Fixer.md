---
navs: []
tags: [He_tools]
image:
title: HET_Fixer
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
            


### HET_Fixer

<br>


- **成员方法**

| 属性     | 方法名                           | 参数                                   | 返回值          | 备注   |
|:-------|:------------------------------|:-------------------------------------|:-------------|:-----|
|        | fixHalfedgeFaceAssignment     | final HE_Mesh mesh                   | void         |      |
|        | fixHalfedgeVertexAssignment   | final HE_Mesh mesh                   | void         |      |
| static | deleteTwoEdgeFace             | final HE_Mesh mesh, final HE_Face f  | void         |      |
| static | deleteTwoEdgeFaces            | final HE_Mesh mesh                   | void         |      |
| static | deleteTwoEdgeVertex           | final HE_Mesh mesh,final HE_Vertex v | void         |      |
| static | deleteTwoEdgeVertices         | final HE_Mesh mesh                   | void         |      |
| static | collapseDegenerateEdges       | final HE_Mesh mesh                   | void         |      |
| static | collapseDegenerateEdges       | final HE_Mesh mesh,final double d    | void         |      |
| static | fixNonManifoldVerticesOnePass | final HE_Mesh mesh                   | boolean      |      |
| static | fixDegenerateTriangles        | final HE_Mesh mesh                   | void         |      |
| static | fixNonManifoldVertices        | final HE_Mesh mesh                   | void         |      |
| static | deleteCollinearVertices       | final HE_Mesh mesh                   | void         |      |
| static | selectCollinearVertices       | final HE_Mesh mesh                   | HE_Selection |      |
| static | selectVerticesWithDegree      | int degree,final HE_Mesh mesh        | HE_Selection |      |
| static | deleteDegenerateTriangles     | final HE_Mesh mesh                   | void         |      |
| static | clean                         | final HE_Mesh mesh                   | void         |      |
| static | fixLoops                      | final HE_Mesh mesh                   | void         |      |
| static | findTJunctions                | final HE_Mesh mesh                   | void         |      |
| static | fixTJunctions                 | final HE_Mesh mesh                   | void         |      |
| static | deleteDanglingEdgesOnePass    | final HE_Mesh mesh                   | boolean      |      |
| static | deleteDanglingEdges           | final HE_Mesh mesh                   | void         |      |
| static | findSubmeshes                 | HE_Mesh mesh                         | int          |      |
| static | unifyNormals                  | HE_Mesh mesh                         | void         |      |

### VertexInfo

<br>


- **构造方法**

| 属性   | 方法名        | 参数   | 返回值        | 备注   |
|:-----|:-----------|:-----|:-----------|:-----|
|      | VertexInfo | ()   | VertexInfo |      |