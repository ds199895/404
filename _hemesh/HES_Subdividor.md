---
navs: []
tags: [He_subdividors]
image:
title: HES_Subdividor
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
  var referrer ='HES_Subdividor';
  localStorage.setItem('referrer', referrer);
}
</script>

<br>

### HES_Subdividor

<br>
#### extends:   [HE_Machine]({{site.baseurl}}/hemesh/he-machine)
<br>


- **构造方法**

| 属性   | 方法名            | 参数   | 返回值            | 备注   |
|:-----|:---------------|:-----|:---------------|:-----|
|      | HES_Subdividor | ()   | HES_Subdividor |      |

- **成员方法**

| 属性   | 方法名   | 参数                           | 返回值     | 备注   |
|:-----|:------|:-----------------------------|:--------|:-----|
|      | apply | final HE_Mesh mesh           | HE_Mesh |      |
|      | apply | final HE_Selection selection | HE_Mesh |      |