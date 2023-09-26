---
created: 2023-09-27T00:01:21 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelNode/
author: 
---

# VoxelNode体素节点

> ## Excerpt
> Inherits: Node3D 继承：节点3D

---
Inherits: [Node3D](https://docs.godotengine.org/en/stable/classes/class_node3d.html) 继承：节点3D

Base class for voxel volumes.  
体素体积的基类。

## Properties: 属性：

| Type 类型 | Name 名字 | Default 违约 |
| --- | --- | --- |
| `int` | [cast\_shadow cast\_shadow](https://voxel-tools.readthedocs.io/en/latest/api/VoxelNode/#i_cast_shadow) | 1 |
| `VoxelGenerator` | [generator 发电机](https://voxel-tools.readthedocs.io/en/latest/api/VoxelNode/#i_generator) |  |
| `int` | [gi\_mode gi\_mode](https://voxel-tools.readthedocs.io/en/latest/api/VoxelNode/#i_gi_mode) | 0 |
| `VoxelMesher` | [mesher 梅舍尔](https://voxel-tools.readthedocs.io/en/latest/api/VoxelNode/#i_mesher) |  |
| `VoxelStream` | [stream 流](https://voxel-tools.readthedocs.io/en/latest/api/VoxelNode/#i_stream) |  |

## Enumerations: 枚举：

enum **GIMode**:  枚举 GIMode：

-   **GI\_MODE\_DISABLED** = **0**
-   **GI\_MODE\_BAKED** = **1**
-   **GI\_MODE\_DYNAMIC** = **2**

## Property Descriptions 属性描述

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **cast\_shadow** = 1 intcast\_shadow = 1
    
-   [VoxelGenerator](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGenerator/) **generator** 体素生成器
    

Procedural generator used to load voxel blocks when not present in the stream.  
过程生成器，用于在流中不存在时加载体素块。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **gi\_mode** = 0 intgi\_mode = 0
    
-   [VoxelMesher](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesher/) **mesher** 体素网格器网格器
    

Defines how voxels are transformed into visible meshes.  
定义如何将体素转换为可见网格。

-   [VoxelStream](https://voxel-tools.readthedocs.io/en/latest/api/VoxelStream/) **stream** 体素流流

Primary source of persistent voxel data. If left unassigned, the whole volume will use the generator.  
持久体素数据的主要来源。如果未分配，则整个卷将使用生成器。

_Generated on Sep 12, 2023  
生成于 Sep 12， 2023_
