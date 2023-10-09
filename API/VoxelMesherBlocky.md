---
created: 2023-10-09T22:38:26 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherBlocky/
author: 
---

# VoxelMesherBlocky体素网格块

> ## Excerpt
> 继承：体素梅舍

---
-   [](https://voxel-tools.readthedocs.io/en/latest/)
  
脚本 API VoxelMesherBlocky

___

 继承：体素梅舍

  
通过批处理对应于每个体素值的模型来生成网格，类似于 Minecraft 或 StarMade 等游戏。

##  说明：

  
从结果中去除遮挡面，并且可以在边缘烘烤一定程度的环境光遮蔽。值应位于VoxelBuffer.CHANNEL\_TYPE通道中。模型是使用体素块库定义的，其中模型索引对应于体素值。模型不必是多维数据集。

##  属性：

|  类型 |  名字 |  违约 |
| --- | --- | --- |
| `VoxelBlockyLibraryBase` |  [图书馆](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherBlocky/#i_library) |  |
| `float` | [occlusion\_darkness](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherBlocky/#i_occlusion_darkness) | 0.8 |
| `bool` | [occlusion\_enabled](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherBlocky/#i_occlusion_enabled) |  真 |

##  属性描述

-     
    体素块库基库
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **occlusion\_darkness** = 0.8
    
-     
    boolocclusion\_enabled = 真
    

_  
生成于 Oct 02， 2023_
