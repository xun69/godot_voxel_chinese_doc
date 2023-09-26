---
created: 2023-09-27T00:01:21 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherCubes/
author: 
---

# VoxelMesherCubes体素网格立方体

> ## Excerpt
> Inherits: VoxelMesher 继承：体素梅舍

---
Inherits: [VoxelMesher](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesher/) 继承：体素梅舍

## Properties: 属性：

| Type 类型 | Name 名字 | Default 违约 |
| --- | --- | --- |
| `int` | [color\_mode color\_mode](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherCubes/#i_color_mode) | 0 |
| `bool` | [greedy\_meshing\_enabled greedy\_meshing\_enabled](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherCubes/#i_greedy_meshing_enabled) | true 真 |
| `Material` | [opaque\_material opaque\_material](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherCubes/#i_opaque_material) |  |
| `VoxelColorPalette` | [palette 调色板](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherCubes/#i_palette) |  |
| `Material` | [transparent\_material transparent\_material](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherCubes/#i_transparent_material) |  |

## Methods: 方法：

## Enumerations: 枚举：

enum **Materials**:  枚举材料：

-   **MATERIAL\_OPAQUE** = **0**
-   **MATERIAL\_TRANSPARENT** = **1**
-   **MATERIAL\_COUNT** = **2**

enum **ColorMode**:  枚举颜色模式：

-   **COLOR\_RAW** = **0**
-   **COLOR\_MESHER\_PALETTE** = **1**
-   **COLOR\_SHADER\_PALETTE** = **2**

## Property Descriptions 属性描述

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **color\_mode** = 0 intcolor\_mode = 0
    
-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **greedy\_meshing\_enabled** = true  
    boolgreedy\_meshing\_enabled = 真
    
-   [Material](https://docs.godotengine.org/en/stable/classes/class_material.html) **opaque\_material** Materialopaque\_material
    
-   [VoxelColorPalette](https://voxel-tools.readthedocs.io/en/latest/api/VoxelColorPalette/) **palette**  
    体素调色板调色板
    
-   [Material](https://docs.godotengine.org/en/stable/classes/class_material.html) **transparent\_material**  
    Materialtransparent\_material
    

## Method Descriptions 方法说明

-   [Mesh](https://docs.godotengine.org/en/stable/classes/class_mesh.html)
    
    **generate\_mesh\_from\_image**( [Image](https://docs.godotengine.org/en/stable/classes/class_image.html) image, [float](https://docs.godotengine.org/en/stable/classes/class_float.html) voxel\_size )  
    Meshgenerate\_mesh\_from\_image（ 图像，浮动voxel\_size ）
-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherCubes/#) **set\_material\_by\_index**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) id, [Material](https://docs.godotengine.org/en/stable/classes/class_material.html) material )  
    voidset\_material\_by\_index（ int id， 材料 ）
    

_Generated on Sep 12, 2023  
生成于 Sep 12， 2023_
