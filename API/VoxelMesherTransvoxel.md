---
created: 2023-10-09T22:38:26 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherTransvoxel/
author: 
---

# VoxelMesherTransvoxel体素网格传输体素

> ## Excerpt
> 继承：体素梅舍

---
-   [](https://voxel-tools.readthedocs.io/en/latest/)
-   Scripting API
-   VoxelMesherTransvoxel

___

 继承：体素梅舍

  
使用Transvoxel算法实现等值面生成（平滑体素）。

##  属性：

##  方法：

|  返回 |  签名 |
| --- | --- |
|  [阵列网格](https://docs.godotengine.org/en/stable/classes/class_arraymesh.html) |   
build\_transition\_mesh （ 体素缓冲区 voxel\_buffer， int 方向 ） |

##  枚举：

 枚举纹理模式：

-   **TEXTURES\_NONE** = **0**
-   **TEXTURES\_BLEND\_4\_OVER\_16** = **1**

##  属性描述

-     
    booldeep\_sampling\_enabled = 假
    
-     
    boolmesh\_optimization\_enabled = 假
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **mesh\_optimization\_error\_threshold** = 0.005
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **mesh\_optimization\_target\_ratio** = 0.0
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **texturing\_mode** = 0
    
-     
    booltransitions\_enabled = 真
    

##  方法说明

-     
    ArrayMeshbuild\_transition\_mesh（体素缓冲区voxel\_buffer，int方向）

_  
生成于 Oct 02， 2023_
