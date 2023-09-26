---
created: 2023-09-27T00:01:21 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelViewer/
author: 
---

# VoxelViewer体素查看器

> ## Excerpt
> Inherits: Node3D 继承：节点3D

---
Inherits: [Node3D](https://docs.godotengine.org/en/stable/classes/class_node3d.html) 继承：节点3D

Attach this as a child node of characters, so the voxel world will know where to load blocks around them.  
将其附加为字符的子节点，以便体素世界将知道在它们周围加载块的位置。

If no viewer is present in the world, nothing will generate.  
如果世界上没有观众，什么都不会产生。

## Description: 说明：

The voxel world uses the position and options of all the [VoxelViewer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelViewer/) nodes to determine where to load blocks, and prioritize updates. For example, a voxel placed 100 units away from a player will have much lower priority than the modifications that player is doing when digging in front of them.  
体素世界使用所有体素查看器节点的位置和选项来确定加载块的位置，并确定更新的优先级。例如，放置在距离玩家 100 个单位的体素的优先级将远低于玩家在他们面前挖掘时所做的修改。

## Properties: 属性：

## Methods: 方法：

| Return 返回 | Signature 签名 |
| --- | --- |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) | [get\_network\_peer\_id](https://voxel-tools.readthedocs.io/en/latest/api/VoxelViewer/#i_get_network_peer_id) ( ) const  
get\_network\_peer\_id （ ） 常量 |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelViewer/#) | [set\_network\_peer\_id](https://voxel-tools.readthedocs.io/en/latest/api/VoxelViewer/#i_set_network_peer_id) ( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) id )  
set\_network\_peer\_id （ 整数 ID ） |

## Property Descriptions 属性描述

-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **requires\_collisions** = true  
    boolrequires\_collisions = 真

If set to `true`, the engine will generate classic collision shapes around this viewer.  
如果设置为 `true` ，引擎将围绕此查看器生成经典的碰撞形状。

-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **requires\_data\_block\_notifications** = false  
    boolrequires\_data\_block\_notifications = 假
    
-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **requires\_visuals** = true  
    boolrequires\_visuals = 真
    

If set to `true`, the engine will generate meshes around this viewer. This may be enabled for the local player.  
如果设置为 `true` ，引擎将围绕此查看器生成网格。可以为本地播放器启用此功能。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **view\_distance** = 128 intview\_distance = 128

How far should voxels generate around this viewer.  
体素应在此查看器周围生成多远。

## Method Descriptions 方法说明

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **get\_network\_peer\_id**( )  
    intget\_network\_peer\_id（ ）
    
-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelViewer/#) **set\_network\_peer\_id**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) id )  
    voidset\_network\_peer\_id（ 整数 ID ）
    

_Generated on Sep 12, 2023  
生成于 Sep 12， 2023_
