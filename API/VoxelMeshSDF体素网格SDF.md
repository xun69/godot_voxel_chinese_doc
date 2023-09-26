---
created: 2023-09-27T00:01:21 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelMeshSDF/
author: 
---

# VoxelMeshSDF体素网格SDF

> ## Excerpt
> Inherits: Resource 继承：资源

---
Inherits: [Resource](https://docs.godotengine.org/en/stable/classes/class_resource.html) 继承：资源

## Properties: 属性：

| Type 类型 | Name 名字 | Default 违约 |
| --- | --- | --- |
| `Dictionary` | [\_data \_数据](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMeshSDF/#i__data) | {} |
| `int` | [bake\_mode bake\_mode](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMeshSDF/#i_bake_mode) | 1 |
| `bool` | [boundary\_sign\_fix\_enabled  
boundary\_sign\_fix\_enabled](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMeshSDF/#i_boundary_sign_fix_enabled) | true 真 |
| `int` | [cell\_count cell\_count](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMeshSDF/#i_cell_count) | 64 |
| `float` | [margin\_ratio margin\_ratio](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMeshSDF/#i_margin_ratio) | 0.25 |
| `Mesh` | [mesh 网孔](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMeshSDF/#i_mesh) |  |
| `int` | [partition\_subdiv partition\_subdiv](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMeshSDF/#i_partition_subdiv) | 32 |

## Methods: 方法：

## Signals: 信号：

-   baked( )  烘烤（ ）

## Enumerations: 枚举：

enum **BakeMode**:  枚举烘焙模式：

-   **BAKE\_MODE\_ACCURATE\_NAIVE** = **0**
-   **BAKE\_MODE\_ACCURATE\_PARTITIONED** = **1**
-   **BAKE\_MODE\_APPROX\_INTERP** = **2**
-   **BAKE\_MODE\_APPROX\_FLOODFILL** = **3**
-   **BAKE\_MODE\_COUNT** = **4**

## Property Descriptions 属性描述

-   [Dictionary](https://docs.godotengine.org/en/stable/classes/class_dictionary.html) **\_data** = {} Dictionary\_data = {}
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **bake\_mode** = 1 intbake\_mode = 1
    
-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **boundary\_sign\_fix\_enabled** = true  
    boolboundary\_sign\_fix\_enabled = 真
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **cell\_count** = 64 intcell\_count = 64
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **margin\_ratio** = 0.25  
    floatmargin\_ratio = 0.25
    
-   [Mesh](https://docs.godotengine.org/en/stable/classes/class_mesh.html) **mesh** 网状网格
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **partition\_subdiv** = 32  
    intpartition\_subdiv = 32
    

## Method Descriptions 方法说明

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMeshSDF/#) **bake**( )  虚空烘焙（ ）
    
-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMeshSDF/#) **bake\_async**( [SceneTree](https://docs.godotengine.org/en/stable/classes/class_scenetree.html) scene\_tree )  
    voidbake\_async（ 场景树 scene\_tree ）
    
-   [Array](https://docs.godotengine.org/en/stable/classes/class_array.html) **debug\_check\_sdf**( [Mesh](https://docs.godotengine.org/en/stable/classes/class_mesh.html) mesh )  
    Arraydebug\_check\_sdf（ 网眼 ）
    
-   [AABB](https://docs.godotengine.org/en/stable/classes/class_aabb.html) **get\_aabb**( )  AABBget\_aabb（ ）
    
-   [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) **get\_voxel\_buffer**( )  
    VoxelBufferget\_voxel\_buffer（ ）
    
-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **is\_baked**( )  boolis\_baked（ ）
    
-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **is\_baking**( )  boolis\_baking（ ）
    

_Generated on Sep 12, 2023  
生成于 Sep 12， 2023_
