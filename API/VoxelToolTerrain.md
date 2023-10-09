---
created: 2023-10-09T22:38:26 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelToolTerrain/
author: 
---

# VoxelToolTerrain体素工具地形

> ## Excerpt
> 继承：体素工具

---
 继承：体素工具

  
VoxelTool的实现，专门用于VoxelTerrain。

##  说明：

  
此类中的函数特定于 VoxelTerrain。对于通用函数，您也可以检查VoxelTool。

  
它不是一个单独实例化的类，您可以使用该方法 `get_voxel_tool()` 从 VoxelTerrain 获取它。

##  方法：

|  返回 |  签名 |
| --- | --- |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelToolTerrain/#) |   
do\_hemisphere（矢量3中心，浮点半径，矢量3 flat\_direction，浮点平滑度=0.0） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelToolTerrain/#) |   
for\_each\_voxel\_metadata\_in\_area （ AABB voxel\_area， 可调用回调 ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelToolTerrain/#) |   
run\_blocky\_random\_tick （ AABB 区域， int voxel\_count， 可调用回调， int batch\_count=16 ） |

##  方法说明

-     
    voiddo\_hemisphere（矢量3中心，浮点半径，矢量3 flat\_direction，浮点平滑度=0.0）
    
-     
    voidfor\_each\_voxel\_metadata\_in\_area（ AABB voxel\_area，可回调）
    

  
为保存给定区域中元数据的每个体素执行一个函数。

  
给定的回调采用两个参数：体素位置 （Vector3i）、体素元数据 （Variant）。

  
重要说明：不允许在此函数中插入新元数据或删除元数据。

-     
    voidrun\_blocky\_random\_tick（ AABB 区域， 整数 voxel\_count， 可调用回调， 整数 batch\_count=16 ）

  
选取指定区域内的随机体素并对其执行函数。这仅适用于使用VoxelMesherBlocky的地形。只会选取Voxel.random\_tickable所在的 `true` 体素。

  
给定的回调有两个参数：体素位置 （Vector3i）、体素值 （int）。

_  
生成于 Oct 02， 2023_
