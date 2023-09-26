---
created: 2023-09-27T00:01:21 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorNoise2D/
author: 
---

# VoxelGeneratorNoise2D体素发生器噪声2D

> ## Excerpt
> Inherits: VoxelGeneratorHeightmap继承：体素生成器高度图

---
Inherits: [VoxelGeneratorHeightmap](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorHeightmap/)  
继承：体素生成器高度图

Voxel generator producing noise-based heightmap terrain.  
体素生成器生成基于噪声的高度图地形。

## Properties: 属性：

| Type 类型 | Name 名字 | Default 违约 |
| --- | --- | --- |
| `Curve` | [curve 曲线](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorNoise2D/#i_curve) |  |
| `float` | [height\_range height\_range](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorNoise2D/#i_height_range) | 200.0 |
| `Noise` | [noise 噪声](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorNoise2D/#i_noise) |  |

## Property Descriptions 属性描述

-   [Curve](https://docs.godotengine.org/en/stable/classes/class_curve.html) **curve** 曲线曲线

When assigned, this curve will alter the distribution of height variations, allowing to give some kind of "profile" to the generated shapes.  
分配后，此曲线将改变高度变化的分布，从而允许为生成的形状提供某种“轮廓”。

By default, a linear curve from 0 to 1 is used.  
默认情况下，使用从 0 到 1 的线性曲线。

-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **height\_range** = 200.0  
    floatheight\_range = 200.0
    
-   [Noise](https://docs.godotengine.org/en/stable/classes/class_noise.html)
    
    **noise** 噪音噪声

Noise used to produce the heightmap. It is required for the generator to work.  
用于生成高度贴图的噪声。发电机工作需要它。

_Generated on Sep 12, 2023  
生成于 Sep 12， 2023_
