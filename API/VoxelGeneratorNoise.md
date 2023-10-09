---
created: 2023-10-09T22:38:26 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorNoise/
author: 
---

# VoxelGeneratorNoise体素发生器噪声

> ## Excerpt
> 继承：体素生成器

---
-   [](https://voxel-tools.readthedocs.io/en/latest/)
  
脚本 API 体素生成器噪声

___

##  体素发生器噪声

 继承：体素生成器

  
体素发生器使用 3D 噪声生成悬垂形状。

##  属性：

|  类型 |  名字 |  违约 |
| --- | --- | --- |
| `int` |  [渠道](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorNoise/#i_channel) | 1 |
| `float` | [height\_range](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorNoise/#i_height_range) | 300.0 |
| `float` | [height\_start](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorNoise/#i_height_start) | 0.0 |
| `Noise` |  [噪声](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorNoise/#i_noise) |  |

##  属性描述

-    内部通道 = 1

  
生成器将在其中生成体素数据的通道。这取决于您需要的网格划分类型。

-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **height\_range** = 300.0

  
将在其中找到形状变化的高度范围。这个范围越高，悬垂就越多。

  
形状将从形状底部附近的最大密度开始（找到空气的可能性很低），并逐渐松散密度，直到达到最大高度。

-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **height\_start** = 0.0

  
形状的底部。它下面的一切都将被地面填满。

-    噪音噪声

  
噪声用作密度函数。发电机工作需要它。

_  
生成于 Oct 02， 2023_
