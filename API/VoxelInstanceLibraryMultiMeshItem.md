---
created: 2023-10-09T22:38:26 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceLibraryMultiMeshItem/
author: 
---

# VoxelInstanceLibraryMultiMeshItem体素实例库多网格项

> ## Excerpt
> 继承：体素实例库项

---
##   
体素实例库多网格项

  
继承：体素实例库项

##  属性：

|  类型 |  名字 |  违约 |
| --- | --- | --- |
| `int` | [cast\_shadow](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceLibraryMultiMeshItem/#i_cast_shadow) | 1 |
| `int` | [collision\_layer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceLibraryMultiMeshItem/#i_collision_layer) | 1 |
| `int` | [collision\_mask](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceLibraryMultiMeshItem/#i_collision_mask) | 1 |
| `Array` | [collision\_shapes](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceLibraryMultiMeshItem/#i_collision_shapes) | \[\] |
| `Material` | [material\_override](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceLibraryMultiMeshItem/#i_material_override) |  |
| `Mesh` |  [网孔](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceLibraryMultiMeshItem/#i_mesh) |  |
| `Mesh` | [mesh\_lod1](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceLibraryMultiMeshItem/#i_mesh_lod1) |  |
| `Mesh` | [mesh\_lod2](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceLibraryMultiMeshItem/#i_mesh_lod2) |  |
| `Mesh` | [mesh\_lod3](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceLibraryMultiMeshItem/#i_mesh_lod3) |  |
| `int` | [render\_layer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceLibraryMultiMeshItem/#i_render_layer) | 1 |
| `PackedScene` |  [现场](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceLibraryMultiMeshItem/#i_scene) |  |

##  方法：

|  返回 |  签名 |
| --- | --- |
|  [字符串名称\[\]](https://docs.godotengine.org/en/stable/classes/class_stringname[].html) |   
get\_collider\_group\_names （ ） 常量 |
|  [网孔](https://docs.godotengine.org/en/stable/classes/class_mesh.html) |   
get\_mesh （ int mesh\_lod\_index ） const |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceLibraryMultiMeshItem/#) |   
set\_collider\_group\_names （ 字符串名称\[\] 名称 ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceLibraryMultiMeshItem/#) |   
set\_mesh （ 网格， int mesh\_lod\_index ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceLibraryMultiMeshItem/#) |   
setup\_from\_template（节点节点） |

##  常量：

-   **MAX\_MESH\_LODS** = **4**

##  属性描述

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **cast\_shadow** = 1
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **collision\_layer** = 1
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **collision\_mask** = 1
    
-   [Array](https://docs.godotengine.org/en/stable/classes/class_array.html) **collision\_shapes** = \[\]
    
-   [Material](https://docs.godotengine.org/en/stable/classes/class_material.html) **material\_override**
    
-    网状网格
    
-   [Mesh](https://docs.godotengine.org/en/stable/classes/class_mesh.html) **mesh\_lod1**
    
-   [Mesh](https://docs.godotengine.org/en/stable/classes/class_mesh.html) **mesh\_lod2**
    
-   [Mesh](https://docs.godotengine.org/en/stable/classes/class_mesh.html) **mesh\_lod3**
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **render\_layer** = 1
    
-    拥挤的场景场景
    

##  方法说明

-     
    字符串名称\[\]get\_collider\_group\_names（ ）

  
获取添加到碰撞器节点的组名的列表。

-     
    Meshget\_mesh（ 国际 mesh\_lod\_index ）
    
-     
    voidset\_collider\_group\_names（ 字符串名称\[\] 名称 ）
    

  
设置将添加到为每个实例生成的碰撞器节点的组名列表。

-     
    voidset\_mesh（ 网格，int mesh\_lod\_index ）
    
-     
    voidsetup\_from\_template（ 节点 ）
    

_  
生成于 Oct 02， 2023_
