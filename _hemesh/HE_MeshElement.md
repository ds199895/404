---
navs: []
tags: [He_core]
image:
title: HE_MeshElement
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
  var referrer ='HE_MeshElement';
  localStorage.setItem('referrer', referrer);
}
</script>

<br>

### HE_MeshElement

<br>
#### extends:   [HE_Element](/hemesh/he-element)
<br>


- **构造方法**

| 属性   | 方法名            | 参数   | 返回值            | 备注   |
|:-----|:---------------|:-----|:---------------|:-----|
|      | HE_MeshElement | ()   | HE_MeshElement |      |

- **成员方法**

| 属性   | 方法名            | 参数                      | 返回值     | 备注   |
|:-----|:---------------|:------------------------|:--------|:-----|
|      | clearVisited   | ()                      | void    |      |
|      | setVisited     | ()                      | void    |      |
|      | setVisited     | final boolean b         | void    |      |
|      | isVisited      | ()                      | boolean |      |
|      | clearVisible   | ()                      | void    |      |
|      | setVisible     | ()                      | void    |      |
|      | setVisible     | final boolean b         | void    |      |
|      | isVisible      | ()                      | boolean |      |
|      | equals         | final Object other      | boolean |      |
|      | copyProperties | final HE_MeshElement el | void    |      |
|      | getColor       | ()                      | int     |      |
|      | setColor       | final int color         | void    |      |