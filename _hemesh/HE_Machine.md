---
navs: []
tags: [He_core]
image:
title: HE_Machine
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
            


### HE_Machine

<br>


- **构造方法**

| 属性   | 方法名        | 参数   | 返回值        | 备注   |
|:-----|:-----------|:-----|:-----------|:-----|
|      | HE_Machine | ()   | HE_Machine |      |

- **成员方法**

| 属性   | 方法名             | 参数                         | 返回值             | 备注   |
|:-----|:----------------|:---------------------------|:----------------|:-----|
|      | getName         | ()                         | String          |      |
|      | setName         | final String name          | void            |      |
|      | getParameterSet | ()                         | HE_ParameterSet |      |
|      | setParameterSet | HE_ParameterSet parameters | void            |      |
|      | set             | String name, Object value  | void            |      |
|      | set             | String name, int value     | void            |      |
|      | set             | String name, double value  | void            |      |
|      | get             | String name                | Object          |      |