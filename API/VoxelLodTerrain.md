---
created: 2023-10-09T22:38:26 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/
author: 
---

# VoxelLodTerrain体素LodTerrain

> ## Excerpt
> 继承：体素节点

---
##  体素地形

 继承：体素节点

  
使用可变细节级别的体素体积。

##  说明：

  
使用可变的细节级别渲染大型地形。这最好与平滑网格一起使用，例如VoxelMesherTransvoxel。

##  属性：

|  类型 |  名字 |  违约 |
| --- | --- | --- |
| `int` | [collision\_layer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_collision_layer) | 1 |
| `int` | [collision\_lod\_count](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_collision_lod_count) | 0 |
| `float` | [collision\_margin](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_collision_margin) | 0.04 |
| `int` | [collision\_mask](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_collision_mask) | 1 |
| `int` | [collision\_update\_delay](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_collision_update_delay) | 0 |
| `bool` | [full\_load\_mode\_enabled](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_full_load_mode_enabled) |  假 |
| `bool` | [generate\_collisions](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_generate_collisions) |  真 |
| `int` | [lod\_count](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_lod_count) | 4 |
| `float` | [lod\_distance](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_lod_distance) | 48.0 |
| `float` | [lod\_fade\_duration](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_lod_fade_duration) | 0.0 |
| `Material` |  [材料](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_material) |  |
| `int` | [mesh\_block\_size](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_mesh_block_size) | 16 |
| `int` | [normalmap\_begin\_lod\_index](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_normalmap_begin_lod_index) | 2 |
| `bool` | [normalmap\_enabled](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_normalmap_enabled) |  假 |
| `int` | [normalmap\_max\_deviation\_degrees](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_normalmap_max_deviation_degrees) | 60 |
| `bool` | [normalmap\_octahedral\_encoding\_enabled](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_normalmap_octahedral_encoding_enabled) |  假 |
| `int` | [normalmap\_tile\_resolution\_max](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_normalmap_tile_resolution_max) | 8 |
| `int` | [normalmap\_tile\_resolution\_min](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_normalmap_tile_resolution_min) | 4 |
| `bool` | [normalmap\_use\_gpu](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_normalmap_use_gpu) |  假 |
| `bool` | [run\_stream\_in\_editor](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_run_stream_in_editor) |  真 |
| `bool` | [threaded\_update\_enabled](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_threaded_update_enabled) |  假 |
| `bool` | [use\_gpu\_generation](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_use_gpu_generation) |  假 |
| `int` | [view\_distance](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_view_distance) | 512 |
| `AABB` | [voxel\_bounds](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#i_voxel_bounds) |   
AABB（-5.36871e+08， -5.36871e+08， -5.36871e+08， 1.07374e+09， 1.07374e+09， 1.07374e+09） |

##  方法：

|  返回 |  签名 |
| --- | --- |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) |   
debug\_dump\_as\_scene （字符串路径，布尔值include\_instancer）常量 |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) |   
debug\_get\_data\_block\_count （ ） 常量 |
|  [字典](https://docs.godotengine.org/en/stable/classes/class_dictionary.html) |   
debug\_get\_data\_block\_info （ Vector3 block\_pos， int lod ） const |
|  [布尔](https://docs.godotengine.org/en/stable/classes/class_bool.html) |   
debug\_get\_draw\_flag （ int flag\_index ） const |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) |   
debug\_get\_mesh\_block\_count （ ） 常量 |
|  [字典](https://docs.godotengine.org/en/stable/classes/class_dictionary.html) |   
debug\_get\_mesh\_block\_info （ Vector3 block\_pos， int lod ） const |
|  [数组](https://docs.godotengine.org/en/stable/classes/class_array.html) |   
debug\_get\_octrees\_detailed （ ） 常量 |
|  [布尔](https://docs.godotengine.org/en/stable/classes/class_bool.html) |   
debug\_is\_draw\_enabled （ ） 常量 |
|  [数组](https://docs.godotengine.org/en/stable/classes/class_array.html) |   
debug\_print\_sdf\_top\_down（矢量3i中心，矢量3i范围） |
|  [数组](https://docs.godotengine.org/en/stable/classes/class_array.html) |   
debug\_raycast\_mesh\_block （ Vector3 origin， Vector3 dir ） const |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#) |   
debug\_set\_draw\_enabled （ 启用布尔值 ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#) |   
debug\_set\_draw\_flag （ int flag\_index， bool 启用 ） |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) |   
get\_data\_block\_region\_extent （ ） 常量 |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) |   
get\_data\_block\_size （ ） 常量 |
|  [体素生成器](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGenerator/) |   
get\_normalmap\_generator\_override （ ） 常量 |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) |   
get\_normalmap\_generator\_override\_begin\_lod\_index （ ） 常量 |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) |   
get\_process\_callback （ ） 常量 |
|  [字典](https://docs.godotengine.org/en/stable/classes/class_dictionary.html) |   
get\_statistics （ ） 常量 |
|  [体素工具](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/) |  get\_voxel\_tool （ ） |
|  [布尔](https://docs.godotengine.org/en/stable/classes/class_bool.html) |   
is\_area\_meshed （ AABB area\_in\_voxels， int lod\_index ） const |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#) |   
save\_modified\_blocks （ ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#) |   
set\_normalmap\_generator\_override （ 体素发生器 generator\_override ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#) |   
set\_normalmap\_generator\_override\_begin\_lod\_index （ 国际 lod\_index ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/#) |   
set\_process\_callback （ 整数模式 ） |
|  [矢量3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) |   
voxel\_to\_data\_block\_position （ Vector3 voxel\_position， int lod\_index ） const |
|  [矢量3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) |   
voxel\_to\_mesh\_block\_position （ Vector3 voxel\_position， int lod\_index ） const |

##  枚举：

 枚举进程回调：

-     
    PROCESS\_CALLBACK\_IDLE = 0 --- 节点将用于 `_process` 在主线程上运行的部分逻辑。
-     
    PROCESS\_CALLBACK\_PHYSICS = 1 --- 节点将用于 `_physics_process` 在主线程上运行的部分逻辑。
-     
    PROCESS\_CALLBACK\_DISABLED = 2 --- 节点不会更新。谨慎使用！

 enum DebugDrawFlag：

-   **DEBUG\_DRAW\_OCTREE\_NODES** = **0**
-   **DEBUG\_DRAW\_OCTREE\_BOUNDS** = **1**
-   **DEBUG\_DRAW\_MESH\_UPDATES** = **2**
-   **DEBUG\_DRAW\_EDIT\_BOXES** = **3**
-   **DEBUG\_DRAW\_VOLUME\_BOUNDS** = **4**
-   **DEBUG\_DRAW\_EDITED\_BLOCKS** = **5**
-   **DEBUG\_DRAW\_MODIFIER\_BOUNDS** = **6**
-   **DEBUG\_DRAW\_FLAGS\_COUNT** = **7**

##  属性描述

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **collision\_layer** = 1

  
生成的碰撞体使用的碰撞层。查看戈多文档以获取更多信息。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **collision\_lod\_count** = 0

  
设置了多少个 LOD 级别以生成碰撞体，从 LOD 0 开始。

-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **collision\_margin** = 0.04

  
生成的碰撞器使用的碰撞余量。请注意，这可能取决于引擎盖下使用的物理引擎，因为有些不使用边距。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **collision\_mask** = 1

  
生成的碰撞体使用的碰撞掩码。查看戈多文档以获取更多信息。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **collision\_update\_delay** = 0

  
编辑后更新碰撞体之前等待的时间（以毫秒为单位）。碰撞体的生成成本很高，因此目的是使其平滑。

-     
    boolfull\_load\_mode\_enabled = 假

  
如果启用，数据流将被关闭，所有体素数据将从VoxelLodTerrain.stream加载到内存中。

  
这消除了一些限制，例如能够在任何位置进行编辑，并允许远程法线贴图包含编辑的区域。这是以牺牲更多内存使用为代价的。但是，只有编辑的区域才会使用内存，因此在实践中它就足够好了。

-     
    boolgenerate\_collisions = 真

  
如果启用，将从网格生成分块碰撞体。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **lod\_count** = 4

  
要使用的 LOD 级别数。这应该与VoxelLodTerrain.lod\_distance一起调整：如果你想看得很远，你需要更多的LOD级别。这允许块越远越大，以将其数量保持在可接受的数量。相比之下，LOD 级别太少意味着远处的区域将不得不使用太多的小块，这可能会影响性能。

-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **lod\_distance** = 48.0

  
LOD 0 从查看器延伸多远。每个父 LOD 的扩展范围将是其子 LOD 级别的两倍。禁用VoxelLodTerrain.full\_load\_mode\_enabled后，这还会定义允许的编辑范围。

-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **lod\_fade\_duration** = 0.0

  
当设置为大于 0 时，启用 LOD 淡入淡出。当网格块随着细节层次的变化而拆分/合并时，它们会褪色以使过渡不那么明显（或至少更令人愉快）。此功能需要使用特定的着色器，请查看在线文档或示例以获取更多信息。

-    材料材料

  
用于体积表面的材料。此节点的主要用途是平滑体素，这意味着如果您希望在地面上有多个“材质”，则需要将 splatmap 技术与着色器一起使用。此外，许多功能需要着色器才能正常工作。有关详细信息，请查看联机文档或示例。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **mesh\_block\_size** = 16

  
用于此体积块的网格大小（以体素为单位）。只能设置为 16 或 32。使用 32 有望提高渲染性能，并略微增加编辑成本。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **normalmap\_begin\_lod\_index** = 2

  
将从中生成详细级别索引法线贴图。此索引下方不会有法线贴图。

-     
    boolnormalmap\_enabled = 假

  
支持生成远程法线贴图。此功能仅用于平滑地形 （SDF）。这是一个昂贵的功能，但允许为遥远的地方带来更多细节。

  
此功能需要使用特定的着色器，请查看在线文档或示例以获取更多信息。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **normalmap\_max\_deviation\_degrees** = 60
    
-     
    boolnormalmap\_octahedral\_encoding\_enabled = 假
    

  
启用法线贴图的八面体压缩，从而将远距离法线贴图导致的内存使用量减少约 33%，对视觉质量有一定影响。您的着色器可能会相应地修改以对其进行解码。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **normalmap\_tile\_resolution\_max** = 8

  
远距离法线贴图中切片的最大分辨率。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **normalmap\_tile\_resolution\_min** = 4

  
远距离法线贴图中切片的最小分辨率。

  
这是法线贴图在 VoxelLodTerrain.normalmap\_begin\_lod\_index 中定义的 LOD 级别开始的分辨率。分辨率在每个 LOD 级别加倍，直到达到VoxelLodTerrain.normalmap\_tile\_resolution\_max。

-     
    boolnormalmap\_use\_gpu = 假

  
启用 GPU 细节法线贴图生成，从而加快速度。这仅对支持它的生成器有效。Vulkan 是必需的。

-     
    boolrun\_stream\_in\_editor = 真

  
VoxelLodTerrain.generator和VoxelLodTerrain.stream将在编辑器中运行的设置。如果包含脚本，此设置可能会自动打开，因为多线程可能会以意外方式与脚本重新加载发生冲突。

-     
    boolthreaded\_update\_enabled = 假

  
启用后，此节点将在单独的线程中运行其更新周期的大部分。否则，它将在主线程上运行。

-     
    booluse\_gpu\_generation = 假

  
启用 GPU 块生成，从而加快速度。这仅对支持它的生成器有效。Vulkan 是必需的。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **view\_distance** = 512

  
地形将在查看器周围加载的最大距离。如果您的地形大小是有限的（例如行星），并且您希望将其保留在视图中，则可能需要将此值设置为非常大的数字。这主要适用于无限地形。

-     
    AABBvoxel\_bounds = AABB（-5.36871e+08， -5.36871e+08， -5.36871e+08， 1.07374e+09， 1.07374e+09， 1.07374e+09）

  
体积数据可以存在于（加载或不加载）的边界，以体素为单位。默认情况下，它是伪无限的。如果你制作一个行星、岛屿或某种竞技场，你可能想选择一个有限的大小。

  
请注意，由于此卷使用具有 LOD 的区块，因此这些边界将捕捉到最近的区块边界。

##  方法说明

-     
    intdebug\_dump\_as\_scene（字符串路径，布尔值include\_instancer）
    
-     
    intdebug\_get\_data\_block\_count（ ）
    
-     
    Dictionarydebug\_get\_data\_block\_info（ Vector3 block\_pos， int lod ）
    
-     
    booldebug\_get\_draw\_flag（ int flag\_index ）
    
-     
    intdebug\_get\_mesh\_block\_count（ ）
    
-     
    Dictionarydebug\_get\_mesh\_block\_info（ Vector3 block\_pos， int lod ）
    
-     
    Arraydebug\_get\_octrees\_detailed（ ）
    
-     
    booldebug\_is\_draw\_enabled（ ）
    
-     
    Arraydebug\_print\_sdf\_top\_down（ 矢量3i 中心， 矢量 3i 范围 ）
    
-     
    Arraydebug\_raycast\_mesh\_block（ 矢量 3 原点， 矢量 3 目录 ）
    
-     
    voiddebug\_set\_draw\_enabled（启用布尔值）
    
-     
    voiddebug\_set\_draw\_flag（ int flag\_index， bool 启用 ）
    
-     
    intget\_data\_block\_region\_extent（ ）
    
-     
    intget\_data\_block\_size（ ）
    

  
获取一个 cunic 数据块的大小（以体素为单位）。

-     
    VoxelGeneratorget\_normalmap\_generator\_override（ ）
    
-     
    intget\_normalmap\_generator\_override\_begin\_lod\_index（ ）
    
-     
    intget\_process\_callback（ ）
    

  
获取用于运行此节点的主线程更新的回调。

-     
    Dictionaryget\_statistics（ ）

  
获取有关处理地形所花费的时间的调试信息。

  
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

-     
    VoxelToolget\_voxel\_tool（ ）

  
获取绑定到此卷的 VoxelTool 实例。允许查询和编辑体素。

-     
    boolis\_area\_meshed（ AABB area\_in\_voxels， int lod\_index ）

  
如果区域已通过网格划分进行处理，则返回 true。这并不意味着该区域实际上包含网格。

  
如果该区域尚未通过网格处理，则返回 false（因此不知道这里是否应该有网格）。

  
流式传输地形时，这可用于确定某个区域是否已完全“加载”，以防游戏依赖于网格或网格碰撞体。

-     
    voidsave\_modified\_blocks（ ）

  
请求保存所有修改的体素。保存是异步的，将在将来的某个时间完成。如果游戏退出，引擎将确保在应用程序关闭之前完成保存任务。

  
目前没有可靠的方法来判断保存是否已完成。

  
请注意，当查看器四处移动时卸载的块也可以触发保存任务，独立于此功能。

-     
    voidset\_normalmap\_generator\_override （ 体素发生器 generator\_override ）
    
-     
    voidset\_normalmap\_generator\_override\_begin\_lod\_index（ int lod\_index ）
    
-     
    voidset\_process\_callback（ 整型 ）
    

  
设置用于运行此节点的主线程更新的进程回调。默认情况下，它使用 `_process` .

-     
    Vector3ivoxel\_to\_data\_block\_position（ 矢量3 voxel\_position， int lod\_index ）

  
将体素位置转换为特定 LOD 索引的数据块位置。

-     
    Vector3ivoxel\_to\_mesh\_block\_position（ 矢量3 voxel\_position， int lod\_index ）

  
将体素位置转换为特定 LOD 索引的网格块位置。

_  
生成于 Oct 02， 2023_
