---
navs: []
tags: [He_tools,io]
image:
title: HET_Export
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
            


### HET_Export

<br>


- **成员方法**

| 属性     | 方法名                      | 参数                                                                                 | 返回值   | 备注   |
|:-------|:-------------------------|:-----------------------------------------------------------------------------------|:------|:-----|
| static | saveToOBJ                | final HE_Mesh mesh, final String path,final String name                            | void  |      |
| static | saveAsOBJ                | final HE_Mesh mesh, final String path,final String name                            | void  |      |
| static | saveToOBJNN              | final HE_Mesh mesh, final String path,final String name                            | void  |      |
| static | saveAsOBJNoNormals       | final HE_Mesh mesh, final String path,final String name                            | void  |      |
| static | saveToOBJWithFaceColor   | final HE_Mesh mesh,final String path, final String name                            | void  |      |
| static | saveAsOBJWithFaceColor   | final HE_Mesh mesh,final String path, final String name                            | void  |      |
| static | saveToOBJWithVertexColor | final HE_Mesh mesh,final String path, final String name                            | void  |      |
| static | saveAsOBJWithVertexColor | final HE_Mesh mesh,final String path, final String name                            | void  |      |
| static | saveToOBJ                | final Collection<? extends HE_Mesh> mesh,final String path, final String name      | void  |      |
| static | saveAsOBJ                | final Collection<? extends HE_Mesh> mesh,final String path, final String name      | void  |      |
| static | saveToOBJ                | final HE_MeshCollection mesh,final String path, final String name                  | void  |      |
| static | saveAsOBJ                | final HE_MeshCollection mesh,final String path, final String name                  | void  |      |
| static | saveToOBJNN              | final Collection<? extends HE_Mesh> mesh,final String path, final String name      | void  |      |
| static | saveAsOBJNoNormals       | ()                                                                                 | void  |      |
| static | saveToOBJNN              | final HE_MeshCollection mesh,final String path, final String name                  | void  |      |
| static | saveAsOBJNoNormals       | final HE_MeshCollection mesh,final String path, final String name                  | void  |      |
| static | saveToOBJWithFaceColor   | ()                                                                                 | void  |      |
| static | saveAsOBJWithFaceColor   | ()                                                                                 | void  |      |
| static | saveToOBJWithFaceColor   | final HE_MeshCollection mesh,final String path, final String name                  | void  |      |
| static | saveAsOBJWithFaceColor   | final HE_MeshCollection mesh,final String path, final String name                  | void  |      |
| static | saveToOBJWithVertexColor | ()                                                                                 | void  |      |
| static | saveAsOBJWithVertexColor | ()                                                                                 | void  |      |
| static | saveToOBJWithVertexColor | final HE_MeshCollection mesh,final String path, final String name                  | void  |      |
| static | saveAsOBJWithVertexColor | final HE_MeshCollection mesh,final String path, final String name                  | void  |      |
| static | saveToOBJ                | final HE_Mesh[] mesh, final String path,final String name                          | void  |      |
| static | saveAsOBJ                | final HE_Mesh[] mesh, final String path,final String name                          | void  |      |
| static | saveToOBJNN              | final HE_Mesh[] mesh, final String path,final String name                          | void  |      |
| static | saveAsOBJNoNormals       | final HE_Mesh[] mesh,final String path, final String name                          | void  |      |
| static | saveToOBJWithFaceColor   | final HE_Mesh[] mesh,final String path, final String name                          | void  |      |
| static | saveAsOBJWithFaceColor   | final HE_Mesh[] mesh,final String path, final String name                          | void  |      |
| static | saveToOBJWithVertexColor | final HE_Mesh[] mesh,final String path, final String name                          | void  |      |
| static | saveAsOBJWithVertexColor | final HE_Mesh[] mesh,final String path, final String name                          | void  |      |
| static | saveToSTL                | final HE_Mesh mesh, final String path,final String name                            | void  |      |
| static | saveAsSTL                | final HE_Mesh mesh, final String path,final String name                            | void  |      |
| static | saveToSTLWithFaceColor   | final HE_Mesh mesh,final String path, final String name, final int colormodel      | void  |      |
| static | saveAsSTLWithFaceColor   | final HE_Mesh mesh,final String path, final String name, final int colormodel      | void  |      |
| static | saveToSTLWithFaceColor   | final HE_Mesh mesh,final HET_WriterSTL stl                                         | void  |      |
| static | saveAsSTLWithFaceColor   | final HE_Mesh mesh,final HET_WriterSTL stl                                         | void  |      |
| static | saveToSimpleMesh         | final HE_Mesh mesh, final String path,final String name                            | void  |      |
| static | saveAsSimpleMesh         | final HE_Mesh mesh, final String path,final String name                            | void  |      |
| static | saveToHemesh             | final HE_Mesh mesh, final String path,final String name                            | void  |      |
| static | saveAsHemesh             | final HE_Mesh mesh, final String path,final String name                            | void  |      |
| static | saveToBinaryHemesh       | final HE_Mesh mesh, final String path,final String name                            | void  |      |
| static | saveAsBinaryHemesh       | final HE_Mesh mesh, final String path,final String name                            | void  |      |
| static | saveToPOV                | final HE_Mesh mesh, final String path,final String name                            | void  |      |
| static | saveAsPOV                | final HE_Mesh mesh, final String path,final String name                            | void  |      |
| static | saveToPOV                | final HE_Mesh mesh, final String path,final String name, final boolean saveNormals | void  |      |
| static | saveAsPOV                | final HE_Mesh mesh, final String path,final String name, final boolean saveNormals | void  |      |
| static | saveToPOV                | final HE_Mesh mesh, final HET_WriterPOV pov,final boolean normals                  | void  |      |
| static | saveAsPOV                | final HE_Mesh mesh, final HET_WriterPOV pov,final boolean normals                  | void  |      |
| static | saveToPOV                | final HE_Mesh mesh, final PrintWriter pw                                           | void  |      |
| static | saveAsPOV                | final HE_Mesh mesh, final PrintWriter pw                                           | void  |      |
| static | saveToPOV                | final HE_Mesh mesh, final PrintWriter pw,final boolean saveNormals                 | void  |      |
| static | saveAsPOV                | final HE_Mesh mesh, final PrintWriter pw,final boolean saveNormals                 | void  |      |
| static | saveToWRLWithFaceColor   | final HE_Mesh mesh,final String path, final String name                            | void  |      |
| static | saveAsWRLWithFaceColor   | final HE_Mesh mesh,final String path, final String name                            | void  |      |
| static | saveToWRLWithVertexColor | final HE_Mesh mesh,final String path, final String name                            | void  |      |
| static | saveAsWRLWithVertexColor | final HE_Mesh mesh,final String path, final String name                            | void  |      |
| static | saveToWRL                | final HE_Mesh mesh, final String path,final String name                            | void  |      |
| static | saveAsWRL                | final HE_Mesh mesh, final String path,final String name                            | void  |      |
| static | saveToPLY                | final HE_Mesh mesh, final String path,final String name                            | void  |      |
| static | saveAsPLY                | final HE_Mesh mesh, final String path,final String name                            | void  |      |
| static | saveToPLYWithVertexColor | final HE_Mesh mesh,final String path, final String name                            | void  |      |
| static | saveAsPLYWithVertexColor | final HE_Mesh mesh,final String path, final String name                            | void  |      |
| static | saveToPLYWithFaceColor   | final HE_Mesh mesh,final String path, final String name                            | void  |      |
| static | saveAsPLYWithFaceColor   | final HE_Mesh mesh,final String path, final String name                            | void  |      |