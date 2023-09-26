---
created: 2023-09-27T00:01:21 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorGraph/
author: 
---

# VoxelGeneratorGraph体素生成器图

> ## Excerpt
> Inherits: VoxelGenerator 继承：体素生成器

---
Inherits: [VoxelGenerator](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGenerator/) 继承：体素生成器

Graph-based voxel generator.  
基于图形的体素生成器。

## Description: 说明：

Generates voxel data from a graph of per-voxel operations.  
从每个体素操作的图形生成体素数据。

The graph must be created, compiled, and only then blocks can be generated.  
必须创建、编译图形，然后才能生成块。

It can be used with SDF-based smooth terrain, and also blocky terrains.  
它可用于基于SDF的光滑地形，也可以用于块状地形。

Warning: methods to modify the graph should only be called from the main thread.  
警告：修改图形的方法只能从主线程调用。

## Properties: 属性：

## Methods: 方法：

## Signals: 信号：

-   node\_name\_changed( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) node\_id )  
    node\_name\_changed（ int node\_id ）

## Property Descriptions 属性描述

-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **debug\_block\_clipping** = false  
    booldebug\_block\_clipping = 假

When enabled, if the graph outputs SDF data, generated blocks that would otherwise be clipped will be inverted. This has the effect of them showing up as "walls artifacts", which is useful to visualize where the optimization occurs.  
启用后，如果图形输出 SDF 数据，则生成的块将被反转，否则会被裁剪。这具有它们显示为“墙壁伪影”的效果，这对于可视化优化发生的位置很有用。

-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **sdf\_clip\_threshold** = 1.5  
    floatsdf\_clip\_threshold = 1.5

When generating SDF blocks for a terrain, if the range analysis of a block is beyond this threshold, its SDF data will be considered either fully 1, or fully -1. This optimizes memory and processing time.  
为地形生成 SDF 块时，如果块的范围分析超出此阈值，则其 SDF 数据将被视为全 1 或全 -1。这优化了内存和处理时间。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **subdivision\_size** = 16  
    intsubdivision\_size = 16

When generating SDF blocks for a terrain, and if block size is divisible by this value, range analysis will operate on such subdivision. This allows to optimize away more precise areas. However, it may not be set too small otherwise overhead will outweight the benefits.  
为地形生成 SDF 方块时，如果方块大小可被此值整除，则范围分析将针对此类细分进行操作。这允许优化更精确的区域。但是，它不能设置得太小，否则开销将超过收益。

-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **use\_optimized\_execution\_map** = true  
    booluse\_optimized\_execution\_map = 真

If enabled, when generating blocks for a terrain, the generator will attempt to skip specific nodes if they are found to have no importance in specific areas.  
如果启用，则在为地形生成块时，如果发现特定节点在特定区域中不重要，生成器将尝试跳过这些节点。

-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **use\_subdivision** = true  
    booluse\_subdivision = 真

If enabled, [VoxelGeneratorGraph.subdivision\_size](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorGraph/#i_subdivision_size) will be used.  
如果启用，将使用VoxelGeneratorGraph.subdivision\_size。

-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **use\_xz\_caching** = true  
    booluse\_xz\_caching = 真

If enabled, the generator will run only once branches of the graph that only depend on X and Z. This is effective when part of the graph generates a heightmap, as this part is not volumetric.  
如果启用，生成器将仅运行仅依赖于 X 和 Z 的图形分支。当图形的一部分生成高度图时，这是有效的，因为该部分不是体积的。

## Method Descriptions 方法说明

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorGraph/#) **bake\_sphere\_bumpmap**( [Image](https://docs.godotengine.org/en/stable/classes/class_image.html) im, [float](https://docs.godotengine.org/en/stable/classes/class_float.html) ref\_radius, [float](https://docs.godotengine.org/en/stable/classes/class_float.html) sdf\_min, [float](https://docs.godotengine.org/en/stable/classes/class_float.html) sdf\_max )  
    voidbake\_sphere\_bumpmap（图像im，浮动ref\_radius，浮动sdf\_min，浮动sdf\_max）

Bakes a spherical bumpmap (or heightmap) using SDF output produced by the generator, if any. The bumpmap uses a panorama projection.  
使用发生器生成的 SDF 输出（如果有）烘焙球面凹凸贴图（或高度贴图）。凹凸图使用全景投影。

`ref_radius`: radius of the sphere on which heights will be sampled.  
`ref_radius` ：将在其上采样高度的球体的半径。

`strength`: strength of produced normals, may default to 1.0.  
`strength` ：生成的法线强度，可能默认为 1.0。

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorGraph/#) **bake\_sphere\_normalmap**( [Image](https://docs.godotengine.org/en/stable/classes/class_image.html) im, [float](https://docs.godotengine.org/en/stable/classes/class_float.html) ref\_radius, [float](https://docs.godotengine.org/en/stable/classes/class_float.html) strength )  
    voidbake\_sphere\_normalmap（图像im，浮ref\_radius，浮子强度）

Bakes a spherical normalmap using SDF output produced by the generator, if any. The normalmap uses a panorama projection. It is assumed the generator produces a spherical shape (like a planet). Such normalmap can be used to add more detail to distant views of a terrain using this generator.  
使用生成器生成的 SDF 输出（如果有）烘焙球面法线贴图。法线贴图使用全景投影。假设发生器产生球形（如行星）。此类法线贴图可用于使用此生成器为地形的远处视图添加更多细节。

`ref_radius`: radius of the sphere on which normals will be sampled.  
`ref_radius` ：将在其上对法线进行采样的球体的半径。

`strength`: strength of produced normals, may default to 1.0.  
`strength` ：生成的法线强度，可能默认为 1.0。

Note: an alternative is to use distance normals feature with [VoxelLodTerrain](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/).  
注意：另一种方法是将距离法线功能与VoxelLodTerrain一起使用。

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorGraph/#) **clear**( )  空清（ ）

Erases all nodes and connections from the graph.  
从图形中删除所有节点和连接。

-   [Dictionary](https://docs.godotengine.org/en/stable/classes/class_dictionary.html) **compile**( )  字典编译（ ）

Compiles the graph so it can be used to generate blocks.  
编译图形，使其可用于生成块。

If it succeeds, the returned result is a dictionary with the following layout:  
如果成功，则返回的结果是具有以下布局的字典：

If it fails, the returned result may contain a message and the ID of a graph node that could be the cause:  
如果失败，返回的结果可能包含一条消息和可能是原因的图形节点的 ID：

```
{
    "success": false,
    "node_id": int,
    "message": String
}

```

The node ID will be -1 if the error is not about a particular node.  
如果错误与特定节点无关，则节点 ID 将为 -1。

-   [Vector2](https://docs.godotengine.org/en/stable/classes/class_vector2.html) **debug\_analyze\_range**( [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) min\_pos, [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) max\_pos )  
    Vector2debug\_analyze\_range（ 矢量3 min\_pos， 矢量3 max\_pos ）
    
-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorGraph/#) **debug\_load\_waves\_preset**( )  
    voiddebug\_load\_waves\_preset（ ）
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **debug\_measure\_microseconds\_per\_voxel**( [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) use\_singular\_queries )  
    floatdebug\_measure\_microseconds\_per\_voxel（ 布尔 use\_singular\_queries ）
    
-   [VoxelGraphFunction](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/) **get\_main\_function**( )  
    VoxelGraphFunctionget\_main\_function（ ）
    

_Generated on Sep 12, 2023  
生成于 Sep 12， 2023_
