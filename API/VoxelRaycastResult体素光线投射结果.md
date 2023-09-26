---
created: 2023-09-27T00:01:21 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelRaycastResult/
author: 
---

# VoxelRaycastResult体素光线投射结果

> ## Excerpt
> Inherits: RefCounted 继承：引用计数

---
Inherits: [RefCounted](https://docs.godotengine.org/en/stable/classes/class_refcounted.html) 继承：引用计数

Result of a raycast performed with [VoxelTool.raycast](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#i_raycast)  
使用 VoxelTool.raycast 执行的光线投射的结果

## Properties: 属性：

| Type 类型 | Name 名字 | Default 违约 |
| --- | --- | --- |
| `float` | [distance 距离](https://voxel-tools.readthedocs.io/en/latest/api/VoxelRaycastResult/#i_distance) | \-4.31602e+08 \-4.31602e+08 |
| `Vector3i` | [position 位置](https://voxel-tools.readthedocs.io/en/latest/api/VoxelRaycastResult/#i_position) | Vector3i(0, 0, 0) 矢量3i（0， 0， 0） |
| `Vector3i` | [previous\_position previous\_position](https://voxel-tools.readthedocs.io/en/latest/api/VoxelRaycastResult/#i_previous_position) | Vector3i(0, 0, 0) 矢量3i（0， 0， 0） |

## Property Descriptions 属性描述

-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **distance** = -4.31602e+08  
    浮点距离 = -4.31602e+08
    
-   [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html)
    
    **position** = Vector3i(0, 0, 0)  
    Vector3iposition = Vector3i（0， 0， 0）

Integer position of the voxel that was hit.  
命中的体素的整数位置。

-   [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) **previous\_position** = Vector3i(0, 0, 0)  
    Vector3iprevious\_position = 向量3i（0， 0， 0）

Integer position of the previous voxel along the ray before the final hit.  
最终命中之前前一个体素沿射线的整数位置。

_Generated on Sep 12, 2023  
生成于 Sep 12， 2023_
