---
created: 2023-09-27T00:01:21 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelStreamRegionFiles/
author: 
---

# VoxelStreamRegionFiles体素流区域文件

> ## Excerpt
> Inherits: VoxelStream 继承：体素流

---
Inherits: [VoxelStream](https://voxel-tools.readthedocs.io/en/latest/api/VoxelStream/) 继承：体素流

Loads and saves blocks to region files indexed by world position, under a directory.  
将块加载并保存到按世界位置索引的区域文件中，位于目录下。

## Description: 说明：

Loads and saves blocks to the filesystem, in multiple region files indexed by world position, under a directory. Regions pack many blocks together, so it reduces file switching and improves performance. Inspired by [Seed of Andromeda](https://www.seedofandromeda.com/blogs/1-creating-a-region-file-system-for-a-voxel-game) and Minecraft.  
将块加载并保存到文件系统中，位于按世界位置索引的多个区域文件中，位于目录下。区域将许多块打包在一起，因此可以减少文件切换并提高性能。灵感来自仙女座种子和我的世界。

Region files are not thread-safe. Because of this, internal mutexing may often constrain the use by one thread only.  
区域文件不是线程安全的。因此，内部互斥通常可能仅限制一个线程的使用。

## Properties: 属性：

| Type 类型 | Name 名字 | Default 违约 |
| --- | --- | --- |
| `int` | [block\_size\_po2 block\_size\_po2](https://voxel-tools.readthedocs.io/en/latest/api/VoxelStreamRegionFiles/#i_block_size_po2) | 4 |
| `String` | [directory 目录](https://voxel-tools.readthedocs.io/en/latest/api/VoxelStreamRegionFiles/#i_directory) | "" |
| `int` | [lod\_count lod\_count](https://voxel-tools.readthedocs.io/en/latest/api/VoxelStreamRegionFiles/#i_lod_count) | 1 |
| `int` | [region\_size\_po2 region\_size\_po2](https://voxel-tools.readthedocs.io/en/latest/api/VoxelStreamRegionFiles/#i_region_size_po2) | 4 |
| `int` | [sector\_size sector\_size](https://voxel-tools.readthedocs.io/en/latest/api/VoxelStreamRegionFiles/#i_sector_size) | 512 |

## Methods: 方法：

## Property Descriptions 属性描述

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **block\_size\_po2** = 4 intblock\_size\_po2 = 4
    
-   [String](https://docs.godotengine.org/en/stable/classes/class_string.html) **directory** = "" 字符串目录 = “”
    

Directory under which the data is saved.  
保存数据的目录。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **lod\_count** = 1 intlod\_count = 1
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **region\_size\_po2** = 4 intregion\_size\_po2 = 4
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **sector\_size** = 512 intsector\_size = 512
    

## Method Descriptions 方法说明

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelStreamRegionFiles/#) **convert\_files**( [Dictionary](https://docs.godotengine.org/en/stable/classes/class_dictionary.html) new\_settings )  
    voidconvert\_files（ 词典 new\_settings ）
    
-   [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) **get\_region\_size**( )  
    Vector3get\_region\_size（ ）
    

_Generated on Sep 12, 2023  
生成于 Sep 12， 2023_
