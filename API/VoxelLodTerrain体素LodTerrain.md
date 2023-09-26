---
created: 2023-09-27T00:01:21 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/
author: 
---

# VoxelLodTerrain体素LodTerrain

> ## Excerpt
> Inherits: VoxelNode 继承：体素节点

---
Inherits: [VoxelNode](https://voxel-tools.readthedocs.io/en/latest/api/VoxelNode/) 继承：体素节点

Voxel volume using variable level of detail.  
使用可变细节级别的体素体积。

## Description: 说明：

Renders large terrain using variable level of details. This is preferably used with smooth meshing such as [VoxelMesherTransvoxel](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherTransvoxel/).  
使用可变的细节级别渲染大型地形。这最好与平滑网格一起使用，例如VoxelMesherTransvoxel。

## Properties: 属性：

## Methods: 方法：

| Return 返回 | Signature 签名 |
| --- | --- |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) | [debug\_dump\_as\_scene](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_debug_dump_as_scene) ( [String](https://docs.godotengine.org/en/stable/classes/class_string.html) path, [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) include\_instancer ) const  
debug\_dump\_as\_scene （字符串路径，布尔值include\_instancer）常量 |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) | [debug\_get\_data\_block\_count](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_debug_get_data_block_count) ( ) const  
debug\_get\_data\_block\_count （ ） 常量 |
| [Dictionary 字典](https://docs.godotengine.org/en/stable/classes/class_dictionary.html) | [debug\_get\_data\_block\_info](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_debug_get_data_block_info) ( [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) block\_pos, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) lod ) const  
debug\_get\_data\_block\_info （ Vector3 block\_pos， int lod ） const |
| [bool 布尔](https://docs.godotengine.org/en/stable/classes/class_bool.html) | [debug\_get\_draw\_flag](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_debug_get_draw_flag) ( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) flag\_index ) const  
debug\_get\_draw\_flag （ int flag\_index ） const |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) | [debug\_get\_mesh\_block\_count](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_debug_get_mesh_block_count) ( ) const  
debug\_get\_mesh\_block\_count （ ） 常量 |
| [Dictionary 字典](https://docs.godotengine.org/en/stable/classes/class_dictionary.html) | [debug\_get\_mesh\_block\_info](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_debug_get_mesh_block_info) ( [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) block\_pos, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) lod ) const  
debug\_get\_mesh\_block\_info （ Vector3 block\_pos， int lod ） const |
| [Array 数组](https://docs.godotengine.org/en/stable/classes/class_array.html) | [debug\_get\_octrees\_detailed](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_debug_get_octrees_detailed) ( ) const  
debug\_get\_octrees\_detailed （ ） 常量 |
| [bool 布尔](https://docs.godotengine.org/en/stable/classes/class_bool.html) | [debug\_is\_draw\_enabled](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_debug_is_draw_enabled) ( ) const  
debug\_is\_draw\_enabled （ ） 常量 |
| [Array 数组](https://docs.godotengine.org/en/stable/classes/class_array.html) | [debug\_print\_sdf\_top\_down](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_debug_print_sdf_top_down) ( [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) center, [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) extents )  
debug\_print\_sdf\_top\_down（矢量3i中心，矢量3i范围） |
| [Array 数组](https://docs.godotengine.org/en/stable/classes/class_array.html) | [debug\_raycast\_mesh\_block](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_debug_raycast_mesh_block) ( [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) origin, [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) dir ) const  
debug\_raycast\_mesh\_block （ Vector3 origin， Vector3 dir ） const |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#) | [debug\_set\_draw\_enabled](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_debug_set_draw_enabled) ( [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) enabled )  
debug\_set\_draw\_enabled （ 启用布尔值 ） |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#) | [debug\_set\_draw\_flag](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_debug_set_draw_flag) ( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) flag\_index, [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) enabled )  
debug\_set\_draw\_flag （ int flag\_index， bool 启用 ） |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) | [get\_data\_block\_region\_extent](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_get_data_block_region_extent) ( ) const  
get\_data\_block\_region\_extent （ ） 常量 |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) | [get\_data\_block\_size](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_get_data_block_size) ( ) const  
get\_data\_block\_size （ ） 常量 |
| [VoxelGenerator 体素生成器](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGenerator/) | [get\_normalmap\_generator\_override](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_get_normalmap_generator_override) ( ) const  
get\_normalmap\_generator\_override （ ） 常量 |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) | [get\_normalmap\_generator\_override\_begin\_lod\_index](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_get_normalmap_generator_override_begin_lod_index) ( ) const  
get\_normalmap\_generator\_override\_begin\_lod\_index （ ） 常量 |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) | [get\_process\_callback](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_get_process_callback) ( ) const  
get\_process\_callback （ ） 常量 |
| [Dictionary 字典](https://docs.godotengine.org/en/stable/classes/class_dictionary.html) | [get\_statistics](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_get_statistics) ( ) const  
get\_statistics （ ） 常量 |
| [VoxelTool 体素工具](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/) | [get\_voxel\_tool](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_get_voxel_tool) ( ) get\_voxel\_tool （ ） |
| [bool 布尔](https://docs.godotengine.org/en/stable/classes/class_bool.html) | [is\_area\_meshed](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_is_area_meshed) ( [AABB](https://docs.godotengine.org/en/stable/classes/class_aabb.html) area\_in\_voxels, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) lod\_index ) const  
is\_area\_meshed （ AABB area\_in\_voxels， int lod\_index ） const |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#) | [save\_modified\_blocks](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_save_modified_blocks) ( )  
save\_modified\_blocks （ ） |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#) | [set\_normalmap\_generator\_override](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_set_normalmap_generator_override) ( [VoxelGenerator](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGenerator/) generator\_override )  
set\_normalmap\_generator\_override （ 体素发生器 generator\_override ） |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#) | [set\_normalmap\_generator\_override\_begin\_lod\_index](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_set_normalmap_generator_override_begin_lod_index) ( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) lod\_index )  
set\_normalmap\_generator\_override\_begin\_lod\_index （ 国际 lod\_index ） |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#) | [set\_process\_callback](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_set_process_callback) ( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) mode )  
set\_process\_callback （ 整数模式 ） |
| [Vector3i 矢量3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) | [voxel\_to\_data\_block\_position](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_voxel_to_data_block_position) ( [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) voxel\_position, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) lod\_index ) const  
voxel\_to\_data\_block\_position （ Vector3 voxel\_position， int lod\_index ） const |
| [Vector3i 矢量3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) | [voxel\_to\_mesh\_block\_position](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_voxel_to_mesh_block_position) ( [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) voxel\_position, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) lod\_index ) const  
voxel\_to\_mesh\_block\_position （ Vector3 voxel\_position， int lod\_index ） const |

## Enumerations: 枚举：

enum **ProcessCallback**:  枚举进程回调：

-   **PROCESS\_CALLBACK\_IDLE** = **0** --- The node will use `_process` for the part of its logic running on the main thread.  
    PROCESS\_CALLBACK\_IDLE = 0 --- 节点将用于 `_process` 在主线程上运行的部分逻辑。
-   **PROCESS\_CALLBACK\_PHYSICS** = **1** --- The node will use `_physics_process` for the part of its logic running on the main thread.  
    PROCESS\_CALLBACK\_PHYSICS = 1 --- 节点将用于 `_physics_process` 在主线程上运行的部分逻辑。
-   **PROCESS\_CALLBACK\_DISABLED** = **2** --- The node will not update. Use with caution!  
    PROCESS\_CALLBACK\_DISABLED = 2 --- 节点不会更新。谨慎使用！

enum **DebugDrawFlag**:  enum DebugDrawFlag：

-   **DEBUG\_DRAW\_OCTREE\_NODES** = **0**
-   **DEBUG\_DRAW\_OCTREE\_BOUNDS** = **1**
-   **DEBUG\_DRAW\_MESH\_UPDATES** = **2**
-   **DEBUG\_DRAW\_EDIT\_BOXES** = **3**
-   **DEBUG\_DRAW\_VOLUME\_BOUNDS** = **4**
-   **DEBUG\_DRAW\_EDITED\_BLOCKS** = **5**
-   **DEBUG\_DRAW\_MODIFIER\_BOUNDS** = **6**
-   **DEBUG\_DRAW\_FLAGS\_COUNT** = **7**

## Property Descriptions 属性描述

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **collision\_layer** = 1 intcollision\_layer = 1

Collision layer used by generated colliders. Check Godot documentation for more information.  
生成的碰撞体使用的碰撞层。查看戈多文档以获取更多信息。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **collision\_lod\_count** = 0  
    intcollision\_lod\_count = 0

How many LOD levels are set to generate colliders, starting from LOD 0.  
设置了多少个 LOD 级别以生成碰撞体，从 LOD 0 开始。

-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **collision\_margin** = 0.04  
    floatcollision\_margin = 0.04

Collision margin used by generated colliders. Note that it may depend on which physics engine is used under the hood, as some don't use margins.  
生成的碰撞器使用的碰撞余量。请注意，这可能取决于引擎盖下使用的物理引擎，因为有些不使用边距。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **collision\_mask** = 1 intcollision\_mask = 1

Collision mask used by generated colliders. Check Godot documentation for more information.  
生成的碰撞体使用的碰撞掩码。查看戈多文档以获取更多信息。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **collision\_update\_delay** = 0  
    intcollision\_update\_delay = 0

How long to wait before updating colliders after an edit, in milliseconds. Collider generation is expensive, so the intent is to smooth it out.  
编辑后更新碰撞体之前等待的时间（以毫秒为单位）。碰撞体的生成成本很高，因此目的是使其平滑。

-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **full\_load\_mode\_enabled** = false  
    boolfull\_load\_mode\_enabled = 假

If enabled, data streaming will be turned off, and all voxel data will be loaded from the [VoxelLodTerrain.stream](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_stream) into memory.  
如果启用，数据流将被关闭，所有体素数据将从VoxelLodTerrain.stream加载到内存中。

This removes several constraints, such as being able to edit anywhere and allowing distant normalmaps to include edited regions. This comes at the expense of more memory usage. However, only edited regions use memory, so in practice it can be good enough.  
这消除了一些限制，例如能够在任何位置进行编辑，并允许远程法线贴图包含编辑的区域。这是以牺牲更多内存使用为代价的。但是，只有编辑的区域才会使用内存，因此在实践中它就足够好了。

-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **generate\_collisions** = true  
    boolgenerate\_collisions = 真

If enabled, chunked colliders will be generated from meshes.  
如果启用，将从网格生成分块碰撞体。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **lod\_count** = 4 intlod\_count = 4

How many LOD levels to use. This should be tuned alongside [VoxelLodTerrain.lod\_distance](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_lod_distance): if you want to see very far, you need more LOD levels. This allows blocks to become larger the further away they are, to keep their numbers to an acceptable amount. In contrast, too few LOD levels means regions far away will have to use too many small blocks, which can affect performance.  
要使用的 LOD 级别数。这应该与VoxelLodTerrain.lod\_distance一起调整：如果你想看得很远，你需要更多的LOD级别。这允许块越远越大，以将其数量保持在可接受的数量。相比之下，LOD 级别太少意味着远处的区域将不得不使用太多的小块，这可能会影响性能。

-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **lod\_distance** = 48.0  
    floatlod\_distance = 48.0

How far LOD 0 extends from the viewer. Each parent LOD will extend twice as far as their children LOD levels. When [VoxelLodTerrain.full\_load\_mode\_enabled](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_full_load_mode_enabled) is disabled, this also defines how far edits are allowed.  
LOD 0 从查看器延伸多远。每个父 LOD 的扩展范围将是其子 LOD 级别的两倍。禁用VoxelLodTerrain.full\_load\_mode\_enabled后，这还会定义允许的编辑范围。

-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **lod\_fade\_duration** = 0.0  
    floatlod\_fade\_duration = 0.0

When set greater than 0, enables LOD fading. When mesh blocks get split/merged as level of detail changes, they will fade to make the transition less noticeable (or at least more pleasant). This feature requires to use a specific shader, check the online documentation or examples for more information.  
当设置为大于 0 时，启用 LOD 淡入淡出。当网格块随着细节层次的变化而拆分/合并时，它们会褪色以使过渡不那么明显（或至少更令人愉快）。此功能需要使用特定的着色器，请查看在线文档或示例以获取更多信息。

-   [Material](https://docs.godotengine.org/en/stable/classes/class_material.html) **material** 材料材料

Material used for the surface of the volume. The main usage of this node is with smooth voxels, which means if you want more than one "material" on the ground, you need to use splatmapping techniques with a shader. In addition, many features require shaders to work properly. Check the online documentation or examples for more information.  
用于体积表面的材料。此节点的主要用途是平滑体素，这意味着如果您希望在地面上有多个“材质”，则需要将 splatmap 技术与着色器一起使用。此外，许多功能需要着色器才能正常工作。有关详细信息，请查看联机文档或示例。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **mesh\_block\_size** = 16 intmesh\_block\_size = 16

Size of meshes used for chunks of this volume, in voxels. Can only be set to either 16 or 32. Using 32 is expected to increase rendering performance, and slightly increase the cost of edits.  
用于此体积块的网格大小（以体素为单位）。只能设置为 16 或 32。使用 32 有望提高渲染性能，并略微增加编辑成本。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **normalmap\_begin\_lod\_index** = 2  
    intnormalmap\_begin\_lod\_index = 2

From which LOD index normalmaps will be generated. There won't be normalmaps below this index.  
将从中生成详细级别索引法线贴图。此索引下方不会有法线贴图。

-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **normalmap\_enabled** = false  
    boolnormalmap\_enabled = 假

Enables generation of distant normalmaps. This is a feature used with smooth terrain only (SDF). It is an expensive feature but allows to bring a lot more detail to distant ground.  
支持生成远程法线贴图。此功能仅用于平滑地形 （SDF）。这是一个昂贵的功能，但允许为遥远的地方带来更多细节。

This feature requires to use a specific shader, check the online documentation or examples for more information.  
此功能需要使用特定的着色器，请查看在线文档或示例以获取更多信息。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html)
    
    **normalmap\_max\_deviation\_degrees** = 60  
    intnormalmap\_max\_deviation\_degrees = 60
-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **normalmap\_octahedral\_encoding\_enabled** = false  
    boolnormalmap\_octahedral\_encoding\_enabled = 假
    

Enables octahedral compression of normalmaps, which reduces memory usage caused by distant normalmaps by about 33%, with some impact on visual quality. Your shader may be modified accordingly to decode them.  
启用法线贴图的八面体压缩，从而将远距离法线贴图导致的内存使用量减少约 33%，对视觉质量有一定影响。您的着色器可能会相应地修改以对其进行解码。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **normalmap\_tile\_resolution\_max** = 8  
    intnormalmap\_tile\_resolution\_max = 8

Maximum resolution of tiles in distant normalmaps.  
远距离法线贴图中切片的最大分辨率。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **normalmap\_tile\_resolution\_min** = 4  
    intnormalmap\_tile\_resolution\_min = 4

Minimum resolution of tiles in distant normalmaps.  
远距离法线贴图中切片的最小分辨率。

This is the resolution at which normalmaps will begin with, at the LOD level defined in [VoxelLodTerrain.normalmap\_begin\_lod\_index](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_normalmap_begin_lod_index). Resolutions will double at each LOD level, until they reach [VoxelLodTerrain.normalmap\_tile\_resolution\_max](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_normalmap_tile_resolution_max).  
这是法线贴图在 VoxelLodTerrain.normalmap\_begin\_lod\_index 中定义的 LOD 级别开始的分辨率。分辨率在每个 LOD 级别加倍，直到达到VoxelLodTerrain.normalmap\_tile\_resolution\_max。

-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **normalmap\_use\_gpu** = false  
    boolnormalmap\_use\_gpu = 假

Enables GPU detail normalmaps generation, which can speed it up. This is only valid for generators that support it. Vulkan is required.  
启用 GPU 细节法线贴图生成，从而加快速度。这仅对支持它的生成器有效。Vulkan 是必需的。

-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **run\_stream\_in\_editor** = true  
    boolrun\_stream\_in\_editor = 真

Sets wether the [VoxelLodTerrain.generator](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_generator) and the [VoxelLodTerrain.stream](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_stream) will run in the editor. This setting may turn on automatically if either contain a script, as multithreading can clash with script reloading in unexpected ways.  
VoxelLodTerrain.generator和VoxelLodTerrain.stream将在编辑器中运行的设置。如果包含脚本，此设置可能会自动打开，因为多线程可能会以意外方式与脚本重新加载发生冲突。

-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **threaded\_update\_enabled** = false  
    boolthreaded\_update\_enabled = 假

When enabled, this node will run a large part of its update cycle in a separate thread. Otherwise, it will run on the main thread.  
启用后，此节点将在单独的线程中运行其更新周期的大部分。否则，它将在主线程上运行。

-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **use\_gpu\_generation** = false  
    booluse\_gpu\_generation = 假

Enables GPU block generation, which can speed it up. This is only valid for generators that support it. Vulkan is required.  
启用 GPU 块生成，从而加快速度。这仅对支持它的生成器有效。Vulkan 是必需的。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **view\_distance** = 512 intview\_distance = 512

Maximum distance where terrain will load around viewers. If your terrain size is finite (like for a planet) and you want to keep it in view, you may want to set this value to a very large number. This is mainly useful for infinite terrains.  
地形将在查看器周围加载的最大距离。如果您的地形大小是有限的（例如行星），并且您希望将其保留在视图中，则可能需要将此值设置为非常大的数字。这主要适用于无限地形。

-   [AABB](https://docs.godotengine.org/en/stable/classes/class_aabb.html) **voxel\_bounds** = AABB(-5.36871e+08, -5.36871e+08, -5.36871e+08, 1.07374e+09, 1.07374e+09, 1.07374e+09)  
    AABBvoxel\_bounds = AABB（-5.36871e+08， -5.36871e+08， -5.36871e+08， 1.07374e+09， 1.07374e+09， 1.07374e+09）

Bounds within which volume data can exist (loaded or not), in voxels. By default, it is pseudo-infinite. If you make a planet, island or some sort of arena, you may want to choose a finite size.  
体积数据可以存在于（加载或不加载）的边界，以体素为单位。默认情况下，它是伪无限的。如果你制作一个行星、岛屿或某种竞技场，你可能想选择一个有限的大小。

Note, because this volume uses chunks with LOD, these bounds will snap to the closest chunk boundary.  
请注意，由于此卷使用具有 LOD 的区块，因此这些边界将捕捉到最近的区块边界。

## Method Descriptions 方法说明

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **debug\_dump\_as\_scene**( [String](https://docs.godotengine.org/en/stable/classes/class_string.html) path, [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) include\_instancer )  
    intdebug\_dump\_as\_scene（字符串路径，布尔值include\_instancer）
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **debug\_get\_data\_block\_count**( )  
    intdebug\_get\_data\_block\_count（ ）
    
-   [Dictionary](https://docs.godotengine.org/en/stable/classes/class_dictionary.html) **debug\_get\_data\_block\_info**( [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) block\_pos, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) lod )  
    Dictionarydebug\_get\_data\_block\_info（ Vector3 block\_pos， int lod ）
    
-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **debug\_get\_draw\_flag**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) flag\_index )  
    booldebug\_get\_draw\_flag（ int flag\_index ）
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **debug\_get\_mesh\_block\_count**( )  
    intdebug\_get\_mesh\_block\_count（ ）
    
-   [Dictionary](https://docs.godotengine.org/en/stable/classes/class_dictionary.html) **debug\_get\_mesh\_block\_info**( [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) block\_pos, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) lod )  
    Dictionarydebug\_get\_mesh\_block\_info（ Vector3 block\_pos， int lod ）
    
-   [Array](https://docs.godotengine.org/en/stable/classes/class_array.html) **debug\_get\_octrees\_detailed**( )  
    Arraydebug\_get\_octrees\_detailed（ ）
    
-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **debug\_is\_draw\_enabled**( )  
    booldebug\_is\_draw\_enabled（ ）
    
-   [Array](https://docs.godotengine.org/en/stable/classes/class_array.html) **debug\_print\_sdf\_top\_down**( [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) center, [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) extents )  
    Arraydebug\_print\_sdf\_top\_down（ 矢量3i 中心， 矢量 3i 范围 ）
    
-   [Array](https://docs.godotengine.org/en/stable/classes/class_array.html) **debug\_raycast\_mesh\_block**( [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) origin, [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) dir )  
    Arraydebug\_raycast\_mesh\_block（ 矢量 3 原点， 矢量 3 目录 ）
    
-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#) **debug\_set\_draw\_enabled**( [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) enabled )  
    voiddebug\_set\_draw\_enabled（启用布尔值）
    
-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#) **debug\_set\_draw\_flag**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) flag\_index, [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) enabled )  
    voiddebug\_set\_draw\_flag（ int flag\_index， bool 启用 ）
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **get\_data\_block\_region\_extent**( )  
    intget\_data\_block\_region\_extent（ ）
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **get\_data\_block\_size**( )  
    intget\_data\_block\_size（ ）
    

Gets the size of one cunic data block in voxels.  
获取一个 cunic 数据块的大小（以体素为单位）。

-   [VoxelGenerator](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGenerator/) **get\_normalmap\_generator\_override**( )  
    VoxelGeneratorget\_normalmap\_generator\_override（ ）
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **get\_normalmap\_generator\_override\_begin\_lod\_index**( )  
    intget\_normalmap\_generator\_override\_begin\_lod\_index（ ）
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **get\_process\_callback**( )  
    intget\_process\_callback（ ）
    

Gets which callback is used to run the main thread update of this node.  
获取用于运行此节点的主线程更新的回调。

-   [Dictionary](https://docs.godotengine.org/en/stable/classes/class_dictionary.html) **get\_statistics**( )  
    Dictionaryget\_statistics（ ）

Gets debug information about how much time is spent processing the terrain.  
获取有关处理地形所花费的时间的调试信息。

The returned dictionary has the following structure:  
返回的字典具有以下结构：

```
{
    "time_detect_required_blocks": int,
    "time_request_blocks_to_load": int,
    "time_process_load_responses": int,
    "time_request_blocks_to_update": int,
    "time_process_update_responses": int,
    "remaining_main_thread_blocks": int,
    "dropped_block_loads": int,
    "dropped_block_meshs": int,
    "updated_blocks": int,
    "blocked_lods": int
}

```

-   [VoxelTool](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/) **get\_voxel\_tool**( )  
    VoxelToolget\_voxel\_tool（ ）

Gets an instance of [VoxelTool](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/) bound to this volume. Allows to query and edit voxels.  
获取绑定到此卷的 VoxelTool 实例。允许查询和编辑体素。

-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **is\_area\_meshed**( [AABB](https://docs.godotengine.org/en/stable/classes/class_aabb.html) area\_in\_voxels, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) lod\_index )  
    boolis\_area\_meshed（ AABB area\_in\_voxels， int lod\_index ）

Returns true if the area has been processed by meshing. It does not mean the area actually contains a mesh.  
如果区域已通过网格划分进行处理，则返回 true。这并不意味着该区域实际上包含网格。

Returns false if the area has not been processed by meshing (therefore it is unknown whethere there should be a mesh here or not).  
如果该区域尚未通过网格处理，则返回 false（因此不知道这里是否应该有网格）。

When streaming terrain, this can be used to determine if an area has fully "loaded", in case the game relies meshes or mesh colliders.  
流式传输地形时，这可用于确定某个区域是否已完全“加载”，以防游戏依赖于网格或网格碰撞体。

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#) **save\_modified\_blocks**( )  
    voidsave\_modified\_blocks（ ）

Requests saving of all modified voxels. Saving is asynchronous and will complete some time in the future. If the game quits, the engine will ensure saving tasks get completed before the application shuts down.  
请求保存所有修改的体素。保存是异步的，将在将来的某个时间完成。如果游戏退出，引擎将确保在应用程序关闭之前完成保存任务。

There is currently no reliable way to tell if saving has completed.  
目前没有可靠的方法来判断保存是否已完成。

Note that blocks getting unloaded as the viewer moves around can also trigger saving tasks, independently from this function.  
请注意，当查看器四处移动时卸载的块也可以触发保存任务，独立于此功能。

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#) **set\_normalmap\_generator\_override**( [VoxelGenerator](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGenerator/) generator\_override )  
    voidset\_normalmap\_generator\_override （ 体素发生器 generator\_override ）
    
-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#) **set\_normalmap\_generator\_override\_begin\_lod\_index**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) lod\_index )  
    voidset\_normalmap\_generator\_override\_begin\_lod\_index（ int lod\_index ）
    
-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#) **set\_process\_callback**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) mode )  
    voidset\_process\_callback（ 整型 ）
    

Sets which process callback is used to run the main thread update of this node. By default, it uses `_process`.  
设置用于运行此节点的主线程更新的进程回调。默认情况下，它使用 `_process` .

-   [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) **voxel\_to\_data\_block\_position**( [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) voxel\_position, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) lod\_index )  
    Vector3ivoxel\_to\_data\_block\_position（ 矢量3 voxel\_position， int lod\_index ）

Converts a voxel position into a data block position for a specific LOD index.  
将体素位置转换为特定 LOD 索引的数据块位置。

-   [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) **voxel\_to\_mesh\_block\_position**( [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) voxel\_position, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) lod\_index )  
    Vector3ivoxel\_to\_mesh\_block\_position（ 矢量3 voxel\_position， int lod\_index ）

Converts a voxel position into a mesh block position for a specific LOD index.  
将体素位置转换为特定 LOD 索引的网格块位置。

_Generated on Sep 12, 2023  
生成于 Sep 12， 2023_
