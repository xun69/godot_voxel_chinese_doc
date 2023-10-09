---
created: 2023-10-09T22:38:26 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherDMC/
author: 
---

# VoxelMesherDMC体素网格器DMC

> ## Excerpt
> 继承：体素梅舍

---
 继承：体素梅舍

  
使用双行进立方体实现等值面生成（平滑体素）。

##  属性：

|  类型 |  名字 |  违约 |
| --- | --- | --- |
| `int` | [geometric\_error](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherDMC/#i_geometric_error) | 0 |
| `int` | [mesh\_mode](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherDMC/#i_mesh_mode) | 0 |
| `int` | [seam\_mode](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherDMC/#i_seam_mode) | 0 |
| `int` | [simplify\_mode](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherDMC/#i_simplify_mode) | 0 |

##  方法：

|  返回 |  签名 |
| --- | --- |
|  [浮](https://docs.godotengine.org/en/stable/classes/class_float.html) |   
get\_geometric\_error （ ） 常量 |
|  [字典](https://docs.godotengine.org/en/stable/classes/class_dictionary.html) |   
get\_statistics （ ） 常量 |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherDMC/#) |   
set\_geometric\_error （ 浮点错误 ） |

##  枚举：

 枚举网格模式：

-   **MESH\_NORMAL** = **0**
-   **MESH\_WIREFRAME** = **1**
-   **MESH\_DEBUG\_OCTREE** = **2**
-   **MESH\_DEBUG\_DUAL\_GRID** = **3**

 枚举简化模式：

-   **SIMPLIFY\_OCTREE\_BOTTOM\_UP** = **0**
-   **SIMPLIFY\_OCTREE\_TOP\_DOWN** = **1**
-   **SIMPLIFY\_NONE** = **2**

 枚举接缝模式：

-   **SEAM\_NONE** = **0**
-   **SEAM\_MARCHING\_SQUARE\_SKIRTS** = **1**

##  属性描述

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **geometric\_error** = 0
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **mesh\_mode** = 0
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **seam\_mode** = 0
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **simplify\_mode** = 0
    

##  方法说明

-     
    floatget\_geometric\_error（ ）
    
-     
    Dictionaryget\_statistics（ ）
    
-     
    voidset\_geometric\_error（浮点错误）
    

_  
生成于 Oct 02， 2023_
