---
created: 2023-09-27T00:01:21 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceLibraryMultiMeshItem/
author: 
---

# VoxelInstanceLibraryMultiMeshItem体素实例库多网格项

> ## Excerpt
> Inherits: VoxelInstanceLibraryItem继承：体素实例库项

---
Inherits: [VoxelInstanceLibraryItem](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceLibraryItem/)  
继承：体素实例库项

## Properties: 属性：

## Methods: 方法：

## Constants: 常量：

-   **MAX\_MESH\_LODS** = **4**

## Property Descriptions 属性描述

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **cast\_shadow** = 1 intcast\_shadow = 1
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **collision\_layer** = 1 intcollision\_layer = 1
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **collision\_mask** = 1 intcollision\_mask = 1
    
-   [Array](https://docs.godotengine.org/en/stable/classes/class_array.html) **collision\_shapes** = \[\]  
    Arraycollision\_shapes = \[\]
    
-   [Material](https://docs.godotengine.org/en/stable/classes/class_material.html) **material\_override**  
    Materialmaterial\_override
    
-   [Mesh](https://docs.godotengine.org/en/stable/classes/class_mesh.html) **mesh** 网状网格
    
-   [Mesh](https://docs.godotengine.org/en/stable/classes/class_mesh.html) **mesh\_lod1** Meshmesh\_lod1
    
-   [Mesh](https://docs.godotengine.org/en/stable/classes/class_mesh.html) **mesh\_lod2** Meshmesh\_lod2
    
-   [Mesh](https://docs.godotengine.org/en/stable/classes/class_mesh.html) **mesh\_lod3** Meshmesh\_lod3
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **render\_layer** = 1 intrender\_layer = 1
    
-   [PackedScene](https://docs.godotengine.org/en/stable/classes/class_packedscene.html)
    
    **scene** 拥挤的场景场景

## Method Descriptions 方法说明

-   [StringName\[\]](https://docs.godotengine.org/en/stable/classes/class_stringname[].html) **get\_collider\_group\_names**( )  
    字符串名称\[\]get\_collider\_group\_names（ ）

Gets the list of group names that are added to collider nodes.  
获取添加到碰撞器节点的组名的列表。

-   [Mesh](https://docs.godotengine.org/en/stable/classes/class_mesh.html) **get\_mesh**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) mesh\_lod\_index )  
    Meshget\_mesh（ 国际 mesh\_lod\_index ）
    
-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceLibraryMultiMeshItem/#) **set\_collider\_group\_names**( [StringName\[\]](https://docs.godotengine.org/en/stable/classes/class_stringname[].html) names )  
    voidset\_collider\_group\_names（ 字符串名称\[\] 名称 ）
    

Sets the list of group names that will be added to collider nodes generated for each instance.  
设置将添加到为每个实例生成的碰撞器节点的组名列表。

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceLibraryMultiMeshItem/#) **set\_mesh**( [Mesh](https://docs.godotengine.org/en/stable/classes/class_mesh.html) mesh, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) mesh\_lod\_index )  
    voidset\_mesh（ 网格，int mesh\_lod\_index ）
    
-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceLibraryMultiMeshItem/#) **setup\_from\_template**( [Node](https://docs.godotengine.org/en/stable/classes/class_node.html) node )  
    voidsetup\_from\_template（ 节点 ）
    

_Generated on Sep 12, 2023  
生成于 Sep 12， 2023_
