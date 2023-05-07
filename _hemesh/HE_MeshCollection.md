---
navs: []
tags: [He_core]
image:
title: HE_MeshCollection
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
  var referrer ='HE_MeshCollection';
  localStorage.setItem('referrer', referrer);
}
</script>

<br>

### HE_MeshCollection

<br>
#### implements:  Iterable&lt;HE_Mesh&gt;
<br>


- **构造方法**

| 属性   | 方法名               | 参数                              | 返回值               | 备注   |
|:-----|:------------------|:--------------------------------|:------------------|:-----|
|      | HE_MeshCollection | ()                              | HE_MeshCollection |      |
|      | HE_MeshCollection | final HEMC_MultiCreator creator | HE_MeshCollection |      |

- **成员方法**

| 属性   | 方法名               | 参数                                         | 返回值                     | 备注   |
|:-----|:------------------|:-------------------------------------------|:------------------------|:-----|
|      | createThreaded    | final HEMC_MultiCreator creator            | void                    |      |
|      | modify            | final HEM_Modifier modifier                | HE_MeshCollection       |      |
|      | modifyThreaded    | final HEM_Modifier modifier                | HE_MeshCollection       |      |
|      | subdivide         | final HES_Subdividor subdividor            | HE_MeshCollection       |      |
|      | subdivideThreaded | final HES_Subdividor subdividor            | HE_MeshCollection       |      |
|      | simplify          | final HES_Simplifier simplifier            | HE_MeshCollection       |      |
|      | simplifyThreaded  | final HES_Simplifier simplifier            | HE_MeshCollection       |      |
|      | mItr              | ()                                         | HE_MeshIterator         |      |
|      | getMesh           | final int i                                | HE_Mesh                 |      |
|      | toList            | ()                                         | List&lt;HE_Mesh&gt;     |      |
|      | set               | final int i, final HE_Mesh mesh            | HE_Mesh                 |      |
|      | add               | final HE_Mesh mesh                         | boolean                 |      |
|      | addAll            | final Collection<? extends HE_Mesh> meshes | boolean                 |      |
|      | remove            | final HE_Mesh mesh                         | boolean                 |      |
|      | getNumberOfMeshes | ()                                         | int                     |      |
|      | size              | ()                                         | int                     |      |
|      | update            | ()                                         | void                    |      |
|      | isFinished        | ()                                         | boolean                 |      |
|      | iterator          | ()                                         | Iterator&lt;HE_Mesh&gt; |      |

### MultiCreatorThread

<br>
#### implements:  Callable&lt;HE_MeshCollection&gt;
<br>


- **构造方法**

| 属性   | 方法名                | 参数                                                                  | 返回值                | 备注   |
|:-----|:-------------------|:--------------------------------------------------------------------|:-------------------|:-----|
|      | MultiCreatorThread | final HEMC_MultiCreator creator, final HE_MeshCollection collection | MultiCreatorThread |      |

- **成员方法**

| 属性   | 方法名   | 参数   | 返回值               | 备注   |
|:-----|:------|:-----|:------------------|:-----|
|      | call  | ()   | HE_MeshCollection |      |

### MultiModifierThread

<br>
#### implements:  Callable&lt;HE_MeshCollection&gt;
<br>


- **构造方法**

| 属性   | 方法名                 | 参数                                                              | 返回值                 | 备注   |
|:-----|:--------------------|:----------------------------------------------------------------|:--------------------|:-----|
|      | MultiModifierThread | final HEM_Modifier modifier, final HE_MeshCollection collection | MultiModifierThread |      |

- **成员方法**

| 属性   | 方法名   | 参数   | 返回值               | 备注   |
|:-----|:------|:-----|:------------------|:-----|
|      | call  | ()   | HE_MeshCollection |      |

### MultiSubdividorThread

<br>
#### implements:  Callable&lt;HE_MeshCollection&gt;
<br>


- **构造方法**

| 属性   | 方法名                   | 参数                                                                  | 返回值                   | 备注   |
|:-----|:----------------------|:--------------------------------------------------------------------|:----------------------|:-----|
|      | MultiSubdividorThread | final HES_Subdividor subdividor, final HE_MeshCollection collection | MultiSubdividorThread |      |

- **成员方法**

| 属性   | 方法名   | 参数   | 返回值               | 备注   |
|:-----|:------|:-----|:------------------|:-----|
|      | call  | ()   | HE_MeshCollection |      |

### MultiSimplifierThread

<br>
#### implements:  Callable&lt;HE_MeshCollection&gt;
<br>


- **构造方法**

| 属性   | 方法名                   | 参数                                                                  | 返回值                   | 备注   |
|:-----|:----------------------|:--------------------------------------------------------------------|:----------------------|:-----|
|      | MultiSimplifierThread | final HES_Simplifier simplifier, final HE_MeshCollection collection | MultiSimplifierThread |      |

- **成员方法**

| 属性   | 方法名   | 参数   | 返回值               | 备注   |
|:-----|:------|:-----|:------------------|:-----|
|      | call  | ()   | HE_MeshCollection |      |