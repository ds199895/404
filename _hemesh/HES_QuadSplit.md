---
navs: []
tags: [He_subdividors]
image:
title: HES_QuadSplit
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
  var referrer ='HES_QuadSplit';
  localStorage.setItem('referrer', referrer);
}
</script>

<br>

### HES_QuadSplit

<br>
#### extends:   [HES_Subdividor]({{site.baseurl}}/hemesh/hes-subdividor)
<br>


- **构造方法**

| 属性   | 方法名           | 参数   | 返回值           | 备注   |
|:-----|:--------------|:-----|:--------------|:-----|
|      | HES_QuadSplit | ()   | HES_QuadSplit |      |

- **成员方法**

| 属性   | 方法名           | 参数                     | 返回值           | 备注   |
|:-----|:--------------|:-----------------------|:--------------|:-----|
|      | setOffset     | final double d         | HES_QuadSplit |      |
|      | applySelf     | final HE_Mesh mesh     | HE_Mesh       |      |
|      | applySelf     | final HE_Selection sel | HE_Mesh       |      |
|      | getSplitFaces | ()                     | HE_Selection  |      |