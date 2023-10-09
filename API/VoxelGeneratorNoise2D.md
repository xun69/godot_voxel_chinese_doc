---
created: 2023-10-09T22:38:26 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorNoise2D/
author: 
---

# VoxelGeneratorNoise2D体素发生器噪声2D

> ## Excerpt
> 继承：体素生成器高度图

---
-   [](https://voxel-tools.readthedocs.io/en/latest/)
  
脚本 API 体素生成器噪声2D

___

  
继承：体素生成器高度图

  
体素生成器生成基于噪声的高度图地形。

##  属性：

|  类型 |  名字 |  违约 |
| --- | --- | --- |
| `Curve` |  [曲线](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorNoise2D/#i_curve) |  |
| `float` | [height\_range](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorNoise2D/#i_height_range) | 200.0 |
| `Noise` |  [噪声](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorNoise2D/#i_noise) |  |

##  属性描述

-    曲线曲线

  
分配后，此曲线将改变高度变化的分布，从而允许为生成的形状提供某种“轮廓”。

  
默认情况下，使用从 0 到 1 的线性曲线。

-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **height\_range** = 200.0
    
-    噪音噪声
    

  
用于生成高度贴图的噪声。发电机工作需要它。

_  
生成于 Oct 02， 2023_
