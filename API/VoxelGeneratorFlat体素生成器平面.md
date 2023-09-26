---
created: 2023-09-27T00:01:21 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorFlat/
author: 
---

# VoxelGeneratorFlat体素生成器平面

> ## Excerpt
> Inherits: VoxelGenerator 继承：体素生成器

---
Inherits: [VoxelGenerator](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGenerator/) 继承：体素生成器

Voxel generator producing an infinite flat ground.  
体素生成器产生无限平坦的地面。

## Properties: 属性：

| Type 类型 | Name 名字 | Default 违约 |
| --- | --- | --- |
| `int` | [channel 渠道](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorFlat/#i_channel) | 1 |
| `float` | [height 高度](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorFlat/#i_height) | 0.0 |
| `int` | [voxel\_type voxel\_type](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorFlat/#i_voxel_type) | 1 |

## Property Descriptions 属性描述

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **channel** = 1 内部通道 = 1

Channel that will be used to generate the ground.  
将用于生成接地的通道。

-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **height** = 0.0 浮点高度 = 0.0

Altitude of the ground.  
地面的高度。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **voxel\_type** = 1 intvoxel\_type = 1

If [VoxelGeneratorFlat.channel](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorFlat/#i_channel) is set to [VoxelBuffer.CHANNEL\_TYPE](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#enumerations), this value will be used to fill ground voxels.  
如果 VoxelGeneratorFlat.channel 设置为 VoxelBuffer.CHANNEL\_TYPE，则此值将用于填充地面体素。

_Generated on Sep 12, 2023  
生成于 Sep 12， 2023_
