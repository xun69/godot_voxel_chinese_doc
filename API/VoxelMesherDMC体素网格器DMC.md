---
created: 2023-09-27T00:01:21 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherDMC/
author: 
---

# VoxelMesherDMC体素网格器DMC

> ## Excerpt
> Inherits: VoxelMesher 继承：体素梅舍

---
Inherits: [VoxelMesher](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesher/) 继承：体素梅舍

Implements isosurface generation (smooth voxels) using [Dual Marching Cubes](https://www.volume-gfx.com/volume-rendering/dual-marching-cubes/).  
使用双行进立方体实现等值面生成（平滑体素）。

## Properties: 属性：

| Type 类型 | Name 名字 | Default 违约 |
| --- | --- | --- |
| `int` | [geometric\_error geometric\_error](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherDMC/#i_geometric_error) | 0 |
| `int` | [mesh\_mode mesh\_mode](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherDMC/#i_mesh_mode) | 0 |
| `int` | [seam\_mode seam\_mode](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherDMC/#i_seam_mode) | 0 |
| `int` | [simplify\_mode simplify\_mode](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherDMC/#i_simplify_mode) | 0 |

## Methods: 方法：

## Enumerations: 枚举：

enum **MeshMode**:  枚举网格模式：

-   **MESH\_NORMAL** = **0**
-   **MESH\_WIREFRAME** = **1**
-   **MESH\_DEBUG\_OCTREE** = **2**
-   **MESH\_DEBUG\_DUAL\_GRID** = **3**

enum **SimplifyMode**:  枚举简化模式：

-   **SIMPLIFY\_OCTREE\_BOTTOM\_UP** = **0**
-   **SIMPLIFY\_OCTREE\_TOP\_DOWN** = **1**
-   **SIMPLIFY\_NONE** = **2**

enum **SeamMode**:  枚举接缝模式：

-   **SEAM\_NONE** = **0**
-   **SEAM\_MARCHING\_SQUARE\_SKIRTS** = **1**

## Property Descriptions 属性描述

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html)
    
    **geometric\_error** = 0 intgeometric\_error = 0
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **mesh\_mode** = 0 intmesh\_mode = 0
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **seam\_mode** = 0 intseam\_mode = 0
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **simplify\_mode** = 0 intsimplify\_mode = 0
    

## Method Descriptions 方法说明

-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **get\_geometric\_error**( )  
    floatget\_geometric\_error（ ）
    
-   [Dictionary](https://docs.godotengine.org/en/stable/classes/class_dictionary.html) **get\_statistics**( )  
    Dictionaryget\_statistics（ ）
    
-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherDMC/#) **set\_geometric\_error**( [float](https://docs.godotengine.org/en/stable/classes/class_float.html) error )  
    voidset\_geometric\_error（浮点错误）
    

_Generated on Sep 12, 2023  
生成于 Sep 12， 2023_
