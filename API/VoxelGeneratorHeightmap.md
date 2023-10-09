---
created: 2023-10-09T22:38:26 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorHeightmap/
author: 
---

# VoxelGeneratorHeightmap体素生成器高度图

> ## Excerpt
> 继承：体素生成器

---
-   [](https://voxel-tools.readthedocs.io/en/latest/)
  
脚本 API 体素生成器高度图

___

##   
体素生成器高度图

 继承：体素生成器

  
继承者： VoxelGeneratorImage， VoxelGeneratorNoise2D， VoxelGeneratorWaves

##  属性：

|  类型 |  名字 |  违约 |
| --- | --- | --- |
| `int` |  [渠道](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorHeightmap/#i_channel) | 1 |
| `float` | [height\_range](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorHeightmap/#i_height_range) | 30.0 |
| `float` | [height\_start](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorHeightmap/#i_height_start) | \-50.0 |
| `float` | [iso\_scale](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorHeightmap/#i_iso_scale) | 0.002 |

##  属性描述

-    内部通道 = 1
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **height\_range** = 30.0
    

  
可以生成的最低和最高表面点之间的最大距离。

  
注意：由于Godot文档工具中的错误，此处显示的默认值不是30.0，而是200.0。这似乎是因为其中一个子类 `VoxelGeneratorWaves` 具有不同的默认值，选择该值是为了获得更好的实际结果。此属性现在也出现在一些子类中，尽管它是在基类中定义的。

-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **height\_start** = -50.0

  
将生成曲面的最小高度。

-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **iso\_scale** = 0.002

  
应用于带符号距离字段的比例。这在使用平滑体素时非常有用，以减少远距离的块状。

_  
生成于 Oct 02， 2023_
