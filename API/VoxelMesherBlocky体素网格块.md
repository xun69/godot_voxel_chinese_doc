---
created: 2023-09-27T00:01:21 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherBlocky/
author: 
---

# VoxelMesherBlocky体素网格块

> ## Excerpt
> Inherits: VoxelMesher 继承：体素梅舍

---
Inherits: [VoxelMesher](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesher/) 继承：体素梅舍

Produces a mesh by batching models corresponding to each voxel value, similar to games like Minecraft or StarMade.  
通过批处理对应于每个体素值的模型来生成网格，类似于 Minecraft 或 StarMade 等游戏。

## Description: 说明：

Occluded faces are removed from the result, and some degree of ambient occlusion can be baked on the edges. Values are expected to be in the [VoxelBuffer.CHANNEL\_TYPE](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#enumerations) channel. Models are defined with a [VoxelBlockyLibrary](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyLibrary/), in which model indices correspond to the voxel values. Models don't have to be cubes.  
从结果中去除遮挡面，并且可以在边缘烘烤一定程度的环境光遮蔽。值应位于VoxelBuffer.CHANNEL\_TYPE通道中。模型是使用体素块库定义的，其中模型索引对应于体素值。模型不必是多维数据集。

## Properties: 属性：

| Type 类型 | Name 名字 | Default 违约 |
| --- | --- | --- |
| `VoxelBlockyLibraryBase` | [library 图书馆](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherBlocky/#i_library) |  |
| `float` | [occlusion\_darkness occlusion\_darkness](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherBlocky/#i_occlusion_darkness) | 0.8 |
| `bool` | [occlusion\_enabled occlusion\_enabled](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherBlocky/#i_occlusion_enabled) | true 真 |

## Property Descriptions 属性描述

-   [VoxelBlockyLibraryBase](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyLibraryBase/) **library**  
    体素块库基库
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **occlusion\_darkness** = 0.8  
    floatocclusion\_darkness = 0.8
    
-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **occlusion\_enabled** = true  
    boolocclusion\_enabled = 真
    

_Generated on Sep 12, 2023  
生成于 Sep 12， 2023_
