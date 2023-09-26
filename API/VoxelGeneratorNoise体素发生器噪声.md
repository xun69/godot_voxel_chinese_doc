---
created: 2023-09-27T00:01:21 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorNoise/
author: 
---

# VoxelGeneratorNoise体素发生器噪声

> ## Excerpt
> Inherits: VoxelGenerator 继承：体素生成器

---
Inherits: [VoxelGenerator](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGenerator/) 继承：体素生成器

Voxel generator producing overhanging shapes using 3D noise.  
体素发生器使用 3D 噪声生成悬垂形状。

## Properties: 属性：

| Type 类型 | Name 名字 | Default 违约 |
| --- | --- | --- |
| `int` | [channel 渠道](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorNoise/#i_channel) | 1 |
| `float` | [height\_range height\_range](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorNoise/#i_height_range) | 300.0 |
| `float` | [height\_start height\_start](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorNoise/#i_height_start) | 0.0 |
| `Noise` | [noise 噪声](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorNoise/#i_noise) |  |

## Property Descriptions 属性描述

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **channel** = 1 内部通道 = 1

Channel into which the generator will produce voxel data. This depends on the type of meshing you need.  
生成器将在其中生成体素数据的通道。这取决于您需要的网格划分类型。

-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **height\_range** = 300.0  
    floatheight\_range = 300.0

Range of altitudes within which the shape variations will be found. The higher this range, the more overhangs there will be.  
将在其中找到形状变化的高度范围。这个范围越高，悬垂就越多。

Shapes will start at maximum density near the base of the shape (low probability to find air), and progressively loose density until it reaches maximum height.  
形状将从形状底部附近的最大密度开始（找到空气的可能性很低），并逐渐松散密度，直到达到最大高度。

-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **height\_start** = 0.0 floatheight\_start = 0.0

Base of the shape. Everything below it will be filled with ground.  
形状的底部。它下面的一切都将被地面填满。

-   [Noise](https://docs.godotengine.org/en/stable/classes/class_noise.html) **noise** 噪音噪声

Noise used as density function. It is required for the generator to work.  
噪声用作密度函数。发电机工作需要它。

_Generated on Sep 12, 2023  
生成于 Sep 12， 2023_
