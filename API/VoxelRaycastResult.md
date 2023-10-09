---
created: 2023-10-09T22:38:26 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelRaycastResult/
author: 
---

# VoxelRaycastResult体素光线投射结果

> ## Excerpt
> 继承：引用计数

---
-   [](https://voxel-tools.readthedocs.io/en/latest/)
  
脚本 API 体素光线投射结果

___

##  体素光线投射结果

 继承：引用计数

  
使用 VoxelTool.raycast 执行的光线投射的结果

##  属性：

|  类型 |  名字 |  违约 |
| --- | --- | --- |
| `float` |  [距离](https://voxel-tools.readthedocs.io/en/latest/api/VoxelRaycastResult/#i_distance) | \-4.31602e+08 |
| `Vector3i` |  [位置](https://voxel-tools.readthedocs.io/en/latest/api/VoxelRaycastResult/#i_position) |  矢量3i（0， 0， 0） |
| `Vector3i` | [previous\_position](https://voxel-tools.readthedocs.io/en/latest/api/VoxelRaycastResult/#i_previous_position) |  矢量3i（0， 0， 0） |

##  属性描述

-     
    浮点距离 = -4.31602e+08
    
-     
    Vector3iposition = Vector3i（0， 0， 0）
    

  
命中的体素的整数位置。

-     
    Vector3iprevious\_position = 向量3i（0， 0， 0）

  
最终命中之前前一个体素沿射线的整数位置。

_  
生成于 Oct 02， 2023_
