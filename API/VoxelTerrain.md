---
created: 2023-10-09T22:38:26 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelTerrain/
author: 
---

# VoxelTerrain体素地形

> ## Excerpt
> 继承：体素节点

---
##  体素地形

 继承：体素节点

  
使用恒定细节水平的体素体积。

##  属性：

|  类型 |  名字 |  违约 |
| --- | --- | --- |
| `bool` | [area\_edit\_notification\_enabled](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTerrain/#i_area_edit_notification_enabled) |  假 |
| `bool` | [automatic\_loading\_enabled](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTerrain/#i_automatic_loading_enabled) |  真 |
| `bool` | [block\_enter\_notification\_enabled](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTerrain/#i_block_enter_notification_enabled) |  假 |
| `AABB` |  [边界](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTerrain/#i_bounds) |   
AABB（-5.36871e+08， -5.36871e+08， -5.36871e+08， 1.07374e+09， 1.07374e+09， 1.07374e+09） |
| `int` | [collision\_layer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTerrain/#i_collision_layer) | 1 |
| `float` | [collision\_margin](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTerrain/#i_collision_margin) | 0.04 |
| `int` | [collision\_mask](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTerrain/#i_collision_mask) | 1 |
| `bool` | [generate\_collisions](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTerrain/#i_generate_collisions) |  真 |
| `Material` | [material\_override](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTerrain/#i_material_override) |  |
| `int` | [max\_view\_distance](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTerrain/#i_max_view_distance) | 128 |
| `int` | [mesh\_block\_size](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTerrain/#i_mesh_block_size) | 16 |
| `bool` | [run\_stream\_in\_editor](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTerrain/#i_run_stream_in_editor) |  真 |
| `bool` | [use\_gpu\_generation](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTerrain/#i_use_gpu_generation) |  假 |

##  方法：

|  返回 |  签名 |
| --- | --- |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTerrain/#) |   
\_on\_area\_edited （ Vector3i area\_origin， Vector3i area\_size ） 虚拟 |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTerrain/#) |   
\_on\_data\_block\_entered （体素数据块输入信息） 虚拟 |
|  [矢量3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) |   
data\_block\_to\_voxel （ Vector3i block\_pos ） const |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) |   
get\_data\_block\_size （ ） 常量 |
|  [字典](https://docs.godotengine.org/en/stable/classes/class_dictionary.html) |   
get\_statistics （ ） 常量 |
| [PackedInt32Array](https://docs.godotengine.org/en/stable/classes/class_packedint32array.html) |   
get\_viewer\_network\_peer\_ids\_in\_area （ Vector3i area\_origin， Vector3i area\_size ） const |
|  [体素工具](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/) |  get\_voxel\_tool （ ） |
|  [布尔](https://docs.godotengine.org/en/stable/classes/class_bool.html) |   
has\_data\_block （ Vector3i block\_position ） const |
|  [布尔](https://docs.godotengine.org/en/stable/classes/class_bool.html) |   
is\_area\_meshed （ AABB area\_in\_voxels ） 常量 |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTerrain/#) |   
save\_block （ 矢量3i 位置 ） |
| [  
体素保存完成跟踪器](https://docs.godotengine.org/en/stable/classes/class_voxelsavecompletiontracker.html) |   
save\_modified\_blocks （ ） |
|  [布尔](https://docs.godotengine.org/en/stable/classes/class_bool.html) |   
try\_set\_block\_data（Vector3i 位置，体素缓冲区体素） |
|  [矢量3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) |   
voxel\_to\_data\_block （ 矢量3 voxel\_pos ） 常量 |

##  信号：

-     
    block\_loaded（ 矢量3i 位置 ）

  
从流加载新数据块时发出。这可能在网格或碰撞体可用之前发生。

-     
    block\_unloaded（ 矢量3i 位置 ）

  
在由于超出视图距离而卸载数据块时发出。

-     
    mesh\_block\_entered（ 矢量3i 位置 ）

  
当网格块收到自添加到查看器范围以来的首次更新时发出。这与网格是否为空无关。它跟踪使用VoxelTerrain.is\_area\_meshed获得的相同状态的变化。

-     
    mesh\_block\_exited（ 矢量3i 位置 ）

  
在卸载网格块时发出。它是VoxelTerrain.mesh\_block\_entered的对应物。

##  属性描述

-     
    boolarea\_edit\_notification\_enabled = 假
    
-     
    boolautomatic\_loading\_enabled = 真
    
-     
    boolblock\_enter\_notification\_enabled = 假
    
-     
    AABBbounds = AABB（-5.36871e+08， -5.36871e+08， -5.36871e+08， 1.07374e+09， 1.07374e+09， 1.07374e+09）
    

  
定义允许地形具有体素的边界。如果使用无限世界生成器，则块将仅在此区域内生成。外面的所有东西都将空置。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **collision\_layer** = 1
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **collision\_margin** = 0.04
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **collision\_mask** = 1
    
-     
    boolgenerate\_collisions = 真
    

  
支持使用经典物理引擎生成碰撞形状。如果您需要逼真或非平凡的碰撞或物理，请使用此功能。

  
注意 1：您还需要 VoxelViewer 来请求冲突，否则它们不会生成。

  
注2：如果你需要简单的Minecraft/AABB物理，你可以使用VoxelBoxMover，它可能在块状世界中表现得更好。

-   [Material](https://docs.godotengine.org/en/stable/classes/class_material.html) **material\_override**
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **max\_view\_distance** = 128
    

  
设置此地形可以支持的最大距离。如果体素查看器请求更多，它将被钳制。

  
注意：恒定 LOD 地形的内部限制为 512，因为进一步可能会严重影响性能和内存。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **mesh\_block\_size** = 16
    
-     
    boolrun\_stream\_in\_editor = 真
    

  
使地形显示在编辑器中。

  
重要提示：如果您设置了脚本世界生成器，此选项将自动关闭。在线程使用脚本时修改脚本会导致未定义的行为。如果需要预览，您仍然可以打开此选项，但强烈建议将其关闭并等待所有生成完成，然后再再次编辑脚本。

-     
    booluse\_gpu\_generation = 假

  
启用 GPU 块生成，从而加快速度。这仅对支持它的生成器有效。Vulkan 是必需的。

##  方法说明

-     
    void\_on\_area\_edited（ Vector3i area\_origin， Vector3i area\_size ）
    
-     
    void\_on\_data\_block\_entered（ 体素数据块输入信息信息 ）
    
-     
    Vector3idata\_block\_to\_voxel（ 矢量3i block\_pos ）
    

  
将数据块坐标转换为体素坐标。块的体素坐标对应于其最低角。

-     
    intget\_data\_block\_size（ ）
    
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
    "updated_blocks": int
}
```

-     
    PackedInt32Arrayget\_viewer\_network\_peer\_ids\_in\_area（ Vector3i area\_origin， Vector3i area\_size ）
    
-     
    VoxelToolget\_voxel\_tool（ ）
    

  
创建绑定到此节点的体素工具实例，以访问体素和编辑方法。

  
您可以将其保留在成员变量中以避免再次创建一个成员变量，只要节点仍然存在。

-     
    boolhas\_data\_block（ 矢量3i block\_position ）
    
-     
    boolis\_area\_meshed（ AABB area\_in\_voxels ）
    

  
如果区域已通过网格划分进行处理，则返回 true。这并不意味着该区域实际上包含网格。

  
如果该区域尚未通过网格处理，则返回 false（因此不知道这里是否应该有网格）。

  
流式传输地形时，这可用于确定某个区域是否已完全“加载”，以防游戏依赖于网格或网格碰撞体。

-     
    voidsave\_block（ 矢量3i 位置 ）

  
强制保存特定块。

  
注1：在地形被破坏之前，所有修改后的方块都会自动保存。

  
注2：仅当此地形上的流设置支持保存时，这才有效。

  
注意3：保存是异步的，不会阻止游戏。保存可能仅在调用此方法后很短的时间完成。

-     
    VoxelSaveCompletionTrackersave\_modified\_blocks（ ）

  
强制保存所有修改的块。

  
注1：在地形被破坏之前，所有修改后的方块都会自动保存。

  
注2：仅当此地形上的流设置支持保存时，这才有效。

  
注意3：保存是异步的，不会阻止游戏。保存可能仅在调用此方法后很短的时间完成。

-     
    booltry\_set\_block\_data（ Vector3i position， VoxelBuffer 体素 ）
    
-     
    Vector3ivoxel\_to\_data\_block（ 矢量3 voxel\_pos ）
    

_  
生成于 Oct 02， 2023_
