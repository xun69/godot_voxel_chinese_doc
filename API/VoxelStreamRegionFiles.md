---
created: 2023-10-09T22:38:26 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelStreamRegionFiles/
author: 
---

# VoxelStreamRegionFiles体素流区域文件

> ## Excerpt
> 继承：体素流

---
##  体素流区域文件

 继承：体素流

  
将块加载并保存到按世界位置索引的区域文件中，位于目录下。

##  说明：

  
将块加载并保存到文件系统中，位于按世界位置索引的多个区域文件中，位于目录下。区域将许多块打包在一起，因此可以减少文件切换并提高性能。灵感来自仙女座种子和我的世界。

  
区域文件不是线程安全的。因此，内部互斥通常可能仅限制一个线程的使用。

##  属性：

|  类型 |  名字 |  违约 |
| --- | --- | --- |
| `int` | [block\_size\_po2](https://voxel-tools.readthedocs.io/en/latest/api/VoxelStreamRegionFiles/#i_block_size_po2) | 4 |
| `String` |  [目录](https://voxel-tools.readthedocs.io/en/latest/api/VoxelStreamRegionFiles/#i_directory) | "" |
| `int` | [lod\_count](https://voxel-tools.readthedocs.io/en/latest/api/VoxelStreamRegionFiles/#i_lod_count) | 1 |
| `int` | [region\_size\_po2](https://voxel-tools.readthedocs.io/en/latest/api/VoxelStreamRegionFiles/#i_region_size_po2) | 4 |
| `int` | [sector\_size](https://voxel-tools.readthedocs.io/en/latest/api/VoxelStreamRegionFiles/#i_sector_size) | 512 |

##  方法：

|  返回 |  签名 |
| --- | --- |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelStreamRegionFiles/#) |   
convert\_files （ 字典 new\_settings ） |
|  [矢量3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) |   
get\_region\_size （ ） 常量 |

##  属性描述

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **block\_size\_po2** = 4
    
-    字符串目录 = “”
    

  
保存数据的目录。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **lod\_count** = 1
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **region\_size\_po2** = 4
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **sector\_size** = 512
    

##  方法说明

-     
    voidconvert\_files（ 词典 new\_settings ）
    
-     
    Vector3get\_region\_size（ ）
    

_  
生成于 Oct 02， 2023_
