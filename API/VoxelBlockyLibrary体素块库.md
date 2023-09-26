---
created: 2023-09-27T00:01:21 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyLibrary/
author: 
---

# VoxelBlockyLibrary体素块库

> ## Excerpt
> Inherits: VoxelBlockyLibraryBase继承：体素块库库

---
Inherits: [VoxelBlockyLibraryBase](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyLibraryBase/)  
继承：体素块库库

Contains a list of models that can be used by [VoxelMesherBlocky](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherBlocky/).  
包含可由VoxelMesherBlocky使用的模型列表。

## Description: 说明：

Provides a list of models that can be used by [VoxelMesherBlocky](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherBlocky/). Each model corresponds to an ID in voxel data, and is generally defined from a mesh. Some extra properties can also be defined, such as how sides get culled by neighbor voxels, or how it is treated by some functionality of the voxel engine.  
提供可由 VoxelMesherBlocky 使用的模型列表。每个模型对应于体素数据中的一个 ID，并且通常从网格定义。还可以定义一些额外的属性，例如相邻体素如何剔除边，或者体素引擎的某些功能如何处理这些属性。

If you create this library from code, it needs to be baked at the end using the [VoxelBlockyLibraryBase.bake](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyLibraryBase/#i_bake) function.  
如果从代码创建此库，则需要在最后使用 VoxelBlockyLibraryBase.bake 函数对其进行烘焙。

The first model (at index 0) is conventionally used for "air" or "empty".  
第一个模型（索引 0）通常用于“空气”或“空”。

## Properties: 属性：

| Type 类型 | Name 名字 | Default 违约 |
| --- | --- | --- |
| `VoxelBlockyModel[]` | [models 模型](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyLibrary/#i_models) | \[\] |

## Methods: 方法：

## Property Descriptions 属性描述

-   [VoxelBlockyModel\[\]](https://docs.godotengine.org/en/stable/classes/class_voxelblockymodel[].html) **models** = \[\]  
    体素块模型\[\]模型 = \[\]

Array of all the models. The index of each model corresponds to the value representing them in voxel data's TYPE channel.  
所有模型的数组。每个模型的索引对应于体素数据的 TYPE 通道中表示它们的值。

## Method Descriptions 方法说明

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **add\_model**( [VoxelBlockyModel](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModel/) \_unnamed\_arg0 )  
    intadd\_model（体素块模型\_unnamed\_arg0）

Adds a model to the library. Returns its index, which will be the value of voxels representing it.  
将模型添加到库中。返回其索引，该索引将是表示它的体素的值。

-   [VoxelBlockyModel](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModel/) **get\_model**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) index )  
    VoxelBlockyModelget\_model（ 整数 ）

Gets a model from its index.  
从模型的索引中获取模型。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **get\_model\_index\_from\_resource\_name**( [String](https://docs.godotengine.org/en/stable/classes/class_string.html) name )  
    intget\_model\_index\_from\_resource\_name（ 字符串名称 ）

Finds the index of the first model having the specified resource name. If not found, returns `null`.  
查找具有指定资源名称的第一个模型的索引。如果未找到，则返回 `null` 。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **get\_voxel\_index\_from\_name**( [String](https://docs.godotengine.org/en/stable/classes/class_string.html) name )  
    intget\_voxel\_index\_from\_name（ 字符串名称 ）

Finds the index of the first model having the specified resource name. If not found, returns `null`.  
查找具有指定资源名称的第一个模型的索引。如果未找到，则返回 `null` 。

_Generated on Sep 12, 2023  
生成于 Sep 12， 2023_
