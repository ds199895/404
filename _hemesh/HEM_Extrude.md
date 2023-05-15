---
navs: []
tags: [He_modifiers]
image:
title: HEM_Extrude
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
  var referrer ='HEM_Extrude';
  localStorage.setItem('referrer', referrer);
}
</script>

<br>

### HEM_Extrude

<br>
#### extends:   [HEM_Modifier]({{site.baseurl}}/hemesh/hem-modifier)
<br>


- **构造方法**

| 属性   | 方法名         | 参数   | 返回值         | 备注   |
|:-----|:------------|:-----|:------------|:-----|
|      | HEM_Extrude | ()   | HEM_Extrude |      |

- **成员方法**

| 属性   | 方法名                                      | 参数                                                                                                    | 返回值         | 备注   |
|:-----|:-----------------------------------------|:------------------------------------------------------------------------------------------------------|:------------|:-----|
|      | setDistance                              | final double d                                                                                        | HEM_Extrude |      |
|      | setDistance                              | final WB_ScalarParameter d                                                                            | HEM_Extrude |      |
|      | setChamfer                               | final double c                                                                                        | HEM_Extrude |      |
|      | setChamfer                               | final WB_ScalarParameter c                                                                            | HEM_Extrude |      |
|      | setHardEdgeChamfer                       | final double c                                                                                        | HEM_Extrude |      |
|      | setHardEdgeChamfer                       | final WB_ScalarParameter c                                                                            | HEM_Extrude |      |
|      | setRelative                              | final boolean relative                                                                                | HEM_Extrude |      |
|      | setFuse                                  | final boolean b                                                                                       | HEM_Extrude |      |
|      | setPeak                                  | final boolean b                                                                                       | HEM_Extrude |      |
|      | setThresholdAngle                        | final double a                                                                                        | HEM_Extrude |      |
|      | setFuseAngle                             | final double a                                                                                        | HEM_Extrude |      |
|      | setDistances                             | final double[] distances                                                                              | HEM_Extrude |      |
|      | setDistances                             | final float[] distances                                                                               | HEM_Extrude |      |
|      | setDistances                             | final int[] distances                                                                                 | HEM_Extrude |      |
|      | applySelf                                | final HE_Mesh mesh                                                                                    | HE_Mesh     |      |
|      | applySelf                                | final HE_Selection selection                                                                          | HE_Mesh     |      |
|      | applyStraight                            | final HE_Mesh mesh,final List<HE_Face> faces                                                          | HE_Mesh     |      |
|      | applyStraightToOneFaceIgnoreNeighborhood | final int id,final List<HE_Face> selfaces, final HE_Mesh mesh,final boolean[] visited, final double d | boolean     |      |
|      | applyStraightToOneFace                   | final int id,final List<HE_Face> selfaces, final HE_Mesh mesh,final boolean[] visited, final double d | boolean     |      |
|      | applyPeaked                              | final HE_Mesh mesh, final List<HE_Face> faces                                                         | HE_Mesh     |      |
|      | applyPeakToOneFace                       | final int id, final List<HE_Face> selFaces,final HE_Mesh mesh, final double d                         | void        |      |
|      | applyFlat                                | final HE_Mesh mesh, final List<HE_Face> faces,final boolean fuse                                      | HE_Mesh     |      |
|      | applyFlatToOneFace                       | final int id,final List<HE_Face> selFaces, final HE_Mesh mesh,final HE_Selection fuse                 | boolean     |      |