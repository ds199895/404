---
navs: []
tags: [He_core]
image:
title: HE_FaceHalfedgeInnerCirculator
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
  var referrer ='HE_FaceHalfedgeInnerCirculator';
  localStorage.setItem('referrer', referrer);
}
</script>

<br>

### HE_FaceHalfedgeInnerCirculator

<br>
#### implements:  Iterator&lt;HE_Halfedge&gt;
<br>


- **构造方法**

| 属性   | 方法名                            | 参数              | 返回值                            | 备注   |
|:-----|:-------------------------------|:----------------|:-------------------------------|:-----|
|      | HE_FaceHalfedgeInnerCirculator | final HE_Face f | HE_FaceHalfedgeInnerCirculator |      |

- **成员方法**

| 属性   | 方法名     | 参数   | 返回值         | 备注   |
|:-----|:--------|:-----|:------------|:-----|
|      | hasNext | ()   | boolean     |      |
|      | next    | ()   | HE_Halfedge |      |
|      | remove  | ()   | void        |      |