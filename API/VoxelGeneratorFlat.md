---
created: 2023-10-09T22:38:26 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorFlat/
author: 
---

# VoxelGeneratorFlat体素生成器平面

> ## Excerpt
> 继承：体素生成器

---
-   [](https://voxel-tools.readthedocs.io/en/latest/)
  
脚本 API 体素生成器平面

___

##  体素生成器平面

 继承：体素生成器

  
体素生成器产生无限平坦的地面。

##  属性：

|  类型 |  名字 |  违约 |
| --- | --- | --- |
| `int` |  [渠道](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorFlat/#i_channel) | 1 |
| `float` |  [高度](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorFlat/#i_height) | 0.0 |
| `int` | [voxel\_type](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorFlat/#i_voxel_type) | 1 |

##  属性描述

-    内部通道 = 1

  
将用于生成接地的通道。

-    浮点高度 = 0.0

  
地面的高度。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **voxel\_type** = 1

  
如果 VoxelGeneratorFlat.channel 设置为 VoxelBuffer.CHANNEL\_TYPE，则此值将用于填充地面体素。

_  
生成于 Oct 02， 2023_
