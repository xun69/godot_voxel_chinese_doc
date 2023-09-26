---
created: 2023-09-27T00:01:21 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorHeightmap/
author: 
---

# VoxelGeneratorHeightmap体素生成器高度图

> ## Excerpt
> Inherits: VoxelGenerator 继承：体素生成器

---
Inherits: [VoxelGenerator](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGenerator/) 继承：体素生成器

## Properties: 属性：

| Type 类型 | Name 名字 | Default 违约 |
| --- | --- | --- |
| `int` | [channel 渠道](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorHeightmap/#i_channel) | 1 |
| `float` | [height\_range height\_range](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorHeightmap/#i_height_range) | 30.0 |
| `float` | [height\_start height\_start](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorHeightmap/#i_height_start) | \-50.0 |
| `float` | [iso\_scale iso\_scale](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorHeightmap/#i_iso_scale) | 0.002 |

## Property Descriptions 属性描述

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **channel** = 1 内部通道 = 1
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **height\_range** = 30.0  
    floatheight\_range = 30.0
    

Maximum distance between the lowest and highest surface points that can generate.  
可以生成的最低和最高表面点之间的最大距离。

NOTE: due to a bug in Godot's documentation tool, the default value shown here is not 30.0, but 200.0. This seems to be because one of the subclasses, `VoxelGeneratorWaves`, has a different default value, chosen for better practical results. This property also appears in some subclasses now, despite being defined in the base class.  
注意：由于Godot文档工具中的错误，此处显示的默认值不是30.0，而是200.0。这似乎是因为其中一个子类 `VoxelGeneratorWaves` 具有不同的默认值，选择该值是为了获得更好的实际结果。此属性现在也出现在一些子类中，尽管它是在基类中定义的。

-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **height\_start** = -50.0  
    floatheight\_start = -50.0

Minimum height where the surface will generate.  
将生成曲面的最小高度。

-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **iso\_scale** = 0.002 floatiso\_scale = 0.002

Scale applied to the signed distance field. This is useful when smooth voxels are used, to reduce blockyness over large distances.  
应用于带符号距离字段的比例。这在使用平滑体素时非常有用，以减少远距离的块状。

_Generated on Sep 12, 2023  
生成于 Sep 12， 2023_
