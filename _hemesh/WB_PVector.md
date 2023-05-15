---
navs: []
tags: [Processing]
image:
title: WB_PVector
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
  var referrer ='WB_PVector';
  localStorage.setItem('referrer', referrer);
}
</script>

<br>

### WB_PVector

<br>
#### extends:   [PVector]({{site.baseurl}}/hemesh/pvector)
<br>
#### implements:   [WB_MutableCoord]({{site.baseurl}}/hemesh/wb-mutablecoord)
<br>


- **成员方法**

| 属性   | 方法名       | 参数                                                             | 返回值     | 备注   |
|:-----|:----------|:---------------------------------------------------------------|:--------|:-----|
|      | xd        | ()                                                             | double  |      |
|      | yd        | ()                                                             | double  |      |
|      | zd        | ()                                                             | double  |      |
|      | wd        | ()                                                             | double  |      |
|      | getd      | final int i                                                    | double  |      |
|      | xf        | ()                                                             | float   |      |
|      | yf        | ()                                                             | float   |      |
|      | zf        | ()                                                             | float   |      |
|      | wf        | ()                                                             | float   |      |
|      | getf      | final int i                                                    | float   |      |
|      | setX      | final double x                                                 | void    |      |
|      | setY      | final double y                                                 | void    |      |
|      | setZ      | final double z                                                 | void    |      |
|      | setW      | final double w                                                 | void    |      |
|      | setCoord  | final int i, final double v                                    | void    |      |
|      | set       | final WB_Coord p                                               | void    |      |
|      | set       | final double x, final double y                                 | void    |      |
|      | set       | final double x, final double y, final double z                 | void    |      |
|      | set       | final double x, final double y, final double z, final double w | void    |      |
|      | compareTo | final WB_Coord p                                               | int     |      |
|      | equals    | final Object o                                                 | boolean |      |
|      | hashCode  | ()                                                             | int     |      |