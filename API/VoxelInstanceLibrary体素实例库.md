---
created: 2023-09-27T00:01:21 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceLibrary/
author: 
---

# VoxelInstanceLibrary体素实例库

> ## Excerpt
> Inherits: Resource 继承：资源

---
Inherits: [Resource](https://docs.godotengine.org/en/stable/classes/class_resource.html) 继承：资源

Contains a list of models that can be used by [VoxelInstancer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstancer/), associated with a unique ID.  
包含可由 VoxelInstancer 使用的模型列表，这些模型与唯一 ID 相关联。

## Methods: 方法：

## Constants: 常量：

-   **MAX\_ID** = **65535**

## Method Descriptions 方法说明

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceLibrary/#) **add\_item**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) id, [VoxelInstanceLibraryItem](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceLibraryItem/) item )  
    voidadd\_item（ int id， VoxelInstanceLibraryItem item ）
    
-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceLibrary/#) **clear**( )  空清（ ）
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html)
    
    **find\_item\_by\_name**( [String](https://docs.godotengine.org/en/stable/classes/class_string.html) name )  
    intfind\_item\_by\_name（ 字符串名称 ）
-   [PackedInt32Array](https://docs.godotengine.org/en/stable/classes/class_packedint32array.html) **get\_all\_item\_ids**( )  
    PackedInt32Arrayget\_all\_item\_ids（ ）
    
-   [VoxelInstanceLibraryItem](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceLibraryItem/) **get\_item**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) id )  
    VoxelInstanceLibraryItemget\_item（ 整数 ID ）
    
-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceLibrary/#) **remove\_item**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) id )  
    voidremove\_item（ 整数 ID ）
    

_Generated on Sep 12, 2023  
生成于 Sep 12， 2023_
