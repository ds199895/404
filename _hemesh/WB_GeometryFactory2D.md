---
navs: []
tags: [Geom,factory]
image:
title: WB_GeometryFactory2D
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
            


### WB_GeometryFactory2D

<br>


- **构造方法**

| 属性   | 方法名                  | 参数   | 返回值                  | 备注   |
|:-----|:---------------------|:-----|:---------------------|:-----|
|      | WB_GeometryFactory2D | ()   | WB_GeometryFactory2D |      |

- **成员方法**

| 属性   | 方法名                                     | 参数                                                                                                       | 返回值                    | 备注   |
|:-----|:----------------------------------------|:---------------------------------------------------------------------------------------------------------|:-----------------------|:-----|
|      | WORLD                                   | ()                                                                                                       | WB_CoordinateSystem    |      |
|      | createCSFromOriginAndX2D                | final WB_Coord origin,final WB_Coord X                                                                   | WB_CoordinateSystem    |      |
|      | createCSFromOriginAndX2D                | final WB_Coord origin,final WB_Coord X, final WB_CoordinateSystem parent                                 | WB_CoordinateSystem    |      |
|      | createCSFromOriginAndXY2D               | final WB_Coord origin,final WB_Coord X, final WB_Coord Y                                                 | WB_CoordinateSystem    |      |
|      | createCSFromOriginAndXY2D               | final WB_Coord origin,final WB_Coord X, final WB_Coord Y,final WB_CoordinateSystem parent                | WB_CoordinateSystem    |      |
|      | createTransformedCS                     | ()                                                                                                       | WB_CoordinateSystem    |      |
|      | createTransformedCS                     | ()                                                                                                       | WB_CoordinateSystem    |      |
|      | createPoint2D                           | ()                                                                                                       | WB_Point               |      |
|      | createPoint2D                           | final WB_Coord p                                                                                         | WB_Point               |      |
|      | createPoint2D                           | final double x, final double y                                                                           | WB_Point               |      |
|      | createInterpolatedPoint2D               | final WB_Coord p,final WB_Coord q, final double f                                                        | WB_Point               |      |
|      | createPointFromPolar                    | final double r, final double phi                                                                         | WB_Point               |      |
|      | createPointFromBipolar                  | final double a, final double sigma,final double tau                                                      | WB_Point               |      |
|      | createPointFromParabolic                | final double sigma,final double tau                                                                      | WB_Point               |      |
|      | createPointFromHyperbolic               | final double u, final double v                                                                           | WB_Point               |      |
|      | createPointFromElliptic                 | final double a, final double sigma,final double tau                                                      | WB_Point               |      |
|      | createIncenter2D                        | final WB_Triangle tri                                                                                    | WB_Point               |      |
|      | createClosestPointOnLine2D              | final WB_Coord p,final WB_Line L                                                                         | WB_Point               |      |
|      | createClosestPoint                      | final WB_Line L1,final WB_Line L2                                                                        | List&lt;WB_Point&gt;   |      |
|      | createIntersectionPoints2D              | final WB_Circle C0,final WB_Circle C1                                                                    | List&lt;WB_Point&gt;   |      |
|      | createIntersectionPoints2D              | final WB_Line L,final WB_Circle C                                                                        | List&lt;WB_Point&gt;   |      |
|      | createIntersectionPoint2D               | final WB_Line L1,final WB_Line L2                                                                        | WB_Point               |      |
|      | createMirrorPoint2D                     | final WB_Coord p, final double x0,final double y0, final double x1, final double y1                      | WB_Point               |      |
|      | createMirrorPoint2D                     | final WB_Coord p, final WB_Line L                                                                        | WB_Point               |      |
|      | createPointFromBarycentricCoordinates2D | final double u,final double v, final double w, final WB_Triangle tri                                     | WB_Point               |      |
|      | createInversionPoint2D                  | final WB_Coord p,final WB_Circle inversionCircle                                                         | WB_Point               |      |
|      | createCentroid2D                        | final WB_Triangle tri                                                                                    | WB_Point               |      |
|      | createCircumcenter2D                    | final WB_Triangle tri                                                                                    | WB_Point               |      |
|      | createOrthocenter2D                     | final WB_Triangle tri                                                                                    | WB_Point               |      |
|      | createPointFromTrilinearCoordinates2D   | final double u,final double v, final double w, final WB_Triangle tri                                     | WB_Point               |      |
|      | createMidpoint2D                        | final WB_Coord p, final WB_Coord q                                                                       | WB_Point               |      |
|      | createVector2D                          | ()                                                                                                       | WB_Vector              |      |
|      | createVectorFromTo2D                    | final WB_Coord p, final WB_Coord q                                                                       | WB_Vector              |      |
|      | createVector2D                          | final WB_Coord p                                                                                         | WB_Vector              |      |
|      | createVector2D                          | final double _x, final double _y                                                                         | WB_Vector              |      |
|      | createNormalizedVector2D                | final WB_Coord p                                                                                         | WB_Vector              |      |
|      | createNormalizedVectorFromTo2D          | final WB_Coord p,final WB_Coord q                                                                        | WB_Vector              |      |
|      | createNormalizedVector2D                | final double _x,final double _y                                                                          | WB_Vector              |      |
|      | createNormalizedPerpendicularVector2D   | final double _x,final double _y                                                                          | WB_Vector              |      |
|      | createNormalizedPerpendicularVector2D   | final WB_Coord v                                                                                         | WB_Vector              |      |
|      | createVectorFromPolar                   | final double r, final double phi                                                                         | WB_Vector              |      |
|      | createVectorFromBipolar                 | final double a, final double sigma,final double tau                                                      | WB_Vector              |      |
|      | createVectorFromParabolic               | final double sigma,final double tau                                                                      | WB_Vector              |      |
|      | createVectorFromHyperbolic              | final double u,final double v                                                                            | WB_Vector              |      |
|      | createVectorFromElliptic                | final double a, final double mu,final double nu                                                          | WB_Vector              |      |
|      | createLineThroughPoints2D               | final WB_Coord p1,final WB_Coord p2                                                                      | WB_Line                |      |
|      | createLineThroughPoints2D               | final double x1, final double y1,final double x2, final double y2                                        | WB_Line                |      |
|      | createLineWithDirection2D               | final WB_Coord origin,final WB_Coord direction                                                           | WB_Line                |      |
|      | createLineWithDirection2D               | final double ox, final double oy,final double dx, final double dy                                        | WB_Line                |      |
|      | createParallelLineThroughPoint2D        | final WB_Line L,final WB_Coord p                                                                         | WB_Line                |      |
|      | createPerpendicularLineThroughPoint2D   | final WB_Line L,final WB_Coord p                                                                         | WB_Line                |      |
|      | createParallelLines2D                   | final WB_Line L,final double d                                                                           | List&lt;WB_Line&gt;    |      |
|      | createBisector2D                        | final WB_Coord p, final WB_Coord q                                                                       | WB_Line                |      |
|      | createAngleBisector2D                   | final WB_Line L1,final WB_Line L2                                                                        | List&lt;WB_Line&gt;    |      |
|      | createLineTangentToCircleInPoint        | final WB_Circle C,final WB_Coord p                                                                       | WB_Line                |      |
|      | createLinesTangentToCircleThroughPoint  | ()                                                                                                       | List&lt;WB_Line&gt;    |      |
|      | createLinesTangentTo2Circles            | final WB_Circle C0,final WB_Circle C1                                                                    | List&lt;WB_Line&gt;    |      |
|      | getDirections2D                         | final WB_Coord w, final double a                                                                         | List&lt;WB_Vector&gt;  |      |
|      | createPerpendicularLinesTangentToCircle | ()                                                                                                       | List&lt;WB_Line&gt;    |      |
|      | createRayThroughPoints2D                | final WB_Coord p1,final WB_Coord p2                                                                      | WB_Ray                 |      |
|      | createRayThroughPoints2D                | final double x1, final double y1,final double x2, final double y2                                        | WB_Ray                 |      |
|      | createRayWithDirection2D                | final WB_Coord origin,final WB_Coord direction                                                           | WB_Ray                 |      |
|      | createRayWithDirection2D                | final double ox, final double oy,final double dx, final double dy                                        | WB_Ray                 |      |
|      | createParallelRayThroughPoint2D         | final WB_Line L,final WB_Coord p                                                                         | WB_Ray                 |      |
|      | createSegment2D                         | final WB_Coord p1, final WB_Coord p2                                                                     | WB_Segment             |      |
|      | createSegmentWithLength2D               | final WB_Coord origin,final WB_Coord direction, final double length                                      | WB_Segment             |      |
|      | createSegment2D                         | final double x1, final double y1,final double x2, final double y2                                        | WB_Segment             |      |
|      | createSegmentWithLength2D               | final double ox,final double oy, final double dx, final double dy,final double length                    | WB_Segment             |      |
|      | createPolyLine                          | final WB_Coord[] points                                                                                  | WB_PolyLine            |      |
|      | createPolyLine                          | ()                                                                                                       | WB_PolyLine            |      |
|      | createRing                              | final WB_Coord[] points                                                                                  | WB_Ring                |      |
|      | createRing                              | final List<? extends WB_Coord> points                                                                    | WB_Ring                |      |
|      | createSimplePolygon                     | final WB_CoordCollection points                                                                          | WB_Polygon             |      |
|      | createSimplePolygon                     | final WB_Polygon poly                                                                                    | WB_Polygon             |      |
|      | createSimplePolygon                     | ()                                                                                                       | WB_Polygon             |      |
|      | createSimplePolygon                     | final WB_Triangle triangle                                                                               | WB_Polygon             |      |
|      | createSimplePolygon                     | final WB_Quad quad                                                                                       | WB_Polygon             |      |
|      | createSimplePolygon                     | final WB_Pentagon pentagon                                                                               | WB_Polygon             |      |
|      | createSimplePolygon                     | final WB_Hexagon hexagon                                                                                 | WB_Polygon             |      |
|      | createSimplePolygon                     | final WB_Octagon octagon                                                                                 | WB_Polygon             |      |
|      | createSimplePolygon                     | final List<? extends WB_Coord> tuples,final int[] indices                                                | WB_Polygon             |      |
|      | createPolygonWithHole                   | final WB_Coord[] points,final WB_Coord[] innerpoints                                                     | WB_Polygon             |      |
|      | createPolygonWithHole                   | ()                                                                                                       | WB_Polygon             |      |
|      | createPolygonWithHoles                  | final WB_Coord[] points,final WB_Coord[][] innerpoints                                                   | WB_Polygon             |      |
|      | createPolygonWithHoles                  | ()                                                                                                       | WB_Polygon             |      |
|      | createPolygonConvexHull2D               | final WB_Polygon poly                                                                                    | WB_Polygon             |      |
|      | createConvexPolygonDecomposition2D      | ()                                                                                                       | List&lt;WB_Polygon&gt; |      |
|      | createBufferedPolygons2D                | final WB_Polygon poly,final double d                                                                     | List&lt;WB_Polygon&gt; |      |
|      | createBufferedPolygons2D                | ()                                                                                                       | List&lt;WB_Polygon&gt; |      |
|      | createBufferedPolygons2D                | final WB_Polygon poly,final double d, final int n                                                        | List&lt;WB_Polygon&gt; |      |
|      | createBufferedPolygonsStraight2D        | ()                                                                                                       | List&lt;WB_Polygon&gt; |      |
|      | createBufferedPolygons2D                | ()                                                                                                       | List&lt;WB_Polygon&gt; |      |
|      | createBufferedPolygonsStraight2D        | ()                                                                                                       | List&lt;WB_Polygon&gt; |      |
|      | createBoundaryPolygons2D                | final WB_Polygon poly                                                                                    | List&lt;WB_Polygon&gt; |      |
|      | createBoundaryPolygons2D                | ()                                                                                                       | List&lt;WB_Polygon&gt; |      |
|      | createRibbonPolygons2D                  | final WB_Polygon poly,final double d                                                                     | List&lt;WB_Polygon&gt; |      |
|      | createRibbonPolygons2D                  | ()                                                                                                       | List&lt;WB_Polygon&gt; |      |
|      | createRibbonPolygons2D                  | final WB_Polygon poly,final double o, final double i                                                     | List&lt;WB_Polygon&gt; |      |
|      | createRibbonPolygons2D                  | ()                                                                                                       | List&lt;WB_Polygon&gt; |      |
|      | createSimplifiedPolygon2D               | final WB_Polygon poly,final double tol                                                                   | List&lt;WB_Polygon&gt; |      |
|      | createDensifiedPolygon2D                | final WB_Polygon poly,final double max                                                                   | List&lt;WB_Polygon&gt; |      |
|      | unionPolygons2D                         | final WB_Polygon poly1,final WB_Polygon poly2                                                            | List&lt;WB_Polygon&gt; |      |
|      | unionPolygons2D                         | final WB_Polygon poly1,final Collection<? extends WB_Polygon> poly2                                      | List&lt;WB_Polygon&gt; |      |
|      | unionPolygons2D                         | ()                                                                                                       | List&lt;WB_Polygon&gt; |      |
|      | subtractPolygons2D                      | final WB_Polygon poly1,final WB_Polygon poly2                                                            | List&lt;WB_Polygon&gt; |      |
|      | subtractPolygons2D                      | final WB_Polygon poly1,final Collection<? extends WB_Polygon> poly2                                      | List&lt;WB_Polygon&gt; |      |
|      | subtractPolygons2D                      | ()                                                                                                       | List&lt;WB_Polygon&gt; |      |
|      | subtractPolygons2D                      | ()                                                                                                       | List&lt;WB_Polygon&gt; |      |
|      | intersectPolygons2D                     | final WB_Polygon poly1,final WB_Polygon poly2                                                            | List&lt;WB_Polygon&gt; |      |
|      | intersectPolygons2D                     | final WB_Polygon poly1,final Collection<? extends WB_Polygon> poly2                                      | List&lt;WB_Polygon&gt; |      |
|      | intersectPolygons2D                     | ()                                                                                                       | List&lt;WB_Polygon&gt; |      |
|      | symDifferencePolygons2D                 | final WB_Polygon poly1,final WB_Polygon poly2                                                            | List&lt;WB_Polygon&gt; |      |
|      | symDifferencePolygons2D                 | final WB_Polygon poly1,final Collection<? extends WB_Polygon> poly2                                      | List&lt;WB_Polygon&gt; |      |
|      | symDifferencePolygons2D                 | ()                                                                                                       | List&lt;WB_Polygon&gt; |      |
|      | constrainPolygons2D                     | final WB_Polygon poly,final WB_Polygon container                                                         | List&lt;WB_Polygon&gt; |      |
|      | constrainPolygons2D                     | final WB_Polygon[] polygons,final WB_Polygon container                                                   | List&lt;WB_Polygon&gt; |      |
|      | constrainPolygons2D                     | final List<WB_Polygon> polygons,final WB_Polygon container                                               | List&lt;WB_Polygon&gt; |      |
|      | createTextWithTrueTypeFont              | final String text,final String fontName, final float pointSize                                           | List&lt;WB_Polygon&gt; |      |
|      | createTextWithTrueTypeFont              | final String text,final String fontName, final float pointSize,final double flatness                     | List&lt;WB_Polygon&gt; |      |
|      | createTextWithTrueTypeFont              | final String text,final String fontName, final int style, final float pointSize,final double flatness    | List&lt;WB_Polygon&gt; |      |
|      | createTextWithFont                      | final String text,final String fontName, final float pointSize                                           | List&lt;WB_Polygon&gt; |      |
|      | createTextWithFont                      | final String text,final String fontName, final float pointSize,final double flatness                     | List&lt;WB_Polygon&gt; |      |
|      | createTextWithFont                      | final String text,final String fontName, final int style, final float pointSize,final double flatness    | List&lt;WB_Polygon&gt; |      |
|      | createTextWithOpenTypeFont              | final String text,final String fontName, final float pointSize                                           | List&lt;WB_Polygon&gt; |      |
|      | createTextWithOpenTypeFont              | final String text,final String fontName, final float pointSize,final double flatness                     | List&lt;WB_Polygon&gt; |      |
|      | createTextWithOpenTypeFont              | final String text,final String fontName, final int style, final float pointSize,final double flatness    | List&lt;WB_Polygon&gt; |      |
|      | createTextWithType1Font                 | final String text,final String fontName, final float pointSize                                           | List&lt;WB_Polygon&gt; |      |
|      | createTextWithType1Font                 | final String text,final String fontName, final float pointSize,final double flatness                     | List&lt;WB_Polygon&gt; |      |
|      | createTextWithType1Font                 | final String text,final String fontName, final int style, final float pointSize,final double flatness    | List&lt;WB_Polygon&gt; |      |
|      | createText                              | final String text, final String fontName,final float pointSize                                           | List&lt;WB_Polygon&gt; |      |
|      | createText                              | final String text, final String fontName,final float pointSize, final double flatness                    | List&lt;WB_Polygon&gt; |      |
|      | createText                              | final String text, final String fontName,final int style, final float pointSize, final double flatness   | List&lt;WB_Polygon&gt; |      |
|      | createText                              | final String text, final Font font,final int style, final float pointSize, final double flatness         | List&lt;WB_Polygon&gt; |      |
|      | createText                              | final String text, final Font font,final double flatness                                                 | List&lt;WB_Polygon&gt; |      |
|      | createShape                             | final Shape shape,final double flatness                                                                  | List&lt;WB_Polygon&gt; |      |
|      | createTriangle2D                        | final double p1x, final double p1y,final double p2x, final double p2y, final double p3x,final double p3y | WB_Triangle            |      |
|      | createTriangle2D                        | final WB_Coord p1, final WB_Coord p2,final WB_Coord p3                                                   | WB_Triangle            |      |
|      | createCircleWithDiameter                | final WB_Coord center,final WB_Coord normal, final double diameter                                       | WB_Circle              |      |
|      | createCircleWithRadius                  | final WB_Coord center,final WB_Coord normal, final double radius                                         | WB_Circle              |      |
|      | createCircleWithRadius                  | final WB_Coord center,final double radius                                                                | WB_Circle              |      |
|      | createCircleWithDiameter                | final WB_Coord center,final double diameter                                                              | WB_Circle              |      |
|      | createCircleWithRadius                  | final double x, final double y,final double radius                                                       | WB_Circle              |      |
|      | createCircleWithDiameter                | final double x, final double y,final double diameter                                                     | WB_Circle              |      |
|      | createInversionCircle2D                 | final WB_Circle C,final WB_Circle inversionCircle                                                        | WB_Circle              |      |
|      | createCircumcircle2D                    | final WB_Triangle tri                                                                                    | WB_Circle              |      |
|      | createIncircle2D                        | final WB_Triangle tri                                                                                    | WB_Circle              |      |
|      | createCirclePPP                         | final WB_Coord p0, final WB_Coord p1,final WB_Coord p2                                                   | WB_Circle              |      |
|      | createCirclePPL                         | final WB_Coord p, final WB_Coord q,final WB_Line L                                                       | List&lt;WB_Circle&gt;  |      |
|      | createCirclePLL                         | final WB_Coord p, final WB_Line L1,final WB_Line L2                                                      | List&lt;WB_Circle&gt;  |      |
|      | createCirclePPC                         | final WB_Coord p, final WB_Coord q,final WB_Circle C                                                     | List&lt;WB_Circle&gt;  |      |
|      | createCirclePCC                         | final WB_Coord p, final WB_Circle C1,final WB_Circle C2                                                  | List&lt;WB_Circle&gt;  |      |
|      | createCirclePLC                         | final WB_Coord p, final WB_Line L,final WB_Circle C                                                      | List&lt;WB_Circle&gt;  |      |
|      | createCircleLLL                         | final WB_Line L1, final WB_Line L2,final WB_Line L3                                                      | List&lt;WB_Circle&gt;  |      |
|      | createCircleLLC                         | final WB_Line L1, final WB_Line L2,final WB_Circle C                                                     | List&lt;WB_Circle&gt;  |      |
|      | createCircleLCC                         | final WB_Line L, final WB_Circle C1,final WB_Circle C2                                                   | List&lt;WB_Circle&gt;  |      |
|      | createCircleCCC                         | WB_Circle C1, WB_Circle C2,WB_Circle C3                                                                  | List&lt;WB_Circle&gt;  |      |