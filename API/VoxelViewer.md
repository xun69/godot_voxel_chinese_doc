---
created: 2023-10-09T22:38:26 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelViewer/
author: 
---

# VoxelViewer体素查看器

> ## Excerpt
> 继承：节点3D

---
##  体素查看器

 继承：节点3D

  
将其附加为字符的子节点，以便体素世界将知道在它们周围加载块的位置。

  
如果世界上没有观众，什么都不会产生。

##  说明：

  
体素世界使用所有体素查看器节点的位置和选项来确定加载块的位置，并确定更新的优先级。例如，放置在距离玩家 100 个单位的体素的优先级将远低于玩家在他们面前挖掘时所做的修改。

##  属性：

|  类型 |  名字 |  违约 |
| --- | --- | --- |
| `bool` | [requires\_collisions](https://voxel-tools.readthedocs.io/en/latest/api/VoxelViewer/#i_requires_collisions) |  真 |
| `bool` | [requires\_data\_block\_notifications](https://voxel-tools.readthedocs.io/en/latest/api/VoxelViewer/#i_requires_data_block_notifications) |  假 |
| `bool` | [requires\_visuals](https://voxel-tools.readthedocs.io/en/latest/api/VoxelViewer/#i_requires_visuals) |  真 |
| `int` | [view\_distance](https://voxel-tools.readthedocs.io/en/latest/api/VoxelViewer/#i_view_distance) | 128 |

##  方法：

|  返回 |  签名 |
| --- | --- |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) |   
get\_network\_peer\_id （ ） 常量 |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelViewer/#) |   
set\_network\_peer\_id （ 整数 ID ） |

##  属性描述

-     
    boolrequires\_collisions = 真

  
如果设置为 `true` ，引擎将围绕此查看器生成经典的碰撞形状。

-     
    boolrequires\_data\_block\_notifications = 假
    
-     
    boolrequires\_visuals = 真
    

  
如果设置为 `true` ，引擎将围绕此查看器生成网格。可以为本地播放器启用此功能。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **view\_distance** = 128

  
体素应在此查看器周围生成多远。

##  方法说明

-     
    intget\_network\_peer\_id（ ）
    
-     
    voidset\_network\_peer\_id（ 整数 ID ）
    

_  
生成于 Oct 02， 2023_
