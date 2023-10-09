---
created: 2023-10-09T22:38:26 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorGraph/
author: 
---

# VoxelGeneratorGraph体素生成器图

> ## Excerpt
> 继承：体素生成器

---
##  体素生成器图

 继承：体素生成器

  
基于图形的体素生成器。

##  说明：

  
从每个体素操作的图形生成体素数据。

  
必须创建、编译图形，然后才能生成块。

  
它可用于基于SDF的光滑地形，也可以用于块状地形。

  
警告：修改图形的方法只能从主线程调用。

##  属性：

|  类型 |  名字 |  违约 |
| --- | --- | --- |
| `bool` | [debug\_block\_clipping](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorGraph/#i_debug_block_clipping) |  假 |
| `float` | [sdf\_clip\_threshold](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorGraph/#i_sdf_clip_threshold) | 1.5 |
| `int` | [subdivision\_size](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorGraph/#i_subdivision_size) | 16 |
| `bool` | [use\_optimized\_execution\_map](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorGraph/#i_use_optimized_execution_map) |  真 |
| `bool` | [use\_subdivision](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorGraph/#i_use_subdivision) |  真 |
| `bool` | [use\_xz\_caching](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorGraph/#i_use_xz_caching) |  真 |

##  方法：

|  返回 |  签名 |
| --- | --- |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorGraph/#) |   
bake\_sphere\_bumpmap （ 图像 im、浮ref\_radius、浮sdf\_min、浮sdf\_max） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorGraph/#) |   
bake\_sphere\_normalmap （ 图像 im， 浮子ref\_radius， 浮子强度 ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorGraph/#) |  清除 （ ） |
|  [字典](https://docs.godotengine.org/en/stable/classes/class_dictionary.html) |  编译 （ ） |
|  [矢量2](https://docs.godotengine.org/en/stable/classes/class_vector2.html) |   
debug\_analyze\_range （ Vector3 min\_pos， Vector3 max\_pos ） const |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorGraph/#) |   
debug\_load\_waves\_preset （ ） |
|  [浮](https://docs.godotengine.org/en/stable/classes/class_float.html) |   
debug\_measure\_microseconds\_per\_voxel （ 布尔 use\_singular\_queries ） |
|  [体素图函数](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/) |   
get\_main\_function （ ） 常量 |

##  信号：

-     
    node\_name\_changed（ int node\_id ）

##  属性描述

-     
    booldebug\_block\_clipping = 假

  
启用后，如果图形输出 SDF 数据，则生成的块将被反转，否则会被裁剪。这具有它们显示为“墙壁伪影”的效果，这对于可视化优化发生的位置很有用。

-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **sdf\_clip\_threshold** = 1.5

  
为地形生成 SDF 块时，如果块的范围分析超出此阈值，则其 SDF 数据将被视为全 1 或全 -1。这优化了内存和处理时间。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **subdivision\_size** = 16

  
为地形生成 SDF 方块时，如果方块大小可被此值整除，则范围分析将针对此类细分进行操作。这允许优化更精确的区域。但是，它不能设置得太小，否则开销将超过收益。

-     
    booluse\_optimized\_execution\_map = 真

  
如果启用，则在为地形生成块时，如果发现特定节点在特定区域中不重要，生成器将尝试跳过这些节点。

-     
    booluse\_subdivision = 真

  
如果启用，将使用VoxelGeneratorGraph.subdivision\_size。

-     
    booluse\_xz\_caching = 真

  
如果启用，生成器将仅运行仅依赖于 X 和 Z 的图形分支。当图形的一部分生成高度图时，这是有效的，因为该部分不是体积的。

##  方法说明

-     
    voidbake\_sphere\_bumpmap（图像im，浮动ref\_radius，浮动sdf\_min，浮动sdf\_max）

  
使用发生器生成的 SDF 输出（如果有）烘焙球面凹凸贴图（或高度贴图）。凹凸图使用全景投影。

  
`ref_radius` ：将在其上采样高度的球体的半径。

  
`strength` ：生成的法线强度，可能默认为 1.0。

-     
    voidbake\_sphere\_normalmap（图像im，浮ref\_radius，浮子强度）

  
使用生成器生成的 SDF 输出（如果有）烘焙球面法线贴图。法线贴图使用全景投影。假设发生器产生球形（如行星）。此类法线贴图可用于使用此生成器为地形的远处视图添加更多细节。

  
`ref_radius` ：将在其上对法线进行采样的球体的半径。

  
`strength` ：生成的法线强度，可能默认为 1.0。

  
注意：另一种方法是将距离法线功能与VoxelLodTerrain一起使用。

-    空清（ ）

  
从图形中删除所有节点和连接。

-    字典编译（ ）

  
编译图形，使其可用于生成块。

  
如果成功，则返回的结果是具有以下布局的字典：

```
{
    "success": true
}
```

  
如果失败，返回的结果可能包含一条消息和可能是原因的图形节点的 ID：

```
{
    "success": false,
    "node_id": int,
    "message": String
}
```

  
如果错误与特定节点无关，则节点 ID 将为 -1。

-     
    Vector2debug\_analyze\_range（ 矢量3 min\_pos， 矢量3 max\_pos ）
    
-     
    voiddebug\_load\_waves\_preset（ ）
    
-     
    floatdebug\_measure\_microseconds\_per\_voxel（ 布尔 use\_singular\_queries ）
    
-     
    VoxelGraphFunctionget\_main\_function（ ）
    

_  
生成于 Oct 02， 2023_
