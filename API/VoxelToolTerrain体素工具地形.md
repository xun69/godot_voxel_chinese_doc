---
created: 2023-09-27T00:01:21 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelToolTerrain/
author: 
---

# VoxelToolTerrain体素工具地形

> ## Excerpt
> Inherits: VoxelTool 继承：体素工具

---
Inherits: [VoxelTool](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/) 继承：体素工具

Implementation of [VoxelTool](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/) specialized for uses on [VoxelTerrain](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTerrain/).  
VoxelTool的实现，专门用于VoxelTerrain。

## Description: 说明：

Functions in this class are specific to [VoxelTerrain](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTerrain/). For generic functions, you may also check [VoxelTool](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/).  
此类中的函数特定于 VoxelTerrain。对于通用函数，您也可以检查VoxelTool。

It's not a class to instantiate alone, you may get it from [VoxelTerrain](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTerrain/) using the `get_voxel_tool()` method.  
它不是一个单独实例化的类，您可以使用该方法 `get_voxel_tool()` 从 VoxelTerrain 获取它。

## Methods: 方法：

| Return 返回 | Signature 签名 |
| --- | --- |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelToolTerrain/#) | [do\_hemisphere](https://voxel-tools.readthedocs.io/en/latest/api/VoxelToolTerrain/#i_do_hemisphere) ( [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) center, [float](https://docs.godotengine.org/en/stable/classes/class_float.html) radius, [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) flat\_direction, [float](https://docs.godotengine.org/en/stable/classes/class_float.html) smoothness=0.0 )  
do\_hemisphere（矢量3中心，浮点半径，矢量3 flat\_direction，浮点平滑度=0.0） |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelToolTerrain/#) | [for\_each\_voxel\_metadata\_in\_area](https://voxel-tools.readthedocs.io/en/latest/api/VoxelToolTerrain/#i_for_each_voxel_metadata_in_area) ( [AABB](https://docs.godotengine.org/en/stable/classes/class_aabb.html) voxel\_area, [Callable](https://docs.godotengine.org/en/stable/classes/class_callable.html) callback )  
for\_each\_voxel\_metadata\_in\_area （ AABB voxel\_area， 可调用回调 ） |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelToolTerrain/#) | [run\_blocky\_random\_tick](https://voxel-tools.readthedocs.io/en/latest/api/VoxelToolTerrain/#i_run_blocky_random_tick) ( [AABB](https://docs.godotengine.org/en/stable/classes/class_aabb.html) area, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) voxel\_count, [Callable](https://docs.godotengine.org/en/stable/classes/class_callable.html) callback, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) batch\_count=16 )  
run\_blocky\_random\_tick （ AABB 区域， int voxel\_count， 可调用回调， int batch\_count=16 ） |

## Method Descriptions 方法说明

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelToolTerrain/#) **do\_hemisphere**( [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) center, [float](https://docs.godotengine.org/en/stable/classes/class_float.html) radius, [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) flat\_direction, [float](https://docs.godotengine.org/en/stable/classes/class_float.html) smoothness=0.0 )  
    voiddo\_hemisphere（矢量3中心，浮点半径，矢量3 flat\_direction，浮点平滑度=0.0）
    
-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelToolTerrain/#) **for\_each\_voxel\_metadata\_in\_area**( [AABB](https://docs.godotengine.org/en/stable/classes/class_aabb.html) voxel\_area, [Callable](https://docs.godotengine.org/en/stable/classes/class_callable.html) callback )  
    voidfor\_each\_voxel\_metadata\_in\_area（ AABB voxel\_area，可回调）
    

Executes a function for each voxel holding metadata in the given area.  
为保存给定区域中元数据的每个体素执行一个函数。

The given callback takes two arguments: voxel position (Vector3i), voxel metadata (Variant).  
给定的回调采用两个参数：体素位置 （Vector3i）、体素元数据 （Variant）。

IMPORTANT: inserting new or removing metadata from inside this function is not allowed.  
重要说明：不允许在此函数中插入新元数据或删除元数据。

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelToolTerrain/#) **run\_blocky\_random\_tick**( [AABB](https://docs.godotengine.org/en/stable/classes/class_aabb.html) area, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) voxel\_count, [Callable](https://docs.godotengine.org/en/stable/classes/class_callable.html) callback, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) batch\_count=16 )  
    voidrun\_blocky\_random\_tick（ AABB 区域， 整数 voxel\_count， 可调用回调， 整数 batch\_count=16 ）

Picks random voxels within the specified area and executes a function on them. This only works for terrains using [VoxelMesherBlocky](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherBlocky/). Only voxels where [Voxel.random\_tickable](https://docs.godotengine.org/en/stable/classes/class_voxel.html#class-voxel-property-random-tickable) is `true` will be picked.  
选取指定区域内的随机体素并对其执行函数。这仅适用于使用VoxelMesherBlocky的地形。只会选取Voxel.random\_tickable所在的 `true` 体素。

The given callback takes two arguments: voxel position (Vector3i), voxel value (int).  
给定的回调有两个参数：体素位置 （Vector3i）、体素值 （int）。

_Generated on Sep 12, 2023  
生成于 Sep 12， 2023_
