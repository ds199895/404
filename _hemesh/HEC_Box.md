---
navs: []
tags: [He_creators,primitives]
image:
title: HEC_Box
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
            

<br>
<a href="{{site.baseurl}}/display/hemesh" onclick="saveReferrer()">继承关系图谱display</a>
<script>
function saveReferrer() {
  var referrer ='HEC_Box';
  localStorage.setItem('referrer', referrer);
}
</script>

<br>

### HEC_Box

<br>
#### extends:   [HEC_Creator]({{site.baseurl}}/hemesh/hec-creator)
<br>


- **构造方法**

| 属性   | 方法名     | 参数                                                                                                                                   | 返回值     | 备注   |
|:-----|:--------|:-------------------------------------------------------------------------------------------------------------------------------------|:--------|:-----|
|      | HEC_Box | ()                                                                                                                                   | HEC_Box |      |
|      | HEC_Box | final double W, final double H, final double D, final int L, final int M, final int N                                                | HEC_Box |      |
|      | HEC_Box | final double x, final double y, final double z, final double W, final double H, final double D,final int L, final int M, final int N | HEC_Box |      |
|      | HEC_Box | final WB_Coord center, final double W, final double H, final double D, final int L, final int M,final int N                          | HEC_Box |      |

- **成员方法**

| 属性   | 方法名               | 参数                                                                                                              | 返回值     | 备注   |
|:-----|:------------------|:----------------------------------------------------------------------------------------------------------------|:--------|:-----|
|      | setFromAABB       | final WB_AABB AABB, final double padding                                                                        | HEC_Box |      |
|      | setFromAABB       | final WB_AABB AABB                                                                                              | HEC_Box |      |
|      | setFromCorners    | final WB_Coord min, final WB_Coord max                                                                          | HEC_Box |      |
|      | setFromCorners    | final double minx, final double miny, final double minz, final double maxx,final double maxy, final double maxz | HEC_Box |      |
|      | setSegments       | final int L, final int M, final int N                                                                           | HEC_Box |      |
|      | setWidth          | final double W                                                                                                  | HEC_Box |      |
|      | setHeight         | final double H                                                                                                  | HEC_Box |      |
|      | setDepth          | final double D                                                                                                  | HEC_Box |      |
|      | setSize           | final double W, final double H, final double D                                                                  | HEC_Box |      |
|      | setWidthSegments  | final int L                                                                                                     | HEC_Box |      |
|      | setHeightSegments | final int M                                                                                                     | HEC_Box |      |
|      | setDepthSegments  | final int N                                                                                                     | HEC_Box |      |
|      | createBase        | ()                                                                                                              | HE_Mesh |      |