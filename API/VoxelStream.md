---
created: 2023-10-09T22:38:26 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelStream/
author: 
---

# VoxelStream体素流

> ## Excerpt
> 继承：资源

---
##  体素流

 继承：资源

  
继承者：VoxelStreamRegionFiles， VoxelStreamSQLite， VoxelStreamScript

  
实现加载和保存体素块，主要使用文件。

##  属性：

|  类型 |  名字 |  违约 |
| --- | --- | --- |
| `bool` | [save\_generator\_output](https://voxel-tools.readthedocs.io/en/latest/api/VoxelStream/#i_save_generator_output) |  假 |

##  方法：

|  返回 |  签名 |
| --- | --- |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) |   
emerge\_block （ VoxelBuffer out\_buffer， Vector3 origin\_in\_voxels， int lod ） |
|  [矢量3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) |   
get\_block\_size （ ） 常量 |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) |   
get\_used\_channels\_mask （ ） 常量 |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelStream/#) |   
immerge\_block （ VoxelBuffer buffer， Vector3 origin\_in\_voxels， int lod ） |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) |   
load\_voxel\_block （ VoxelBuffer out\_buffer， Vector3i origin\_in\_voxels， int lod ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelStream/#) |   
save\_voxel\_block （ VoxelBuffer buffer， Vector3i origin\_in\_voxels， int lod ） |

##  枚举：

 枚举结果代码：

-     
    RESULT\_ERROR = 0 --- 加载块时出错。请求将中止。
-     
    RESULT\_BLOCK\_FOUND = 2 --- 找到块。
-     
    RESULT\_BLOCK\_NOT\_FOUND = 1 --- 未找到块。请求者可以回退使用生成器（如果有）。

##  属性描述

-     
    boolsave\_generator\_output = 假

  
启用此功能后，如果在流中找不到块并生成该块，则生成的块将立即保存到流中。如果生成器太昂贵而无法动态运行（如 Minecraft），则可以使用此功能，但它需要更多的磁盘使用量（I/O 和空间量）和最终的网络流量。如果关闭此设置，则仅保存修改的块。

##  方法说明

-     
    intemerge\_block（ VoxelBuffer out\_buffer， Vector3 origin\_in\_voxels， int lod ）
    
-     
    Vector3get\_block\_size（ ）
    
-     
    intget\_used\_channels\_mask（ ）
    
-     
    voidimmerge\_block（ VoxelBuffer buffer， Vector3 origin\_in\_voxels， int lod ）
    

  
`buffer` ：要保存的体素块。强烈建议之后不要保留对该数据的引用，因为允许流缓存它，并且保存的数据必须表示快照（副本）或在其所属卷被销毁后对数据的最后一次引用。

-     
    intload\_voxel\_block（ VoxelBuffer out\_buffer， Vector3i origin\_in\_voxels， int lod ）
    
-     
    voidsave\_voxel\_block（ VoxelBuffer buffer， Vector3i origin\_in\_voxels， int lod ）
    

_  
生成于 Oct 02， 2023_
