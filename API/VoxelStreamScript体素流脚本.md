---
created: 2023-09-27T00:01:21 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelStreamScript/
author: 
---

# VoxelStreamScript体素流脚本

> ## Excerpt
> Inherits: VoxelStream 继承：体素流

---
Inherits: [VoxelStream](https://voxel-tools.readthedocs.io/en/latest/api/VoxelStream/) 继承：体素流

Base class for custom streams defined with a script.  
使用脚本定义的自定义流的基类。

## Methods: 方法：

| Return 返回 | Signature 签名 |
| --- | --- |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) | [\_get\_used\_channels\_mask](https://voxel-tools.readthedocs.io/en/latest/api/VoxelStreamScript/#i__get_used_channels_mask) ( ) virtual const  
\_get\_used\_channels\_mask （ ） 虚拟常量 |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) | [\_load\_voxel\_block](https://voxel-tools.readthedocs.io/en/latest/api/VoxelStreamScript/#i__load_voxel_block) ( [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) out\_buffer, [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) origin\_in\_voxels, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) lod ) virtual  
\_load\_voxel\_block （ VoxelBuffer out\_buffer， Vector3i origin\_in\_voxels， int lod ） virtual |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelStreamScript/#) | [\_save\_voxel\_block](https://voxel-tools.readthedocs.io/en/latest/api/VoxelStreamScript/#i__save_voxel_block) ( [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) buffer, [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) origin\_in\_voxels, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) lod ) virtual  
\_save\_voxel\_block （ VoxelBuffer buffer， Vector3i origin\_in\_voxels， int lod ） virtual |

## Method Descriptions 方法说明

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **\_get\_used\_channels\_mask**( )  
    int\_get\_used\_channels\_mask（ ）
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **\_load\_voxel\_block**( [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) out\_buffer, [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) origin\_in\_voxels, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) lod )  
    int\_load\_voxel\_block（ VoxelBuffer out\_buffer， Vector3i origin\_in\_voxels， int lod ）
    
-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelStreamScript/#) **\_save\_voxel\_block**( [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) buffer, [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) origin\_in\_voxels, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) lod )  
    void\_save\_voxel\_block（ VoxelBuffer buffer， Vector3i origin\_in\_voxels， int lod ）
    

_Generated on Sep 12, 2023  
生成于 Sep 12， 2023_
