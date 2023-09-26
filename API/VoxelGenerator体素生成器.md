---
created: 2023-09-27T00:01:21 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelGenerator/
author: 
---

# VoxelGenerator体素生成器

> ## Excerpt
> Inherits: Resource 继承：资源

---
Inherits: [Resource](https://docs.godotengine.org/en/stable/classes/class_resource.html) 继承：资源

Base class to all voxel procedural generators.  
所有体素过程生成器的基类。

## Methods: 方法：

| Return 返回 | Signature 签名 |
| --- | --- |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGenerator/#) | [generate\_block](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGenerator/#i_generate_block) ( [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) out\_buffer, [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) origin\_in\_voxels, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) lod )  
generate\_block （ VoxelBuffer out\_buffer， Vector3 origin\_in\_voxels， int lod ） |

## Method Descriptions 方法说明

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGenerator/#) **generate\_block**( [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) out\_buffer, [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) origin\_in\_voxels, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) lod )  
    voidgenerate\_block（ VoxelBuffer out\_buffer， Vector3 origin\_in\_voxels， int lod ）

Generates a block of voxels within the specified world area.  
在指定的世界区域内生成体素块。

`out_buffer`: Buffer in which voxel data will be generated. It should not be `null` and should have a non-empty size. Do not keep a reference on it after the call. Note: this buffer can have any non-empty size, but some assumptions can be made depending on which terrain node you're using. [VoxelTerrain](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTerrain/) will always request blocks of size 16x16x16, but [VoxelLodTerrain](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/) can request blocks of different sizes.  
`out_buffer` ：将在其中生成体素数据的缓冲区。它不应该并且 `null` 应该具有非空大小。通话后不要保留参考。注意：此缓冲区可以具有任何非空大小，但可以根据您使用的地形节点进行一些假设。VoxelTerrain 将始终请求大小为 16x16x16 的块，但 VoxelLodTerrain 可以请求不同大小的块。

`origin_in_voxels`: Coordinates of the lower corner of the box to generate, relative to LOD0.  
`origin_in_voxels` ：要生成的框下角相对于 LOD0 的坐标。

`lod`: Level of detail index to use for this block. Some generators might not support LOD, in which case it can be left 0. At LOD 0, each cell of the passed buffer spans 1 space unit. At LOD 1, 2 units. At LOD 2, 4 units, and so on.  
`lod` ：用于此块的详细级别索引。某些发生器可能不支持 LOD，在这种情况下，它可以保留为 0。在 LOD 0 处，传递的缓冲区的每个单元格跨越 1 个空间单元。在LOD 1,2个单位。在 LOD 2、4 个单位，依此类推。

_Generated on Sep 12, 2023  
生成于 Sep 12， 2023_
