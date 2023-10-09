---
created: 2023-10-09T22:38:26 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelToolLodTerrain/
author: 
---

# VoxelToolLodTerrain体素工具LodTerrain

> ## Excerpt
> 继承：体素工具

---
 继承：体素工具

  
实现专门用于VoxelLodTerrain的VoxelTool。

##  说明：

  
此类中的函数特定于 VoxelLodTerrain。对于通用函数，您也可以检查VoxelTool。

  
它不是一个单独实例化的类，您可以使用该方法 `get_voxel_tool()` 从VoxelLodTerrain获取它。

##  方法：

|  返回 |  签名 |
| --- | --- |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelToolLodTerrain/#) |   
do\_graph （ 体素生成器图， 变换3D变换， 矢量3 area\_size ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelToolLodTerrain/#) |   
do\_hemisphere（矢量3中心，浮点半径，矢量3 flat\_direction，浮点平滑度=0.0） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelToolLodTerrain/#) |   
do\_sphere\_async（矢量3中心，浮点半径） |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) |   
get\_raycast\_binary\_search\_iterations （ ） 常量 |
|  [浮](https://docs.godotengine.org/en/stable/classes/class_float.html) |   
get\_voxel\_f\_interpolated （ 矢量3 位置 ） 常量 |
|  [数组](https://docs.godotengine.org/en/stable/classes/class_array.html) |   
separate\_floating\_chunks （ AABB 框， 节点 parent\_node ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelToolLodTerrain/#) |   
set\_raycast\_binary\_search\_iterations （ 整数迭代 ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelToolLodTerrain/#) |   
stamp\_sdf （ 体素网格SDF mesh\_sdf， 变换3D变换， 浮点等值水平， 浮sdf\_scale ） |

##  方法说明

-     
    voiddo\_graph（ 体素生成器图， 变换3D变换， 矢量3 area\_size ）
    
-     
    voiddo\_hemisphere（矢量3中心，浮点半径，矢量3 flat\_direction，浮点平滑度=0.0）
    
-     
    voiddo\_sphere\_async（矢量3中心，浮动半径）
    
-     
    intget\_raycast\_binary\_search\_iterations（ ）
    
-     
    floatget\_voxel\_f\_interpolated（ 矢量3位置 ）
    
-     
    Arrayseparate\_floating\_chunks（ AABB 框， 节点 parent\_node ）
    

  
将浮动体素转换为刚体。

  
在框中检测到浮动体素块。该框相对于此体素工具所附着的体素体积。块必须完全包含在该框中才能被视为浮动。块从源体积中删除，并转换为具有凸碰撞形状的刚体。它们将被添加为所提供节点的子节点。它们将开始“运动学”，并在短时间内变为“刚性”，以允许地形在移除后更新其碰撞器（否则它们将重叠）。该函数返回这些刚体的数组，您可以使用这些刚体将进一步的行为附加到它们（例如，在一段时间或距离后消失）。

  
这种算法很快就会变得昂贵，所以盒子不应该太大。大约 30 个体素的大小应该没问题。

-     
    voidset\_raycast\_binary\_search\_iterations（ 整数迭代 ）
    
-     
    voidstamp\_sdf（体素网格SDF mesh\_sdf，变换3D变换，浮点等值水平，浮sdf\_scale）
    

_  
生成于 Oct 02， 2023_
