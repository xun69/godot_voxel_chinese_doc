---
created: 2023-09-27T00:01:21 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyLibraryBase/
author: 
---

# VoxelBlockyLibraryBase体素块库库

> ## Excerpt
> Inherits: Resource 继承：资源

---
Inherits: [Resource](https://docs.godotengine.org/en/stable/classes/class_resource.html) 继承：资源

Contains a list of models that can be used by [VoxelMesherBlocky](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherBlocky/).  
包含可由VoxelMesherBlocky使用的模型列表。

## Description: 说明：

Models used by [VoxelMesherBlocky](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherBlocky/) must be baked before they can be used efficiently at runtime. The way this process happens depends on the implementation of this class. It can be a simple list of models, or a list of high-level types generating variant models. Check child classes for more information.  
VoxelMesherBlocky使用的模型必须先烘焙，然后才能在运行时有效使用。此过程发生的方式取决于此类的实现。它可以是模型的简单列表，也可以是生成变体模型的高级类型的列表。有关详细信息，请查看子类。

## Properties: 属性：

| Type 类型 | Name 名字 | Default 违约 |
| --- | --- | --- |
| `bool` | [bake\_tangents bake\_tangents](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyLibraryBase/#i_bake_tangents) | true 真 |

## Methods: 方法：

## Constants: 常量：

-   **MAX\_MODELS** = **65536**

## Property Descriptions 属性描述

-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **bake\_tangents** = true  
    boolbake\_tangents = 真

Enable this option if you need normal mapping on your voxels. If you don't need it, disabling can reduce memory usage and give a small speed boost.  
如果需要体素上的法线映射，请启用此选项。如果您不需要它，禁用可以减少内存使用量并略微提高速度。

## Method Descriptions 方法说明

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyLibraryBase/#) **bake**( )  虚空烘焙（ ）

Bakes the library. The data of models is optimized in order to combine them more efficiently when generating voxel meshes.  
烘焙库。优化模型数据，以便在生成体素网格时更有效地组合它们。

-   [Material\[\]](https://docs.godotengine.org/en/stable/classes/class_material[].html) **get\_materials**( )  
    材料\[\]get\_materials（ ）

Gets a list of all distinct materials found in all models of the library.  
获取在库的所有模型中找到的所有不同材质的列表。

Note, if at least one non-empty model has no material, there will be one `null` entry in this list to represent "The default material".  
请注意，如果至少一个非空模型没有材质，则此列表中将有一个 `null` 条目表示“默认材质”。

_Generated on Sep 12, 2023  
生成于 Sep 12， 2023_
