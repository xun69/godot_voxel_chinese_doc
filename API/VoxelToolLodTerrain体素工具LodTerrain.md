---
created: 2023-09-27T00:01:21 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelToolLodTerrain/
author: 
---

# VoxelToolLodTerrain体素工具LodTerrain

> ## Excerpt
> Inherits: VoxelTool 继承：体素工具

---
Inherits: [VoxelTool](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/) 继承：体素工具

Implementation of [VoxelTool](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/) specialized for uses on [VoxelLodTerrain](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/).  
实现专门用于VoxelLodTerrain的VoxelTool。

## Description: 说明：

Functions in this class are specific to [VoxelLodTerrain](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/). For generic functions, you may also check [VoxelTool](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/).  
此类中的函数特定于 VoxelLodTerrain。对于通用函数，您也可以检查VoxelTool。

It's not a class to instantiate alone, you may get it from [VoxelLodTerrain](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/) using the `get_voxel_tool()` method.  
它不是一个单独实例化的类，您可以使用该方法 `get_voxel_tool()` 从VoxelLodTerrain获取它。

## Methods: 方法：

| Return 返回 | Signature 签名 |
| --- | --- |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelToolLodTerrain/#) | [do\_graph](https://voxel-tools.readthedocs.io/en/latest/api/VoxelToolLodTerrain/#i_do_graph) ( [VoxelGeneratorGraph](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorGraph/) graph, [Transform3D](https://docs.godotengine.org/en/stable/classes/class_transform3d.html) transform, [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) area\_size )  
do\_graph （ 体素生成器图， 变换3D变换， 矢量3 area\_size ） |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelToolLodTerrain/#) | [do\_hemisphere](https://voxel-tools.readthedocs.io/en/latest/api/VoxelToolLodTerrain/#i_do_hemisphere) ( [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) center, [float](https://docs.godotengine.org/en/stable/classes/class_float.html) radius, [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) flat\_direction, [float](https://docs.godotengine.org/en/stable/classes/class_float.html) smoothness=0.0 )  
do\_hemisphere（矢量3中心，浮点半径，矢量3 flat\_direction，浮点平滑度=0.0） |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelToolLodTerrain/#) | [do\_sphere\_async](https://voxel-tools.readthedocs.io/en/latest/api/VoxelToolLodTerrain/#i_do_sphere_async) ( [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) center, [float](https://docs.godotengine.org/en/stable/classes/class_float.html) radius )  
do\_sphere\_async（矢量3中心，浮点半径） |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) | [get\_raycast\_binary\_search\_iterations](https://voxel-tools.readthedocs.io/en/latest/api/VoxelToolLodTerrain/#i_get_raycast_binary_search_iterations) ( ) const  
get\_raycast\_binary\_search\_iterations （ ） 常量 |
| [float 浮](https://docs.godotengine.org/en/stable/classes/class_float.html) | [get\_voxel\_f\_interpolated](https://voxel-tools.readthedocs.io/en/latest/api/VoxelToolLodTerrain/#i_get_voxel_f_interpolated) ( [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) position ) const  
get\_voxel\_f\_interpolated （ 矢量3 位置 ） 常量 |
| [Array 数组](https://docs.godotengine.org/en/stable/classes/class_array.html) | [separate\_floating\_chunks](https://voxel-tools.readthedocs.io/en/latest/api/VoxelToolLodTerrain/#i_separate_floating_chunks) ( [AABB](https://docs.godotengine.org/en/stable/classes/class_aabb.html) box, [Node](https://docs.godotengine.org/en/stable/classes/class_node.html) parent\_node )  
separate\_floating\_chunks （ AABB 框， 节点 parent\_node ） |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelToolLodTerrain/#) | [set\_raycast\_binary\_search\_iterations](https://voxel-tools.readthedocs.io/en/latest/api/VoxelToolLodTerrain/#i_set_raycast_binary_search_iterations) ( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) iterations )  
set\_raycast\_binary\_search\_iterations （ 整数迭代 ） |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelToolLodTerrain/#) | [stamp\_sdf](https://voxel-tools.readthedocs.io/en/latest/api/VoxelToolLodTerrain/#i_stamp_sdf) ( [VoxelMeshSDF](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMeshSDF/) mesh\_sdf, [Transform3D](https://docs.godotengine.org/en/stable/classes/class_transform3d.html) transform, [float](https://docs.godotengine.org/en/stable/classes/class_float.html) isolevel, [float](https://docs.godotengine.org/en/stable/classes/class_float.html) sdf\_scale )  
stamp\_sdf （ 体素网格SDF mesh\_sdf， 变换3D变换， 浮点等值水平， 浮sdf\_scale ） |

## Method Descriptions 方法说明

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelToolLodTerrain/#)
    
    **do\_graph**( [VoxelGeneratorGraph](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorGraph/) graph, [Transform3D](https://docs.godotengine.org/en/stable/classes/class_transform3d.html) transform, [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) area\_size )  
    voiddo\_graph（ 体素生成器图， 变换3D变换， 矢量3 area\_size ）
-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelToolLodTerrain/#) **do\_hemisphere**( [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) center, [float](https://docs.godotengine.org/en/stable/classes/class_float.html) radius, [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) flat\_direction, [float](https://docs.godotengine.org/en/stable/classes/class_float.html) smoothness=0.0 )  
    voiddo\_hemisphere（矢量3中心，浮点半径，矢量3 flat\_direction，浮点平滑度=0.0）
    
-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelToolLodTerrain/#) **do\_sphere\_async**( [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) center, [float](https://docs.godotengine.org/en/stable/classes/class_float.html) radius )  
    voiddo\_sphere\_async（矢量3中心，浮动半径）
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **get\_raycast\_binary\_search\_iterations**( )  
    intget\_raycast\_binary\_search\_iterations（ ）
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **get\_voxel\_f\_interpolated**( [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) position )  
    floatget\_voxel\_f\_interpolated（ 矢量3位置 ）
    
-   [Array](https://docs.godotengine.org/en/stable/classes/class_array.html) **separate\_floating\_chunks**( [AABB](https://docs.godotengine.org/en/stable/classes/class_aabb.html) box, [Node](https://docs.godotengine.org/en/stable/classes/class_node.html) parent\_node )  
    Arrayseparate\_floating\_chunks（ AABB 框， 节点 parent\_node ）
    

Turns floating voxels into RigidBodies.  
将浮动体素转换为刚体。

Chunks of floating voxels are detected within a box. The box is relative to the voxel volume this VoxelTool is attached to. Chunks have to be contained entirely within that box to be considered floating. Chunks are removed from the source volume and transformed into RigidBodies with convex collision shapes. They will be added as child of the provided node. They will start "kinematic", and turn "rigid" after a short time, to allow the terrain to update its colliders after the removal (otherwise they will overlap). The function returns an array of these rigid bodies, which you can use to attach further behavior to them (such as disappearing after some time or distance for example).  
在框中检测到浮动体素块。该框相对于此体素工具所附着的体素体积。块必须完全包含在该框中才能被视为浮动。块从源体积中删除，并转换为具有凸碰撞形状的刚体。它们将被添加为所提供节点的子节点。它们将开始“运动学”，并在短时间内变为“刚性”，以允许地形在移除后更新其碰撞器（否则它们将重叠）。该函数返回这些刚体的数组，您可以使用这些刚体将进一步的行为附加到它们（例如，在一段时间或距离后消失）。

This algorithm can become expensive quickly, so the box should not be too big. A size of around 30 voxels should be ok.  
这种算法很快就会变得昂贵，所以盒子不应该太大。大约 30 个体素的大小应该没问题。

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelToolLodTerrain/#) **set\_raycast\_binary\_search\_iterations**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) iterations )  
    voidset\_raycast\_binary\_search\_iterations（ 整数迭代 ）
    
-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelToolLodTerrain/#) **stamp\_sdf**( [VoxelMeshSDF](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMeshSDF/) mesh\_sdf, [Transform3D](https://docs.godotengine.org/en/stable/classes/class_transform3d.html) transform, [float](https://docs.godotengine.org/en/stable/classes/class_float.html) isolevel, [float](https://docs.godotengine.org/en/stable/classes/class_float.html) sdf\_scale )  
    voidstamp\_sdf（体素网格SDF mesh\_sdf，变换3D变换，浮点等值水平，浮sdf\_scale）
    

_Generated on Sep 12, 2023  
生成于 Sep 12， 2023_
