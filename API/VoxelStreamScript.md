---
created: 2023-10-09T22:38:26 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelStreamScript/
author: 
---

# VoxelStreamScript体素流脚本

> ## Excerpt
> 继承：体素流

---
-   [](https://voxel-tools.readthedocs.io/en/latest/)
  
脚本 API 体素流脚本

___

##  体素流脚本

 继承：体素流

  
使用脚本定义的自定义流的基类。

##  方法：

|  返回 |  签名 |
| --- | --- |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) |   
\_get\_used\_channels\_mask （ ） 虚拟常量 |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) |   
\_load\_voxel\_block （ VoxelBuffer out\_buffer， Vector3i origin\_in\_voxels， int lod ） virtual |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelStreamScript/#) |   
\_save\_voxel\_block （ VoxelBuffer buffer， Vector3i origin\_in\_voxels， int lod ） virtual |

##  方法说明

-     
    int\_get\_used\_channels\_mask（ ）
    
-     
    int\_load\_voxel\_block（ VoxelBuffer out\_buffer， Vector3i origin\_in\_voxels， int lod ）
    
-     
    void\_save\_voxel\_block（ VoxelBuffer buffer， Vector3i origin\_in\_voxels， int lod ）
    

_  
生成于 Oct 02， 2023_
