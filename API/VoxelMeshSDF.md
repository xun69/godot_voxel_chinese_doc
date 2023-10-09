---
created: 2023-10-09T22:38:26 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelMeshSDF/
author: 
---

# VoxelMeshSDF体素网格SDF

> ## Excerpt
> 继承：资源

---
 继承：资源

##  属性：

|  类型 |  名字 |  违约 |
| --- | --- | --- |
| `Dictionary` |  [\_数据](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMeshSDF/#i__data) | {} |
| `int` | [bake\_mode](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMeshSDF/#i_bake_mode) | 1 |
| `bool` | [boundary\_sign\_fix\_enabled](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMeshSDF/#i_boundary_sign_fix_enabled) |  真 |
| `int` | [cell\_count](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMeshSDF/#i_cell_count) | 64 |
| `float` | [margin\_ratio](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMeshSDF/#i_margin_ratio) | 0.25 |
| `Mesh` |  [网孔](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMeshSDF/#i_mesh) |  |
| `int` | [partition\_subdiv](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMeshSDF/#i_partition_subdiv) | 32 |

##  方法：

|  返回 |  签名 |
| --- | --- |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMeshSDF/#) |  烘烤 （ ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMeshSDF/#) |   
bake\_async （ 场景树 scene\_tree ） |
|  [数组](https://docs.godotengine.org/en/stable/classes/class_array.html) |   
debug\_check\_sdf（网眼） |
|  [阿布](https://docs.godotengine.org/en/stable/classes/class_aabb.html) |   
get\_aabb （ ） 常量 |
|  [体素缓冲器](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) |   
get\_voxel\_buffer （ ） 常量 |
|  [布尔](https://docs.godotengine.org/en/stable/classes/class_bool.html) |   
is\_baked （ ） 常量 |
|  [布尔](https://docs.godotengine.org/en/stable/classes/class_bool.html) |   
is\_baking （ ） 常量 |

##  信号：

-    烘烤（ ）

##  枚举：

 枚举烘焙模式：

-   **BAKE\_MODE\_ACCURATE\_NAIVE** = **0**
-   **BAKE\_MODE\_ACCURATE\_PARTITIONED** = **1**
-   **BAKE\_MODE\_APPROX\_INTERP** = **2**
-   **BAKE\_MODE\_APPROX\_FLOODFILL** = **3**
-   **BAKE\_MODE\_COUNT** = **4**

##  属性描述

-   [Dictionary](https://docs.godotengine.org/en/stable/classes/class_dictionary.html) **\_data** = {}
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **bake\_mode** = 1
    
-     
    boolboundary\_sign\_fix\_enabled = 真
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **cell\_count** = 64
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **margin\_ratio** = 0.25
    
-    网状网格
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **partition\_subdiv** = 32
    

##  方法说明

-    虚空烘焙（ ）
    
-     
    voidbake\_async（ 场景树 scene\_tree ）
    
-     
    Arraydebug\_check\_sdf（ 网眼 ）
    
-    AABBget\_aabb（ ）
    
-     
    VoxelBufferget\_voxel\_buffer（ ）
    
-    boolis\_baked（ ）
    
-    boolis\_baking（ ）
    

_  
生成于 Oct 02， 2023_
