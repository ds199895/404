---
navs: []
tags: [Math]
image:
title: WB_Peak
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
            


### WB_Peak

<br>


- **构造方法**

| 属性   | 方法名     | 参数             | 返回值     | 备注   |
|:-----|:--------|:---------------|:--------|:-----|
|      | WB_Peak | ()             | WB_Peak |      |
|      | WB_Peak | final double p | WB_Peak |      |

- **成员方法**

| 属性     | 方法名        | 参数             | 返回值     | 备注   |
|:-------|:-----------|:---------------|:--------|:-----|
| static | getPeakAbs | final double p | WB_Peak |      |
| static | getPeakCos | final double p | WB_Peak |      |
| static | getPeakSin | final double p | WB_Peak |      |
| static | getPeakMin | final double p | WB_Peak |      |
| static | getPeakMax | final double p | WB_Peak |      |
|        | setPower   | final double p | void    |      |

### PeakAbs

<br>
#### extends:   [WB_Peak]({{site.baseurl}}/hemesh/wb-peak)
<br>


- **构造方法**

| 属性   | 方法名     | 参数             | 返回值     | 备注   |
|:-----|:--------|:---------------|:--------|:-----|
|      | PeakAbs | final double p | PeakAbs |      |

- **成员方法**

| 属性   | 方法名      | 参数             | 返回值    | 备注   |
|:-----|:---------|:---------------|:-------|:-----|
|      | getValue | final double x | double |      |

### PeakCos

<br>
#### extends:   [WB_Peak]({{site.baseurl}}/hemesh/wb-peak)
<br>


- **构造方法**

| 属性   | 方法名     | 参数             | 返回值     | 备注   |
|:-----|:--------|:---------------|:--------|:-----|
|      | PeakCos | final double p | PeakCos |      |

- **成员方法**

| 属性   | 方法名      | 参数             | 返回值    | 备注   |
|:-----|:---------|:---------------|:-------|:-----|
|      | getValue | final double x | double |      |

### PeakSin

<br>
#### extends:   [WB_Peak]({{site.baseurl}}/hemesh/wb-peak)
<br>


- **构造方法**

| 属性   | 方法名     | 参数             | 返回值     | 备注   |
|:-----|:--------|:---------------|:--------|:-----|
|      | PeakSin | final double p | PeakSin |      |

- **成员方法**

| 属性   | 方法名      | 参数             | 返回值    | 备注   |
|:-----|:---------|:---------------|:-------|:-----|
|      | getValue | final double x | double |      |

### PeakMin

<br>
#### extends:   [WB_Peak]({{site.baseurl}}/hemesh/wb-peak)
<br>


- **构造方法**

| 属性   | 方法名     | 参数             | 返回值     | 备注   |
|:-----|:--------|:---------------|:--------|:-----|
|      | PeakMin | final double p | PeakMin |      |

- **成员方法**

| 属性   | 方法名      | 参数             | 返回值    | 备注   |
|:-----|:---------|:---------------|:-------|:-----|
|      | getValue | final double x | double |      |

### PeakMax

<br>
#### extends:   [WB_Peak]({{site.baseurl}}/hemesh/wb-peak)
<br>


- **构造方法**

| 属性   | 方法名     | 参数             | 返回值     | 备注   |
|:-----|:--------|:---------------|:--------|:-----|
|      | PeakMax | final double p | PeakMax |      |

- **成员方法**

| 属性   | 方法名      | 参数             | 返回值    | 备注   |
|:-----|:---------|:---------------|:-------|:-----|
|      | getValue | final double x | double |      |