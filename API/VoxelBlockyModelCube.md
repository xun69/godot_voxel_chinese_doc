# VoxelBlockyModelCube体素块模型立方体

> ## Excerpt
> 继承：体素块模型

---
##  体素块模型立方体

  
继承：体素块模型

  
生成侧面具有特定图块的多维数据集模型。

##  属性：

|  类型 |  名字 |  违约 |
| --- | --- | --- |
| `Vector2i` | [atlas\_size\_in\_tiles](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModelCube/#i_atlas_size_in_tiles) |  矢量2i（16， 16） |
| `AABB[]` | [collision\_aabbs](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModelCube/#i_collision_aabbs) |   
\[AABB（0， 0， 0， 1， 1， 1）\] |
| `float` |  [高度](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModelCube/#i_height) | 1.0 |

##  方法：

|  返回 |  签名 |
| --- | --- |
|  [矢量2i](https://docs.godotengine.org/en/stable/classes/class_vector2i.html) |   
get\_tile （ int side ） const |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModelCube/#) |   
set\_tile （ int 侧， 矢量2i 位置 ） |

##  属性描述

-     
    Vector2iatlas\_size\_in\_tiles = 向量2i（16， 16）

  
设置纹理图集的引用大小（以拼贴为单位）。必须对其进行设置，以便模型从指定的平铺位置生成正确的纹理坐标。

  
如果您不使用图集，并且每条面都使用相同的完整纹理，请使用 （1,1）。

-     
    AABB\[\]collision\_aabbs = \[AABB（0， 0， 0， 1， 1， 1）\]
    
-    浮点高度 = 1.0
    

##  方法说明

-     
    Vector2iget\_tile（ 内侧 ）
    
-     
    voidset\_tile（ int side， Vector2i 位置 ）
    

_  
生成于 Oct 02， 2023_
