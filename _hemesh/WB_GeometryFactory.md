---
navs: []
tags: [Geom,factory]
image:
title: WB_GeometryFactory
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
  var referrer ='WB_GeometryFactory';
  localStorage.setItem('referrer', referrer);
}
</script>

<br>

### WB_GeometryFactory

<br>
#### extends:   [WB_GeometryFactory2D](/hemesh/wb-geometryfactory2d)
<br>


- **构造方法**

| 属性   | 方法名                | 参数   | 返回值                | 备注   |
|:-----|:-------------------|:-----|:-------------------|:-----|
|      | WB_GeometryFactory | ()   | WB_GeometryFactory |      |

- **成员方法**

| 属性     | 方法名                                   | 参数                                                                                                                                                                  | 返回值                    | 备注   |
|:-------|:--------------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-----------------------|:-----|
| static | instance                              | ()                                                                                                                                                                  | WB_GeometryFactory     |      |
|        | origin                                | ()                                                                                                                                                                  | WB_Point               |      |
|        | X                                     | ()                                                                                                                                                                  | WB_Vector              |      |
|        | Y                                     | ()                                                                                                                                                                  | WB_Vector              |      |
|        | Z                                     | ()                                                                                                                                                                  | WB_Vector              |      |
|        | minX                                  | ()                                                                                                                                                                  | WB_Vector              |      |
|        | minY                                  | ()                                                                                                                                                                  | WB_Vector              |      |
|        | minZ                                  | ()                                                                                                                                                                  | WB_Vector              |      |
|        | XY                                    | ()                                                                                                                                                                  | WB_Plane               |      |
|        | YZ                                    | ()                                                                                                                                                                  | WB_Plane               |      |
|        | ZX                                    | ()                                                                                                                                                                  | WB_Plane               |      |
|        | YX                                    | ()                                                                                                                                                                  | WB_Plane               |      |
|        | ZY                                    | ()                                                                                                                                                                  | WB_Plane               |      |
|        | XZ                                    | ()                                                                                                                                                                  | WB_Plane               |      |
|        | createCSFromOriginAndX                | final WB_Coord origin,final WB_Coord X                                                                                                                              | WB_CoordinateSystem    |      |
|        | createCSFromOriginAndX                | final WB_Coord origin,final WB_Coord X, final WB_CoordinateSystem parent                                                                                            | WB_CoordinateSystem    |      |
|        | createCSFromOriginAndXY               | final WB_Coord origin,final WB_Coord X, final WB_Coord Y                                                                                                            | WB_CoordinateSystem    |      |
|        | createCSFromOriginAndXY               | final WB_Coord origin,final WB_Coord X, final WB_Coord Y,final WB_CoordinateSystem parent                                                                           | WB_CoordinateSystem    |      |
|        | createCSFromOriginAndXYZ              | final WB_Coord origin,final WB_Coord X, final WB_Coord Y, final WB_Coord Z,final WB_CoordinateSystem parent                                                         | WB_CoordinateSystem    |      |
|        | createCSFromOriginAndXYZ              | final WB_Coord origin,final WB_Coord X, final WB_Coord Y, final WB_Coord Z                                                                                          | WB_CoordinateSystem    |      |
|        | createEmbeddedPlane                   | ()                                                                                                                                                                  | WB_Map2D               |      |
|        | createEmbeddedPlane                   | final int mode, final double offset                                                                                                                                 | WB_Map2D               |      |
|        | createEmbeddedPlane                   | final int mode                                                                                                                                                      | WB_Map2D               |      |
|        | createEmbeddedPlane                   | final WB_Plane P, final double offset                                                                                                                               | WB_Map2D               |      |
|        | createEmbeddedPlane                   | final WB_Plane P                                                                                                                                                    | WB_Map2D               |      |
|        | createPoint                           | ()                                                                                                                                                                  | WB_Point               |      |
|        | createPoint                           | final WB_Coord p                                                                                                                                                    | WB_Point               |      |
|        | createPoint                           | final double[] p                                                                                                                                                    | WB_Point               |      |
|        | createPoint                           | final double _x, final double _y                                                                                                                                    | WB_Point               |      |
|        | createPoint                           | final double _x, final double _y,final double _z                                                                                                                    | WB_Point               |      |
|        | createInterpolatedPoint               | final WB_Coord p, final WB_Coord q,final double f                                                                                                                   | WB_Point               |      |
|        | createIncenter                        | final WB_Triangle tri                                                                                                                                               | WB_Point               |      |
|        | createOrthocenter                     | final WB_Triangle tri                                                                                                                                               | WB_Point               |      |
|        | createPointFromBarycentricCoordinates | final double u,final double v, final double w, final WB_Triangle tri                                                                                                | WB_Point               |      |
|        | createPointFromCylindrical            | final double r, final double phi,final double z                                                                                                                     | WB_Point               |      |
|        | createPointFromSpherical              | final double r, final double theta,final double phi                                                                                                                 | WB_Point               |      |
|        | createPointFromParaboloidal           | final double sigma,final double tau, final double phi                                                                                                               | WB_Point               |      |
|        | createPointFromParabolic              | final double sigma,final double tau, final double z                                                                                                                 | WB_Point               |      |
|        | createPointFromOblateSpheroidal       | final double a,final double mu, final double nu, final double phi                                                                                                   | WB_Point               |      |
|        | createPointFromProlateSpheroidal      | final double a,final double mu, final double nu, final double phi                                                                                                   | WB_Point               |      |
|        | createPointFromEllipsoidal            | final double a, final double b,final double c, final double lambda, final double mu,final double nu                                                                 | WB_Point               |      |
|        | createPointFromElliptic               | final double a, final double mu,final double nu, final double z                                                                                                     | WB_Point               |      |
|        | createPointFromToroidal               | final double a, final double sigma,final double tau, final double phi                                                                                               | WB_Point               |      |
|        | createPointFromBispherical            | final double a,final double sigma, final double tau, final double phi                                                                                               | WB_Point               |      |
|        | createPointFromBipolarCylindrical     | final double a,final double sigma, final double tau, final double z                                                                                                 | WB_Point               |      |
|        | createPointFromConical                | final double b, final double c,final double r, final double mu, final double nu                                                                                     | WB_Point               |      |
|        | createCentroid                        | final WB_Triangle tri                                                                                                                                               | WB_Point               |      |
|        | createCircumcenter                    | final WB_Triangle tri                                                                                                                                               | WB_Point               |      |
|        | createPointFromTrilinearCoordinates   | final double u,final double v, final double w, final WB_Triangle tri                                                                                                | WB_Point               |      |
|        | createMidpoint                        | final WB_Coord p, final WB_Coord q                                                                                                                                  | WB_Point               |      |
|        | cleanPointlist                        | final List<WB_Point> points                                                                                                                                         | List&lt;WB_Point&gt;   |      |
|        | createVector                          | ()                                                                                                                                                                  | WB_Vector              |      |
|        | createVectorFromTo                    | final WB_Coord p, final WB_Coord q                                                                                                                                  | WB_Vector              |      |
|        | WB_Vector                             | final WB_Coord p                                                                                                                                                    | final                  |      |
|        | createVector                          | final double _x, final double _y                                                                                                                                    | WB_Vector              |      |
|        | createVector                          | final double _x, final double _y,final double _z                                                                                                                    | WB_Vector              |      |
|        | createNormalizedVector                | final WB_Coord p                                                                                                                                                    | WB_Vector              |      |
|        | createNormalizedVectorFromTo          | final WB_Coord p,final WB_Coord q                                                                                                                                   | WB_Vector              |      |
|        | createNormalizedVector                | final double _x, final double _y,final double _z                                                                                                                    | WB_Vector              |      |
|        | createNormalizedVector                | final double _x, final double _y,final double _z, final double _w                                                                                                   | WB_Vector              |      |
|        | createNormalizedVector                | final double _x, final double _y                                                                                                                                    | WB_Vector              |      |
|        | createNormalizedPerpendicularVector   | final double _x,final double _y                                                                                                                                     | WB_Vector              |      |
|        | createNormalizedPerpendicularVector   | final double _x,final double _y, final double _z                                                                                                                    | WB_Vector              |      |
|        | createNormalizedPerpendicularVector   | final WB_Coord p                                                                                                                                                    | WB_Vector              |      |
|        | createVectorFromCylindrical           | final double r,final double phi, final double z                                                                                                                     | WB_Vector              |      |
|        | createVectorFromSpherical             | final double r,final double theta, final double phi                                                                                                                 | WB_Vector              |      |
|        | createVectorFromParaboloidal          | final double sigma,final double tau, final double phi                                                                                                               | WB_Vector              |      |
|        | createVectorFromParabolic             | final double sigma,final double tau, final double z                                                                                                                 | WB_Vector              |      |
|        | createVectorFromOblateSpheroidal      | final double a,final double mu, final double nu, final double phi                                                                                                   | WB_Vector              |      |
|        | createVectorFromProlateSpheroidal     | final double a,final double mu, final double nu, final double phi                                                                                                   | WB_Vector              |      |
|        | createVectorFromEllipsoidal           | final double a, final double b,final double c, final double lambda, final double mu,final double nu                                                                 | WB_Vector              |      |
|        | createVectorFromElliptic              | final double a, final double mu,final double nu, final double z                                                                                                     | WB_Vector              |      |
|        | createVectorFromToroidal              | final double a,final double sigma, final double tau, final double phi                                                                                               | WB_Vector              |      |
|        | createVectorFromBispherical           | final double a,final double sigma, final double tau, final double phi                                                                                               | WB_Vector              |      |
|        | createVectorFromBipolarCylindrical    | final double a,final double sigma, final double tau, final double z                                                                                                 | WB_Vector              |      |
|        | createVectorFromConical               | final double b, final double c,final double r, final double mu, final double nu                                                                                     | WB_Vector              |      |
|        | createLineThroughPoints               | final WB_Coord p1,final WB_Coord p2                                                                                                                                 | WB_Line                |      |
|        | createLineThroughPoints               | final double x1, final double y1,final double x2, final double y2                                                                                                   | WB_Line                |      |
|        | createLineThroughPoints               | final double x1, final double y1,final double z1, final double x2, final double y2,final double z2                                                                  | WB_Line                |      |
|        | createLineWithDirection               | final WB_Coord origin,final WB_Coord direction                                                                                                                      | WB_Line                |      |
|        | createLineWithDirection               | final double ox, final double oy,final double oz, final double dx, final double dy,final double dz                                                                  | WB_Line                |      |
|        | createParallelLineThroughPoint        | final WB_Line L,final WB_Coord p                                                                                                                                    | WB_Line                |      |
|        | createBisector                        | final WB_Coord p, final WB_Coord q                                                                                                                                  | WB_Plane               |      |
|        | createRayThroughPoints                | final WB_Coord p1, final WB_Coord p2                                                                                                                                | WB_Ray                 |      |
|        | createRayThroughPoints                | final double x1, final double y1,final double x2, final double y2                                                                                                   | WB_Ray                 |      |
|        | createRayThroughPoints                | final double x1, final double y1,final double z1, final double x2, final double y2,final double z2                                                                  | WB_Ray                 |      |
|        | createRayWithDirection                | final WB_Coord origin,final WB_Coord direction                                                                                                                      | WB_Ray                 |      |
|        | createRayWithDirection                | final double ox, final double oy,final double oz, final double dx, final double dy,final double dz                                                                  | WB_Ray                 |      |
|        | createParallelRayThroughPoint         | final WB_Line L,final WB_Coord p                                                                                                                                    | WB_Ray                 |      |
|        | createSegment                         | final WB_Coord p1, final WB_Coord p2                                                                                                                                | WB_Segment             |      |
|        | createSegmentWithLength               | final WB_Coord origin,final WB_Coord direction, final double length                                                                                                 | WB_Segment             |      |
|        | createSegment                         | final double x1, final double y1,final double x2, final double y2                                                                                                   | WB_Segment             |      |
|        | createSegmentWithLength               | final double ox, final double oy,final double dx, final double dy, final double length                                                                              | WB_Segment             |      |
|        | createSegment                         | final double x1, final double y1,final double z1, final double x2, final double y2,final double z2                                                                  | WB_Segment             |      |
|        | createSegmentWithLength               | final double ox, final double oy,final double oz, final double dx, final double dy, final double dz,final double length                                             | WB_Segment             |      |
|        | splitSimplePolygon                    | final WB_Polygon poly,final WB_Plane P                                                                                                                              | WB_Polygon[]           |      |
|        | createTriangle                        | final double p1x, final double p1y,final double p1z, final double p2x, final double p2y,final double p2z, final double p3x, final double p3y,final double p3z       | WB_Triangle            |      |
|        | createTriangle                        | final WB_Coord p1, final WB_Coord p2,final WB_Coord p3                                                                                                              | WB_Triangle            |      |
|        | createInversionPoint                  | final WB_Coord p,final WB_Sphere inversionSphere                                                                                                                    | WB_Point               |      |
|        | createInversionCircle                 | final WB_Circle C,final WB_Circle inversionCircle                                                                                                                   | WB_Circle              |      |
|        | createCircumcircle3D                  | final WB_Triangle tri                                                                                                                                               | WB_Circle              |      |
|        | createIncircle                        | final WB_Triangle tri                                                                                                                                               | WB_Circle              |      |
|        | createPlane                           | final WB_Coord origin, final WB_Coord normal                                                                                                                        | WB_Plane               |      |
|        | createPlane                           | final double ox, final double oy,final double oz, final double nx, final double ny,final double nz                                                                  | WB_Plane               |      |
|        | createPlane                           | final WB_Coord p1, final WB_Coord p2,final WB_Coord p3                                                                                                              | WB_Plane               |      |
|        | createPlane                           | final WB_Triangle T                                                                                                                                                 | WB_Plane               |      |
|        | createFlippedPlane                    | final WB_Plane P                                                                                                                                                    | WB_Plane               |      |
|        | createOffsetPlane                     | final WB_Coord origin,final WB_Coord normal, final double offset                                                                                                    | WB_Plane               |      |
|        | createOffsetPlane                     | final double ox, final double oy,final double oz, final double nx, final double ny, final double nz,final double offset                                             | WB_Plane               |      |
|        | createOffsetPlane                     | final WB_Coord p1, final WB_Coord p2,final WB_Coord p3, final double offset                                                                                         | WB_Plane               |      |
|        | createMesh                            | final WB_Coord[] points, final int[][] faces                                                                                                                        | WB_SimpleMesh          |      |
|        | createMesh                            | final Collection<? extends WB_Coord> points,final int[][] faces                                                                                                     | WB_SimpleMesh          |      |
|        | createMesh                            | final WB_AABB aabb                                                                                                                                                  | WB_SimpleMesh          |      |
|        | createUniqueMesh                      | final WB_SimpleMesh mesh                                                                                                                                            | WB_SimpleMesh          |      |
|        | createUniqueMesh                      | final WB_SimpleMesh mesh,final double threshold                                                                                                                     | WB_SimpleMesh          |      |
|        | createRegularPrism                    | final int n, final double radius,final double h                                                                                                                     | WB_SimpleMesh          |      |
|        | createPrism                           | final Collection<? extends WB_Coord> points,final double h                                                                                                          | WB_SimpleMesh          |      |
|        | createPrismOpen                       | final Collection<? extends WB_Coord> points,final double h                                                                                                          | WB_SimpleMesh          |      |
|        | createPrism                           | final WB_Coord[] points, final double h                                                                                                                             | WB_SimpleMesh          |      |
|        | createPrismFaces                      | final int n                                                                                                                                                         | int[][]                |      |
|        | createPrismFacesOpen                  | final int n                                                                                                                                                         | int[][]                |      |
|        | createPrism                           | final WB_Polygon poly, final double h                                                                                                                               | WB_SimpleMesh          |      |
|        | createPrism                           | final WB_Polygon poly, final double h,final double offset                                                                                                           | WB_SimpleMesh          |      |
|        | createMesh                            | final WB_Polygon poly                                                                                                                                               | WB_SimpleMesh          |      |
|        | createMesh                            | final WB_Polygon poly, final double offset                                                                                                                          | WB_SimpleMesh          |      |
|        | createPrismOpen                       | final WB_Polygon poly, final double h                                                                                                                               | WB_SimpleMesh          |      |
|        | createRegularAntiPrism                | final int n, final double radius,final double h                                                                                                                     | WB_SimpleMesh          |      |
|        | createAntiPrism                       | final Collection<? extends WB_Coord> points,final double h                                                                                                          | WB_SimpleMesh          |      |
|        | createAntiPrism                       | final WB_Coord[] points, final double h                                                                                                                             | WB_SimpleMesh          |      |
|        | createAntiprismFaces                  | final int n                                                                                                                                                         | int[][]                |      |
|        | createAntiPrism                       | final WB_Polygon poly, final double h                                                                                                                               | WB_SimpleMesh          |      |
|        | createArchimedes                      | final int type, final double edgeLength                                                                                                                             | WB_SimpleMesh          |      |
|        | createCatalan                         | final int type, final double edgeLength                                                                                                                             | WB_SimpleMesh          |      |
|        | createVerticesFromArray               | final double[][] vertices                                                                                                                                           | List&lt;WB_Point&gt;   |      |
|        | createJohnson                         | final int type, final double edgeLength                                                                                                                             | WB_SimpleMesh          |      |
|        | createOtherPolyhedron                 | final int type,final double edgeLength                                                                                                                              | WB_SimpleMesh          |      |
|        | createPlato                           | final int type, final double edgeLength                                                                                                                             | WB_SimpleMesh          |      |
|        | createPolyhedronFromWRL               | String name, final double radius                                                                                                                                    | WB_SimpleMesh          |      |
|        | createZonohedron                      | final WB_Coord[] vectors,final double scale                                                                                                                         | WB_SimpleMesh          |      |
|        | createStellatedIcosahedron            | final int type,final double radius                                                                                                                                  | WB_SimpleMesh          |      |
|        | createDipyramidWithAngleRange         | ()                                                                                                                                                                  | WB_SimpleMesh          |      |
|        | createDipyramidWithAngleRange         | final WB_Coord[] points,final double minangle, final double maxangle,final WB_Map2D context                                                                         | WB_SimpleMesh          |      |
|        | createDipyramidWithAngle              | ()                                                                                                                                                                  | WB_SimpleMesh          |      |
|        | createDipyramidWithAngle              | final WB_Coord[] points,final double angle, final WB_Map2D context                                                                                                  | WB_SimpleMesh          |      |
|        | createDipyramidWithAngle              | ()                                                                                                                                                                  | WB_SimpleMesh          |      |
|        | createDipyramidWithAngle              | final WB_Coord[] points,final double angle                                                                                                                          | WB_SimpleMesh          |      |
|        | createDipyramidWithHeight             | ()                                                                                                                                                                  | WB_SimpleMesh          |      |
|        | createDipyramidWithHeight             | final WB_Coord[] points,final double height                                                                                                                         | WB_SimpleMesh          |      |
|        | createDipyramidWithHeight             | final WB_Coord[] points,final double height, final WB_Map2D context                                                                                                 | WB_SimpleMesh          |      |
|        | createDipyramidWithHeight             | ()                                                                                                                                                                  | WB_SimpleMesh          |      |
|        | createTaperWithAnglesAndHeight        | ()                                                                                                                                                                  | WB_SimpleMesh          |      |
|        | createTaperWithAnglesAndHeight        | final WB_Coord[] points,final double angles[], final double height, final boolean b,final boolean t, final WB_Map2D context                                         | WB_SimpleMesh          |      |
|        | createTaperWithAngleRangeAndHeight    | ()                                                                                                                                                                  | WB_SimpleMesh          |      |
|        | createTaperWithAngleRangeAndHeight    | final WB_Coord[] points,final double minangle, final double maxangle, final double height,final boolean b, final boolean t, final WB_Map2D context                  | WB_SimpleMesh          |      |
|        | createTaperWithAngleRangeAndHeight    | ()                                                                                                                                                                  | WB_SimpleMesh          |      |
|        | createTaperWithAngleRangeAndHeight    | final WB_Coord[] points,final double minangle, final double maxangle, final double height,final WB_Map2D context                                                    | WB_SimpleMesh          |      |
|        | createTaperWithAngleAndHeight         | ()                                                                                                                                                                  | WB_SimpleMesh          |      |
|        | createTaperWithAngleAndHeight         | final WB_Coord[] points,final double angle, final double height, final WB_Map2D context                                                                             | WB_SimpleMesh          |      |
|        | createTaperWithAngleAndHeight         | ()                                                                                                                                                                  | WB_SimpleMesh          |      |
|        | createTaperWithAngleAndHeight         | final WB_Coord[] points,final double angle, final double height                                                                                                     | WB_SimpleMesh          |      |
|        | createBitaperWithAnglesAndHeight      | ()                                                                                                                                                                  | WB_SimpleMesh          |      |
|        | createBitaperWithAnglesAndHeight      | final WB_Coord[] points,final double[] angles, final double height, final boolean b,final boolean t, final WB_Map2D context                                         | WB_SimpleMesh          |      |
|        | createBitaperWithAngleRangeAndHeight  | ()                                                                                                                                                                  | WB_SimpleMesh          |      |
|        | createBitaperWithAngleRangeAndHeight  | final WB_Coord[] points,final double minangle, final double maxangle, final double height,final boolean b, final boolean t, final WB_Map2D context                  | WB_SimpleMesh          |      |
|        | createBitaperWithAngleRangeAndHeight  | ()                                                                                                                                                                  | WB_SimpleMesh          |      |
|        | createBitaperWithAngleRangeAndHeight  | final WB_Coord[] points,final double minangle, final double maxangle, final double height,final WB_Map2D context                                                    | WB_SimpleMesh          |      |
|        | createBitaperWithAngleRangeAndHeight  | ()                                                                                                                                                                  | WB_SimpleMesh          |      |
|        | createBitaperWithAngleRangeAndHeight  | final WB_Coord[] points,final double minangle, final double maxangle, final double height                                                                           | WB_SimpleMesh          |      |
|        | createBitaperWithAngleAndHeight       | ()                                                                                                                                                                  | WB_SimpleMesh          |      |
|        | createBitaperWithAngleAndHeight       | final WB_Coord[] points,final double angle, final double height, final WB_Map2D context                                                                             | WB_SimpleMesh          |      |
|        | createBitaperWithAngleAndHeight       | ()                                                                                                                                                                  | WB_SimpleMesh          |      |
|        | createBitaperWithAngleAndHeight       | final WB_Coord[] points,final double angle, final double height                                                                                                     | WB_SimpleMesh          |      |
|        | createCapsuleWithAnglesAndHeight      | ()                                                                                                                                                                  | WB_SimpleMesh          |      |
|        | createCapsuleWithAngleRangeAndHeight  | ()                                                                                                                                                                  | WB_SimpleMesh          |      |
|        | createCapsuleWithAngleAndHeight       | ()                                                                                                                                                                  | WB_SimpleMesh          |      |
|        | createCapsuleWithAnglesAndHeight      | ()                                                                                                                                                                  | WB_SimpleMesh          |      |
|        | createCapsuleWithAngleRangeAndHeight  | ()                                                                                                                                                                  | WB_SimpleMesh          |      |
|        | createCapsuleWithAngleAndHeight       | ()                                                                                                                                                                  | WB_SimpleMesh          |      |
|        | createCapsuleWithAnglesAndHeight      | final WB_Coord[] points,final double[] angles, final double height, final double cap,final boolean b, final boolean t, final WB_Map2D context                       | WB_SimpleMesh          |      |
|        | createCapsuleWithAngleRangeAndHeight  | final WB_Coord[] points,final double minangle, final double maxangle, final double height,final double cap, final boolean b, final boolean t,final WB_Map2D context | WB_SimpleMesh          |      |
|        | createCapsuleWithAngleAndHeight       | final WB_Coord[] points,final double angle, final double height, final double cap,final boolean b, final boolean t, final WB_Map2D context                          | WB_SimpleMesh          |      |
|        | createCapsuleWithAnglesAndHeight      | final WB_Coord[] points,final double[] angles, final double height, final double cap                                                                                | WB_SimpleMesh          |      |
|        | createCapsuleWithAngleRangeAndHeight  | final WB_Coord[] points,final double minangle, final double maxangle, final double height,final double cap                                                          | WB_SimpleMesh          |      |
|        | createCapsuleWithAngleAndHeight       | final WB_Coord[] points,final double angle, final double height, final double cap                                                                                   | WB_SimpleMesh          |      |
|        | createSpindleWithAnglesAndHeight      | ()                                                                                                                                                                  | WB_SimpleMesh          |      |
|        | createSpindle                         | final Collection<? extends WB_Coord> points,final double height, final double cap, final WB_Map2D context                                                           | WB_SimpleMesh          |      |
|        | createSpindle                         | final Collection<? extends WB_Coord> points,final double height, final double cap                                                                                   | WB_SimpleMesh          |      |
|        | createSpindleWithAnglesAndHeight      | final WB_Coord[] points,final double[] angles, final double height, final double cap,final WB_Map2D context                                                         | WB_SimpleMesh          |      |
|        | createSpindle                         | final WB_Coord[] points, final double height,final double cap, final WB_Map2D context                                                                               | WB_SimpleMesh          |      |
|        | createSpindle                         | final WB_Coord[] points, final double height,final double cap                                                                                                       | WB_SimpleMesh          |      |
|        | createConvexHull                      | final List<? extends WB_Coord> points                                                                                                                               | WB_SimpleMesh          |      |
|        | createConvexHull                      | final WB_Coord[] points                                                                                                                                             | WB_SimpleMesh          |      |
|        | createConvexHull                      | final WB_Coord[] points,final boolean triangulate                                                                                                                   | WB_SimpleMesh          |      |
|        | createConvexHull                      | final List<? extends WB_Coord> points,final boolean triangulate                                                                                                     | WB_SimpleMesh          |      |
|        | createConvexHullWithThreshold         | final WB_Coord[] points,final boolean triangulate, final double threshold                                                                                           | WB_SimpleMesh          |      |
|        | createConvexHullWithThreshold         | ()                                                                                                                                                                  | WB_SimpleMesh          |      |
|        | createClosestPointOnTriangle          | final WB_Coord p,final WB_Coord a, final WB_Coord b, final WB_Coord c                                                                                               | WB_Point               |      |
|        | createClosestPointOnPolygon           | final WB_Coord p,final WB_Polygon poly                                                                                                                              | WB_Point               |      |
|        | createSphereWithRadius                | final WB_Coord center,final double radius                                                                                                                           | WB_Sphere              |      |
|        | createSphereWithDiameter              | final WB_Coord center,final double diameter                                                                                                                         | WB_Sphere              |      |
|        | createSphereWithRadius                | final double x, final double y,final double z, final double radius                                                                                                  | WB_Sphere              |      |
|        | createSphereWithDiameter              | final double x, final double y,final double z, final double diameter                                                                                                | WB_Sphere              |      |
|        | createTetrahedron                     | final WB_Coord p1,final WB_Coord p2, final WB_Coord p3, final WB_Coord p4                                                                                           | WB_Tetrahedron         |      |
|        | getIntersection                       | final WB_Coord a, final WB_Coord b,final WB_Plane P                                                                                                                 | WB_Point               |      |
|        | createPolygonConvexHull               | final WB_Polygon poly                                                                                                                                               | WB_Polygon             |      |
|        | createBufferedPolygons                | final WB_Polygon poly,final double d                                                                                                                                | List&lt;WB_Polygon&gt; |      |
|        | createBufferedPolygons                | final WB_Polygon poly,final double d, final int n                                                                                                                   | List&lt;WB_Polygon&gt; |      |
|        | createBufferedPolygonsStraight        | ()                                                                                                                                                                  | List&lt;WB_Polygon&gt; |      |
|        | createBufferedPolygons                | ()                                                                                                                                                                  | List&lt;WB_Polygon&gt; |      |
|        | createBufferedPolygons                | ()                                                                                                                                                                  | List&lt;WB_Polygon&gt; |      |
|        | createBufferedPolygonsStraight        | ()                                                                                                                                                                  | List&lt;WB_Polygon&gt; |      |
|        | createBoundaryPolygons                | final WB_Polygon poly                                                                                                                                               | List&lt;WB_Polygon&gt; |      |
|        | createRibbonPolygons                  | final WB_Polygon poly,final double d                                                                                                                                | List&lt;WB_Polygon&gt; |      |
|        | createRibbonPolygons                  | ()                                                                                                                                                                  | List&lt;WB_Polygon&gt; |      |
|        | createRibbonPolygons                  | final WB_Polygon poly,final double o, final double i                                                                                                                | List&lt;WB_Polygon&gt; |      |
|        | createRibbonPolygons                  | ()                                                                                                                                                                  | List&lt;WB_Polygon&gt; |      |
|        | createSimplifiedPolygon               | final WB_Polygon poly,final double tol                                                                                                                              | List&lt;WB_Polygon&gt; |      |
|        | createDensifiedPolygon                | final WB_Polygon poly,final double max                                                                                                                              | List&lt;WB_Polygon&gt; |      |
|        | constrainPolygons                     | final WB_Polygon poly,final WB_Polygon container                                                                                                                    | List&lt;WB_Polygon&gt; |      |
|        | constrainPolygons                     | final WB_Polygon[] polygons,final WB_Polygon container                                                                                                              | List&lt;WB_Polygon&gt; |      |
|        | constrainPolygons                     | final List<WB_Polygon> polygons,final WB_Polygon container                                                                                                          | List&lt;WB_Polygon&gt; |      |
|        | createUniquePoints                    | final List<WB_Coord> points,final double threshold                                                                                                                  | List&lt;WB_Coord&gt;   |      |
|        | createUniquePoints                    | final List<WB_Coord> points                                                                                                                                         | List&lt;WB_Coord&gt;   |      |
|        | createUniquePlanes                    | final List<WB_Plane> planes                                                                                                                                         | List&lt;WB_Plane&gt;   |      |