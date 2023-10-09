---
created: 2023-10-09T22:38:26 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelNode/
author: 
---

# VoxelNode体素节点

> ## Excerpt
> 继承：节点3D

---
-   [](https://voxel-tools.readthedocs.io/en/latest/)
 脚本 API 体素节点

___

##  体素节点

 继承：节点3D

  
继承者：VoxelLodTerrain，VoxelTerrain

  
体素体积的基类。

##  属性：

|  类型 |  名字 |  违约 |
| --- | --- | --- |
| `int` | [cast\_shadow](https://voxel-tools.readthedocs.io/en/latest/api/VoxelNode/#i_cast_shadow) | 1 |
| `VoxelGenerator` |  [发电机](https://voxel-tools.readthedocs.io/en/latest/api/VoxelNode/#i_generator) |  |
| `int` | [gi\_mode](https://voxel-tools.readthedocs.io/en/latest/api/VoxelNode/#i_gi_mode) | 0 |
| `VoxelMesher` |  [梅舍尔](https://voxel-tools.readthedocs.io/en/latest/api/VoxelNode/#i_mesher) |  |
| `VoxelStream` |  [流](https://voxel-tools.readthedocs.io/en/latest/api/VoxelNode/#i_stream) |  |

##  枚举：

 枚举 GIMode：

-   **GI\_MODE\_DISABLED** = **0**
-   **GI\_MODE\_BAKED** = **1**
-   **GI\_MODE\_DYNAMIC** = **2**

##  属性描述

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **cast\_shadow** = 1
    
-    体素生成器
    

  
过程生成器，用于在流中不存在时加载体素块。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **gi\_mode** = 0
    
-    体素网格器网格器
    

  
定义如何将体素转换为可见网格。

-    体素流流

  
持久体素数据的主要来源。如果未分配，则整个卷将使用生成器。

_  
生成于 Oct 02， 2023_
