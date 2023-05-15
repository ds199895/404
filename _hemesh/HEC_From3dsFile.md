---
navs: []
tags: [He_creators,io]
image:
title: HEC_From3dsFile
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
  var referrer ='HEC_From3dsFile';
  localStorage.setItem('referrer', referrer);
}
</script>

<br>

### HEC_From3dsFile

<br>
#### extends:   [HEC_Creator]({{site.baseurl}}/hemesh/hec-creator)
<br>


- **构造方法**

| 属性   | 方法名             | 参数                | 返回值             | 备注   |
|:-----|:----------------|:------------------|:----------------|:-----|
|      | HEC_From3dsFile | ()                | HEC_From3dsFile |      |
|      | HEC_From3dsFile | final String path | HEC_From3dsFile |      |

- **成员方法**

| 属性   | 方法名        | 参数                | 返回值             | 备注   |
|:-----|:-----------|:------------------|:----------------|:-----|
|      | setPath    | final String path | HEC_From3dsFile |      |
|      | setScale   | final double f    | HEC_From3dsFile |      |
|      | createBase | ()                | HE_Mesh         |      |
|      | loadScene  | final String path | void            |      |

### Mesh3ds

<br>

该类无方法，需自行确认

### TextDecode3ds

<br>


- **成员方法**

| 属性   | 方法名   | 参数   | 返回值    | 备注   |
|:-----|:------|:-----|:-------|:-----|
|      | clear | ()   | void   |      |
|      | text  | ()   | String |      |

### Decode3ds

<br>


- **构造方法**

| 属性   | 方法名       | 参数                                          | 返回值       | 备注   |
|:-----|:----------|:--------------------------------------------|:----------|:-----|
|      | Decode3ds | final TextDecode3ds decode, final int level | Decode3ds |      |

- **成员方法**

| 属性   | 方法名        | 参数                                  | 返回值    | 备注   |
|:-----|:-----------|:------------------------------------|:-------|:-----|
|      | enter      | ()                                  | void   |      |
|      | leave      | ()                                  | void   |      |
|      | println    | final String str                    | void   |      |
|      | printBytes | final byte[] buf, int offset, int n | void   |      |
|      | intToHex   | final int val, final int digits     | String |      |
|      | printHead  | final int id, final int length      | void   |      |

### ChunkInfo

<br>


- **构造方法**

| 属性   | 方法名       | 参数                                                   | 返回值       | 备注   |
|:-----|:----------|:-----------------------------------------------------|:----------|:-----|
|      | ChunkInfo | final boolean known, final int id, final String name | ChunkInfo |      |

### Exception3ds

<br>
#### extends:  java.lang.Exception
<br>


- **构造方法**

| 属性   | 方法名          | 参数             | 返回值          | 备注   |
|:-----|:-------------|:---------------|:-------------|:-----|
|      | Exception3ds | final String s | Exception3ds |      |

### Scene3ds

<br>


- **构造方法**

| 属性   | 方法名      | 参数                                                                    | 返回值      | 备注   |
|:-----|:---------|:----------------------------------------------------------------------|:---------|:-----|
|      | Scene3ds | final byte[] file_image, final TextDecode3ds decode, final int level  | Scene3ds |      |
|      | Scene3ds | final byte[] file_image                                               | Scene3ds |      |
|      | Scene3ds | final File file, final TextDecode3ds decode, final int level          | Scene3ds |      |
|      | Scene3ds | final File file                                                       | Scene3ds |      |
|      | Scene3ds | final InputStream stream, final TextDecode3ds decode, final int level | Scene3ds |      |
|      | Scene3ds | final InputStream stream                                              | Scene3ds |      |

- **成员方法**

| 属性   | 方法名                    | 参数                                     | 返回值        | 备注   |
|:-----|:-----------------------|:---------------------------------------|:-----------|:-----|
|      | addMesh                | final Mesh3ds m                        | void       |      |
|      | meshes                 | ()                                     | int        |      |
|      | mesh                   | final int i                            | Mesh3ds    |      |
|      | filePos                | ()                                     | int        |      |
|      | readByte               | ()                                     | byte       |      |
|      | readUnsignedShort      | ()                                     | int        |      |
|      | readInt                | ()                                     | int        |      |
|      | readFloat              | ()                                     | float      |      |
|      | skipBytes              | final int n                            | int        |      |
|      | skipChunk              | final int chunk_len                    | void       |      |
|      | read_HEAD              | ()                                     | Head       |      |
|      | read_NAME              | ()                                     | String     |      |
|      | read_NAME              | final int length                       | String     |      |
|      | read3DS                | ()                                     | void       |      |
|      | read_M3DMAGIC          | final int chunk_len                    | void       |      |
|      | read_MDATA             | final int chunk_len                    | void       |      |
|      | readColor              | final int chunk_len                    | void       |      |
|      | readPercentage         | final int chunk_len                    | float      |      |
|      | read_MAT_ENTRY         | final int chunk_len                    | void       |      |
|      | read_NAMED_OBJECT      | final int chunk_len                    | void       |      |
|      | readSpotChunk          | final int chunk_len                    | void       |      |
|      | read_N_LIGHT           | final String name, final int chunk_len | void       |      |
|      | readRGBColor           | ()                                     | void       |      |
|      | readTrueColor          | ()                                     | void       |      |
|      | read_N_CAMERA          | final String name, final int chunk_len | void       |      |
|      | read_CAM_RANGES        | ()                                     | void       |      |
|      | read_N_TRI_OBJECT      | final String name, final int chunk_len | void       |      |
|      | read_POINT_ARRAY       | ()                                     | WB_Point[] |      |
|      | read_TEX_VERTS         | ()                                     | void       |      |
|      | read_MESH_TEXTURE_INFO | final Mesh3ds mes                      | void       |      |
|      | readMatrix             | ()                                     | void       |      |
|      | read_FACE_ARRAY        | final Mesh3ds mes, final int chunk_len | void       |      |
|      | read_MSH_MAT_GROUP     | final Mesh3ds mes                      | void       |      |
|      | read_SMOOTH_GROUP      | final Mesh3ds mes, final int chunk_len | void       |      |
|      | read_KFDATA            | final int chunk_len                    | void       |      |
|      | read_OBJECT_NODE_TAG   | final int chunk_len                    | void       |      |
|      | read_TARGET_NODE_TAG   | final int chunk_len                    | void       |      |
|      | read_CAMERA_NODE_TAG   | final int chunk_len                    | void       |      |
|      | read_NODE_ID           | ()                                     | int        |      |
|      | readTrackHead          | ()                                     | int        |      |
|      | readSplineParams       | ()                                     | void       |      |
|      | readPTrack             | ()                                     | void       |      |
|      | read_POS_TRACK_TAG     | ()                                     | void       |      |
|      | read_ROT_TRACK_TAG     | ()                                     | void       |      |
|      | read_MORPH_TRACK_TAG   | ()                                     | void       |      |
|      | read_HIDE_TRACK_TAG    | ()                                     | void       |      |

### Head

<br>


- **构造方法**

| 属性   | 方法名   | 参数                             | 返回值   | 备注   |
|:-----|:------|:-------------------------------|:------|:-----|
|      | Head  | final int id, final int length | Head  |      |