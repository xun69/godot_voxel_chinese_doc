---
created: 2023-09-27T00:01:21 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherTransvoxel/
author: 
---

# VoxelMesherTransvoxel体素网格传输体素

> ## Excerpt
> Inherits: VoxelMesher 继承：体素梅舍

---
Inherits: [VoxelMesher](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesher/) 继承：体素梅舍

Implements isosurface generation (smooth voxels) using the [Transvoxel](https://transvoxel.org/) algorithm.  
使用Transvoxel算法实现等值面生成（平滑体素）。

## Properties: 属性：

## Methods: 方法：

## Enumerations: 枚举：

enum **TexturingMode**:  枚举纹理模式：

-   **TEXTURES\_NONE** = **0**
-   **TEXTURES\_BLEND\_4\_OVER\_16** = **1**

## Property Descriptions 属性描述

-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **deep\_sampling\_enabled** = false  
    booldeep\_sampling\_enabled = 假
    
-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **mesh\_optimization\_enabled** = false  
    boolmesh\_optimization\_enabled = 假
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **mesh\_optimization\_error\_threshold** = 0.005  
    floatmesh\_optimization\_error\_threshold = 0.005
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **mesh\_optimization\_target\_ratio** = 0.0  
    floatmesh\_optimization\_target\_ratio = 0.0
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **texturing\_mode** = 0 inttexturing\_mode = 0
    
-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **transitions\_enabled** = true  
    booltransitions\_enabled = 真
    

## Method Descriptions 方法说明

-   [ArrayMesh](https://docs.godotengine.org/en/stable/classes/class_arraymesh.html) **build\_transition\_mesh**( [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) voxel\_buffer, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) direction )  
    ArrayMeshbuild\_transition\_mesh（体素缓冲区voxel\_buffer，int方向）

_Generated on Sep 12, 2023  
生成于 Sep 12， 2023_
