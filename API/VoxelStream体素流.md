---
created: 2023-09-27T00:01:21 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelStream/
author: 
---

# VoxelStream体素流

> ## Excerpt
> Inherits: Resource 继承：资源

---
Inherits: [Resource](https://docs.godotengine.org/en/stable/classes/class_resource.html) 继承：资源

Implements loading and saving voxel blocks, mainly using files.  
实现加载和保存体素块，主要使用文件。

## Properties: 属性：

| Type 类型 | Name 名字 | Default 违约 |
| --- | --- | --- |
| `bool` | [save\_generator\_output save\_generator\_output](https://voxel-tools.readthedocs.io/en/latest/api/VoxelStream/#i_save_generator_output) | false 假 |

## Methods: 方法：

| Return 返回 | Signature 签名 |
| --- | --- |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) | [emerge\_block](https://voxel-tools.readthedocs.io/en/latest/api/VoxelStream/#i_emerge_block) ( [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) out\_buffer, [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) origin\_in\_voxels, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) lod )  
emerge\_block （ VoxelBuffer out\_buffer， Vector3 origin\_in\_voxels， int lod ） |
| [Vector3 矢量3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) | [get\_block\_size](https://voxel-tools.readthedocs.io/en/latest/api/VoxelStream/#i_get_block_size) ( ) const  
get\_block\_size （ ） 常量 |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) | [get\_used\_channels\_mask](https://voxel-tools.readthedocs.io/en/latest/api/VoxelStream/#i_get_used_channels_mask) ( ) const  
get\_used\_channels\_mask （ ） 常量 |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelStream/#) | [immerge\_block](https://voxel-tools.readthedocs.io/en/latest/api/VoxelStream/#i_immerge_block) ( [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) buffer, [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) origin\_in\_voxels, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) lod )  
immerge\_block （ VoxelBuffer buffer， Vector3 origin\_in\_voxels， int lod ） |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) | [load\_voxel\_block](https://voxel-tools.readthedocs.io/en/latest/api/VoxelStream/#i_load_voxel_block) ( [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) out\_buffer, [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) origin\_in\_voxels, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) lod )  
load\_voxel\_block （ VoxelBuffer out\_buffer， Vector3i origin\_in\_voxels， int lod ） |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelStream/#) | [save\_voxel\_block](https://voxel-tools.readthedocs.io/en/latest/api/VoxelStream/#i_save_voxel_block) ( [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) buffer, [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) origin\_in\_voxels, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) lod )  
save\_voxel\_block （ VoxelBuffer buffer， Vector3i origin\_in\_voxels， int lod ） |

## Enumerations: 枚举：

enum **ResultCode**:  枚举结果代码：

-   **RESULT\_ERROR** = **0** --- An error occurred when loading the block. The request will be aborted.  
    RESULT\_ERROR = 0 --- 加载块时出错。请求将中止。
-   **RESULT\_BLOCK\_FOUND** = **2** --- The block was found.  
    RESULT\_BLOCK\_FOUND = 2 --- 找到块。
-   **RESULT\_BLOCK\_NOT\_FOUND** = **1** --- The block was not found. The requester may fallback on using the generator, if any.  
    RESULT\_BLOCK\_NOT\_FOUND = 1 --- 未找到块。请求者可以回退使用生成器（如果有）。

## Property Descriptions 属性描述

-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **save\_generator\_output** = false  
    boolsave\_generator\_output = 假

When this is enabled, if a block cannot be found in the stream and it gets generated, then the generated block will immediately be saved into the stream. This can be used if the generator is too expensive to run on the fly (like Minecraft does), but it will require more disk usage (amount of I/Os and space) and eventual network traffic. If this setting is off, only modified blocks will be saved.  
启用此功能后，如果在流中找不到块并生成该块，则生成的块将立即保存到流中。如果生成器太昂贵而无法动态运行（如 Minecraft），则可以使用此功能，但它需要更多的磁盘使用量（I/O 和空间量）和最终的网络流量。如果关闭此设置，则仅保存修改的块。

## Method Descriptions 方法说明

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **emerge\_block**( [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) out\_buffer, [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) origin\_in\_voxels, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) lod )  
    intemerge\_block（ VoxelBuffer out\_buffer， Vector3 origin\_in\_voxels， int lod ）
    
-   [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) **get\_block\_size**( )  
    Vector3get\_block\_size（ ）
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **get\_used\_channels\_mask**( )  
    intget\_used\_channels\_mask（ ）
    
-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelStream/#)
    
    **immerge\_block**( [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) buffer, [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) origin\_in\_voxels, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) lod )  
    voidimmerge\_block（ VoxelBuffer buffer， Vector3 origin\_in\_voxels， int lod ）

`buffer`: Block of voxels to save. It is strongly recommended to not keep a reference to that data afterward, because streams are allowed to cache it, and saved data must represent either snapshots (copies) or last references to the data after the volume they belonged to is destroyed.  
`buffer` ：要保存的体素块。强烈建议之后不要保留对该数据的引用，因为允许流缓存它，并且保存的数据必须表示快照（副本）或在其所属卷被销毁后对数据的最后一次引用。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **load\_voxel\_block**( [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) out\_buffer, [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) origin\_in\_voxels, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) lod )  
    intload\_voxel\_block（ VoxelBuffer out\_buffer， Vector3i origin\_in\_voxels， int lod ）
    
-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelStream/#) **save\_voxel\_block**( [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) buffer, [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) origin\_in\_voxels, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) lod )  
    voidsave\_voxel\_block（ VoxelBuffer buffer， Vector3i origin\_in\_voxels， int lod ）
    

_Generated on Sep 12, 2023  
生成于 Sep 12， 2023_
