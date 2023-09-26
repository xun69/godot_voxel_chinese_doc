---
created: 2023-09-27T00:01:21 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelDataBlockEnterInfo/
author: 
---

# VoxelDataBlockEnterInfo体素数据块输入信息

> ## Excerpt
> Inherits: Object 继承：对象

---
Inherits: [Object](https://docs.godotengine.org/en/stable/classes/class_object.html) 继承：对象

Information sent by a terrain when one of its data blocks enters the area of a [VoxelViewer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelViewer/).  
当地形的一个数据块进入体素查看器区域时，地形发送的信息。

## Description: 说明：

Information sent by a terrain when one of its data blocks enters the area of a [VoxelViewer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelViewer/). See [VoxelTerrain.\_on\_data\_block\_entered](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTerrain/#i__on_data_block_entered).  
当地形的一个数据块进入体素查看器区域时，地形发送的信息。请参阅VoxelTerrain.\_on\_data\_block\_entered。

Instances of this class must not be stored, as they will become invalid after the call they come from.  
不得存储此类的实例，因为它们在调用后将变得无效。

## Methods: 方法：

## Method Descriptions 方法说明

-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **are\_voxels\_edited**( )  
    boolare\_voxels\_edited（ ）

Tells if voxels in the block have ever been edited. If not, it means the same data can be obtained by running the generator.  
告知块中的体素是否曾经被编辑过。如果不是，则意味着可以通过运行生成器获得相同的数据。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **get\_lod\_index**( )  intget\_lod\_index（ ）

Gets which LOD index the data block is in.  
获取数据块所在的 LOD 索引。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **get\_network\_peer\_id**( )  
    intget\_network\_peer\_id（ ）

Gets the network peer ID of the [VoxelViewer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelViewer/) who caused the block to be referenced.  
获取导致块被引用的体素查看器的网络对等 ID。

-   [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) **get\_position**( )  
    Vector3iget\_position（ ）

Gets the position of the data block, in data block coordinates (voxel coordinates are obtained by multiplying these coordinates with data block size).  
获取数据块在数据块坐标中的位置（体素坐标是通过将这些坐标乘以数据块大小获得的）。

-   [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) **get\_voxels**( )  
    VoxelBufferget\_voxels（ ）

Gets access to the voxels in the block.  
获取对块中体素的访问权限。

_Generated on Sep 12, 2023  
生成于 Sep 12， 2023_
