---
navs: []
tags: [He_modifiers]
image:
title: HEM_Lattice
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
  var referrer ='HEM_Lattice';
  localStorage.setItem('referrer', referrer);
}
</script>

<br>

### HEM_Lattice

<br>
#### extends:   [HEM_Modifier]({{site.baseurl}}/hemesh/hem-modifier)
<br>


- **构造方法**

| 属性   | 方法名         | 参数   | 返回值         | 备注   |
|:-----|:------------|:-----|:------------|:-----|
|      | HEM_Lattice | ()   | HEM_Lattice |      |

- **成员方法**

| 属性   | 方法名               | 参数                                                            | 返回值         | 备注   |
|:-----|:------------------|:--------------------------------------------------------------|:------------|:-----|
|      | setDepth          | final double d                                                | HEM_Lattice |      |
|      | setDepth          | final WB_ScalarParameter d                                    | HEM_Lattice |      |
|      | setWidth          | final double w                                                | HEM_Lattice |      |
|      | setWidth          | final WB_ScalarParameter w                                    | HEM_Lattice |      |
|      | setWidth          | final double w, final double hew                              | HEM_Lattice |      |
|      | setWidth          | final WB_ScalarParameter w,final WB_ScalarParameter hew       | HEM_Lattice |      |
|      | setBulge          | final double d                                                | HEM_Lattice |      |
|      | setBulge          | final WB_ScalarParameter d                                    | HEM_Lattice |      |
|      | setBulge          | final double inner, final double outer                        | HEM_Lattice |      |
|      | setBulge          | final WB_ScalarParameter inner,final WB_ScalarParameter outer | HEM_Lattice |      |
|      | setFuse           | final boolean b                                               | HEM_Lattice |      |
|      | setThresholdAngle | final double a                                                | HEM_Lattice |      |
|      | setFuseAngle      | final double a                                                | HEM_Lattice |      |
|      | applySelf         | final HE_Mesh mesh                                            | HE_Mesh     |      |
|      | applySelf         | final HE_Selection selection                                  | HE_Mesh     |      |