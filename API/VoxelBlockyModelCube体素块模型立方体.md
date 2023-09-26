---
created: 2023-09-27T00:01:21 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModelCube/
author: 
---

# VoxelBlockyModelCube体素块模型立方体

> ## Excerpt
> Inherits: VoxelBlockyModel继承：体素块模型

---
Inherits: [VoxelBlockyModel](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModel/)  
继承：体素块模型

Generates a cube model with specific tiles on its sides.  
生成侧面具有特定图块的多维数据集模型。

## Properties: 属性：

| Type 类型 | Name 名字 | Default 违约 |
| --- | --- | --- |
| `Vector2i` | [atlas\_size\_in\_tiles atlas\_size\_in\_tiles](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModelCube/#i_atlas_size_in_tiles) | Vector2i(16, 16) 矢量2i（16， 16） |
| `AABB[]` | [collision\_aabbs collision\_aabbs](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModelCube/#i_collision_aabbs) | \[AABB(0, 0, 0, 1, 1, 1)\]  
\[AABB（0， 0， 0， 1， 1， 1）\] |
| `float` | [height 高度](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModelCube/#i_height) | 1.0 |

## Methods: 方法：

## Property Descriptions 属性描述

-   [Vector2i](https://docs.godotengine.org/en/stable/classes/class_vector2i.html) **atlas\_size\_in\_tiles** = Vector2i(16, 16)  
    Vector2iatlas\_size\_in\_tiles = 向量2i（16， 16）

Sets a reference size of texture atlas, in tiles. It must be set so the model generates correct texture coordinates from specified tile positions.  
设置纹理图集的引用大小（以拼贴为单位）。必须对其进行设置，以便模型从指定的平铺位置生成正确的纹理坐标。

If you are not using an atlas and every side uses the same full texture, use (1,1).  
如果您不使用图集，并且每条面都使用相同的完整纹理，请使用 （1,1）。

-   [AABB\[\]](https://docs.godotengine.org/en/stable/classes/class_aabb[].html) **collision\_aabbs** = \[AABB(0, 0, 0, 1, 1, 1)\]  
    AABB\[\]collision\_aabbs = \[AABB（0， 0， 0， 1， 1， 1）\]
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **height** = 1.0 浮点高度 = 1.0
    

## Method Descriptions 方法说明

-   [Vector2i](https://docs.godotengine.org/en/stable/classes/class_vector2i.html) **get\_tile**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) side )  
    Vector2iget\_tile（ 内侧 ）
    
-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModelCube/#) **set\_tile**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) side, [Vector2i](https://docs.godotengine.org/en/stable/classes/class_vector2i.html) position )  
    voidset\_tile（ int side， Vector2i 位置 ）
    

_Generated on Sep 12, 2023  
生成于 Sep 12， 2023_
