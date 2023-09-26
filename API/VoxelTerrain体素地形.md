---
created: 2023-09-27T00:01:21 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelTerrain/
author: 
---

# VoxelTerrain体素地形

> ## Excerpt
> Inherits: VoxelNode 继承：体素节点

---
Inherits: [VoxelNode](https://voxel-tools.readthedocs.io/en/latest/api/VoxelNode/) 继承：体素节点

Voxel volume using constant level of detail.  
使用恒定细节水平的体素体积。

## Properties: 属性：

| Type 类型 | Name 名字 | Default 违约 |
| --- | --- | --- |
| `bool` | [area\_edit\_notification\_enabled  
area\_edit\_notification\_enabled](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTerrain/#i_area_edit_notification_enabled) | false 假 |
| `bool` | [automatic\_loading\_enabled  
automatic\_loading\_enabled](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTerrain/#i_automatic_loading_enabled) | true 真 |
| `bool` | [block\_enter\_notification\_enabled  
block\_enter\_notification\_enabled](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTerrain/#i_block_enter_notification_enabled) | false 假 |
| `AABB` | [bounds 边界](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTerrain/#i_bounds) | AABB(-5.36871e+08, -5.36871e+08, -5.36871e+08, 1.07374e+09, 1.07374e+09, 1.07374e+09)  
AABB（-5.36871e+08， -5.36871e+08， -5.36871e+08， 1.07374e+09， 1.07374e+09， 1.07374e+09） |
| `int` | [collision\_layer collision\_layer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTerrain/#i_collision_layer) | 1 |
| `float` | [collision\_margin collision\_margin](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTerrain/#i_collision_margin) | 0.04 |
| `int` | [collision\_mask collision\_mask](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTerrain/#i_collision_mask) | 1 |
| `bool` | [generate\_collisions generate\_collisions](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTerrain/#i_generate_collisions) | true 真 |
| `Material` | [material\_override material\_override](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTerrain/#i_material_override) |  |
| `int` | [max\_view\_distance max\_view\_distance](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTerrain/#i_max_view_distance) | 128 |
| `int` | [mesh\_block\_size mesh\_block\_size](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTerrain/#i_mesh_block_size) | 16 |
| `bool` | [run\_stream\_in\_editor run\_stream\_in\_editor](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTerrain/#i_run_stream_in_editor) | true 真 |
| `bool` | [use\_gpu\_generation use\_gpu\_generation](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTerrain/#i_use_gpu_generation) | false 假 |

## Methods: 方法：

## Signals: 信号：

-   block\_loaded( [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) position )  
    block\_loaded（ 矢量3i 位置 ）

Emitted when a new data block is loaded from stream. This can happen before the mesh or collider becomes available.  
从流加载新数据块时发出。这可能在网格或碰撞体可用之前发生。

-   block\_unloaded( [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) position )  
    block\_unloaded（ 矢量3i 位置 ）

Emitted when a data block is unloaded due to being outside view distance.  
在由于超出视图距离而卸载数据块时发出。

-   mesh\_block\_entered( [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) position )  
    mesh\_block\_entered（ 矢量3i 位置 ）

Emitted when a mesh block receives its first update since it was added in the range of viewers. This is regardless of the mesh being empty or not. It tracks changes of the same state obtained with [VoxelTerrain.is\_area\_meshed](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTerrain/#i_is_area_meshed).  
当网格块收到自添加到查看器范围以来的首次更新时发出。这与网格是否为空无关。它跟踪使用VoxelTerrain.is\_area\_meshed获得的相同状态的变化。

-   mesh\_block\_exited( [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) position )  
    mesh\_block\_exited（ 矢量3i 位置 ）

Emitted when a mesh block gets unloaded. It is the counterpart of [VoxelTerrain.mesh\_block\_entered](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTerrain/#signals).  
在卸载网格块时发出。它是VoxelTerrain.mesh\_block\_entered的对应物。

## Property Descriptions 属性描述

-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **area\_edit\_notification\_enabled** = false  
    boolarea\_edit\_notification\_enabled = 假
    
-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **automatic\_loading\_enabled** = true  
    boolautomatic\_loading\_enabled = 真
    
-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **block\_enter\_notification\_enabled** = false  
    boolblock\_enter\_notification\_enabled = 假
    
-   [AABB](https://docs.godotengine.org/en/stable/classes/class_aabb.html) **bounds** = AABB(-5.36871e+08, -5.36871e+08, -5.36871e+08, 1.07374e+09, 1.07374e+09, 1.07374e+09)  
    AABBbounds = AABB（-5.36871e+08， -5.36871e+08， -5.36871e+08， 1.07374e+09， 1.07374e+09， 1.07374e+09）
    

Defines the bounds within which the terrain is allowed to have voxels. If an infinite world generator is used, blocks will only generate within this region. Everything outside will be left empty.  
定义允许地形具有体素的边界。如果使用无限世界生成器，则块将仅在此区域内生成。外面的所有东西都将空置。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **collision\_layer** = 1 intcollision\_layer = 1
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **collision\_margin** = 0.04  
    floatcollision\_margin = 0.04
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **collision\_mask** = 1 intcollision\_mask = 1
    
-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **generate\_collisions** = true  
    boolgenerate\_collisions = 真
    

Enables the generation of collision shapes using the classic physics engine. Use this feature if you need realistic or non-trivial collisions or physics.  
支持使用经典物理引擎生成碰撞形状。如果您需要逼真或非平凡的碰撞或物理，请使用此功能。

Note 1: you also need [VoxelViewer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelViewer/) to request collisions, otherwise they won't generate.  
注意 1：您还需要 VoxelViewer 来请求冲突，否则它们不会生成。

Note 2: If you need simple Minecraft/AABB physics, you can use [VoxelBoxMover](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBoxMover/) which may perform better in blocky worlds.  
注2：如果你需要简单的Minecraft/AABB物理，你可以使用VoxelBoxMover，它可能在块状世界中表现得更好。

-   [Material](https://docs.godotengine.org/en/stable/classes/class_material.html) **material\_override**  
    Materialmaterial\_override
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **max\_view\_distance** = 128  
    intmax\_view\_distance = 128
    

Sets the maximum distance this terrain can support. If a [VoxelViewer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelViewer/) requests more, it will be clamped.  
设置此地形可以支持的最大距离。如果体素查看器请求更多，它将被钳制。

Note: there is an internal limit of 512 for constant LOD terrains, because going further can affect performance and memory very badly at the moment.  
注意：恒定 LOD 地形的内部限制为 512，因为进一步可能会严重影响性能和内存。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **mesh\_block\_size** = 16 intmesh\_block\_size = 16
    
-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **run\_stream\_in\_editor** = true  
    boolrun\_stream\_in\_editor = 真
    

Makes the terrain appear in the editor.  
使地形显示在编辑器中。

Important: this option will turn off automatically if you setup a script world generator. Modifying scripts while they are in use by threads causes undefined behaviors. You can still turn on this option if you need a preview, but it is strongly advised to turn it back off and wait until all generation has finished before you edit the script again.  
重要提示：如果您设置了脚本世界生成器，此选项将自动关闭。在线程使用脚本时修改脚本会导致未定义的行为。如果需要预览，您仍然可以打开此选项，但强烈建议将其关闭并等待所有生成完成，然后再再次编辑脚本。

-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **use\_gpu\_generation** = false  
    booluse\_gpu\_generation = 假

Enables GPU block generation, which can speed it up. This is only valid for generators that support it. Vulkan is required.  
启用 GPU 块生成，从而加快速度。这仅对支持它的生成器有效。Vulkan 是必需的。

## Method Descriptions 方法说明

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTerrain/#) **\_on\_area\_edited**( [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) area\_origin, [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) area\_size )  
    void\_on\_area\_edited（ Vector3i area\_origin， Vector3i area\_size ）
    
-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTerrain/#) **\_on\_data\_block\_entered**( [VoxelDataBlockEnterInfo](https://voxel-tools.readthedocs.io/en/latest/api/VoxelDataBlockEnterInfo/) info )  
    void\_on\_data\_block\_entered（ 体素数据块输入信息信息 ）
    
-   [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) **data\_block\_to\_voxel**( [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) block\_pos )  
    Vector3idata\_block\_to\_voxel（ 矢量3i block\_pos ）
    

Converts data block coordinates into voxel coordinates. Voxel coordinates of a block correspond to its lowest corner.  
将数据块坐标转换为体素坐标。块的体素坐标对应于其最低角。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **get\_data\_block\_size**( )  
    intget\_data\_block\_size（ ）
    
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
    "updated_blocks": int
}

```

-   [PackedInt32Array](https://docs.godotengine.org/en/stable/classes/class_packedint32array.html) **get\_viewer\_network\_peer\_ids\_in\_area**( [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) area\_origin, [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) area\_size )  
    PackedInt32Arrayget\_viewer\_network\_peer\_ids\_in\_area（ Vector3i area\_origin， Vector3i area\_size ）
    
-   [VoxelTool](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/) **get\_voxel\_tool**( )  
    VoxelToolget\_voxel\_tool（ ）
    

Creates an instance of [VoxelTool](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/) bound to this node, to access voxels and edition methods.  
创建绑定到此节点的体素工具实例，以访问体素和编辑方法。

You can keep it in a member variable to avoid creating one again, as long as the node still exists.  
您可以将其保留在成员变量中以避免再次创建一个成员变量，只要节点仍然存在。

-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **has\_data\_block**( [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) block\_position )  
    boolhas\_data\_block（ 矢量3i block\_position ）
    
-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **is\_area\_meshed**( [AABB](https://docs.godotengine.org/en/stable/classes/class_aabb.html) area\_in\_voxels )  
    boolis\_area\_meshed（ AABB area\_in\_voxels ）
    

Returns true if the area has been processed by meshing. It does not mean the area actually contains a mesh.  
如果区域已通过网格划分进行处理，则返回 true。这并不意味着该区域实际上包含网格。

Returns false if the area has not been processed by meshing (therefore it is unknown whethere there should be a mesh here or not).  
如果该区域尚未通过网格处理，则返回 false（因此不知道这里是否应该有网格）。

When streaming terrain, this can be used to determine if an area has fully "loaded", in case the game relies meshes or mesh colliders.  
流式传输地形时，这可用于确定某个区域是否已完全“加载”，以防游戏依赖于网格或网格碰撞体。

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTerrain/#) **save\_block**( [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) position )  
    voidsave\_block（ 矢量3i 位置 ）

Forces a specific block to be saved.  
强制保存特定块。

Note 1: all modified blocks are automatically saved before the terrain is destroyed.  
注1：在地形被破坏之前，所有修改后的方块都会自动保存。

Note 2: this will only have an effect if the stream setup on this terrain supports saving.  
注2：仅当此地形上的流设置支持保存时，这才有效。

Note 3: saving is asynchronous and won't block the game. the save may complete only a short time after you call this method.  
注意3：保存是异步的，不会阻止游戏。保存可能仅在调用此方法后很短的时间完成。

-   [VoxelSaveCompletionTracker](https://docs.godotengine.org/en/stable/classes/class_voxelsavecompletiontracker.html) **save\_modified\_blocks**( )  
    VoxelSaveCompletionTrackersave\_modified\_blocks（ ）

Forces all modified blocks to be saved.  
强制保存所有修改的块。

Note 1: all modified blocks are automatically saved before the terrain is destroyed.  
注1：在地形被破坏之前，所有修改后的方块都会自动保存。

Note 2: this will only have an effect if the stream setup on this terrain supports saving.  
注2：仅当此地形上的流设置支持保存时，这才有效。

Note 3: saving is asynchronous and won't block the game. the save may complete only a short time after you call this method.  
注意3：保存是异步的，不会阻止游戏。保存可能仅在调用此方法后很短的时间完成。

-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **try\_set\_block\_data**( [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) position, [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) voxels )  
    booltry\_set\_block\_data（ Vector3i position， VoxelBuffer 体素 ）
    
-   [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) **voxel\_to\_data\_block**( [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) voxel\_pos )  
    Vector3ivoxel\_to\_data\_block（ 矢量3 voxel\_pos ）
    

_Generated on Sep 12, 2023  
生成于 Sep 12， 2023_
