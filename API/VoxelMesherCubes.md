---
created: 2023-10-09T22:38:26 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherCubes/
author: 
---

# VoxelMesherCubes体素网格立方体

> ## Excerpt
> 继承：体素梅舍

---
##  体素网格立方体

 继承：体素梅舍

##  属性：

|  类型 |  名字 |  违约 |
| --- | --- | --- |
| `int` | [color\_mode](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherCubes/#i_color_mode) | 0 |
| `bool` | [greedy\_meshing\_enabled](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherCubes/#i_greedy_meshing_enabled) |  真 |
| `Material` | [opaque\_material](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherCubes/#i_opaque_material) |  |
| `VoxelColorPalette` |  [调色板](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherCubes/#i_palette) |  |
| `Material` | [transparent\_material](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherCubes/#i_transparent_material) |  |

##  方法：

|  返回 |  签名 |
| --- | --- |
|  [网孔](https://docs.godotengine.org/en/stable/classes/class_mesh.html) |   
generate\_mesh\_from\_image（图像图像，浮点voxel\_size）静态 |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherCubes/#) |   
set\_material\_by\_index （ int id， 材料 ） |

##  枚举：

 枚举材料：

-   **MATERIAL\_OPAQUE** = **0**
-   **MATERIAL\_TRANSPARENT** = **1**
-   **MATERIAL\_COUNT** = **2**

 枚举颜色模式：

-   **COLOR\_RAW** = **0**
-   **COLOR\_MESHER\_PALETTE** = **1**
-   **COLOR\_SHADER\_PALETTE** = **2**

##  属性描述

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **color\_mode** = 0
    
-     
    boolgreedy\_meshing\_enabled = 真
    
-   [Material](https://docs.godotengine.org/en/stable/classes/class_material.html) **opaque\_material**
    
-     
    体素调色板调色板
    
-   [Material](https://docs.godotengine.org/en/stable/classes/class_material.html) **transparent\_material**
    

##  方法说明

-     
    Meshgenerate\_mesh\_from\_image（ 图像，浮动voxel\_size ）
    
-     
    voidset\_material\_by\_index（ int id， 材料 ）
    

_  
生成于 Oct 02， 2023_
