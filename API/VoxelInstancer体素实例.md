---
created: 2023-09-27T00:01:21 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstancer/
author: 
---

# VoxelInstancer体素实例

> ## Excerpt
> Inherits: Node3D 继承：节点3D

---
Inherits: [Node3D](https://docs.godotengine.org/en/stable/classes/class_node3d.html) 继承：节点3D

Spawns items on top of voxel surfaces.  
在体素表面的顶部生成项目。

## Description: 说明：

Add-on to voxel nodes, allowing to spawn elements on the surface. These elements are rendered with hardware instancing, can have collisions, and also be persistent. It must be child of a voxel node.  
附加到体素节点，允许在表面上生成元素。这些元素使用硬件实例化呈现，可以发生冲突，并且是持久性的。它必须是体素节点的子节点。

## Properties: 属性：

| Type 类型 | Name 名字 | Default 违约 |
| --- | --- | --- |
| `VoxelInstanceLibrary` | [library 图书馆](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstancer/#i_library) |  |
| `int` | [up\_mode up\_mode](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstancer/#i_up_mode) | 0 |

## Methods: 方法：

| Return 返回 | Signature 签名 |
| --- | --- |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstancer/#) | [debug\_dump\_as\_scene](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstancer/#i_debug_dump_as_scene) ( [String](https://docs.godotengine.org/en/stable/classes/class_string.html) fpath ) const  
debug\_dump\_as\_scene （ 字符串 fpath ） 常量 |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) | [debug\_get\_block\_count](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstancer/#i_debug_get_block_count) ( ) const  
debug\_get\_block\_count （ ） 常量 |
| [bool 布尔](https://docs.godotengine.org/en/stable/classes/class_bool.html) | [debug\_get\_draw\_flag](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstancer/#i_debug_get_draw_flag) ( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) flag ) const  
debug\_get\_draw\_flag （ int flag） const |
| [Dictionary 字典](https://docs.godotengine.org/en/stable/classes/class_dictionary.html) | [debug\_get\_instance\_counts](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstancer/#i_debug_get_instance_counts) ( ) const  
debug\_get\_instance\_counts （ ） 常量 |
| [bool 布尔](https://docs.godotengine.org/en/stable/classes/class_bool.html) | [debug\_is\_draw\_enabled](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstancer/#i_debug_is_draw_enabled) ( ) const  
debug\_is\_draw\_enabled （ ） 常量 |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstancer/#) | [debug\_set\_draw\_enabled](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstancer/#i_debug_set_draw_enabled) ( [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) enabled )  
debug\_set\_draw\_enabled （ 启用布尔值 ） |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstancer/#) | [debug\_set\_draw\_flag](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstancer/#i_debug_set_draw_flag) ( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) flag, [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) enabled )  
debug\_set\_draw\_flag （ int 标志，启用布尔值） |

## Enumerations: 枚举：

enum **UpMode**:  枚举上行模式：

-   **UP\_MODE\_POSITIVE\_Y** = **0**
-   **UP\_MODE\_SPHERE** = **1**

enum **DebugDrawFlag**:  enum DebugDrawFlag：

-   **DEBUG\_DRAW\_ALL\_BLOCKS** = **0**
-   **DEBUG\_DRAW\_EDITED\_BLOCKS** = **1**
-   **DEBUG\_DRAW\_FLAGS\_COUNT** = **2**

## Constants: 常量：

-   **MAX\_LOD** = **8**

## Property Descriptions 属性描述

-   [VoxelInstanceLibrary](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceLibrary/) **library**  
    体素实例库
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **up\_mode** = 0 intup\_mode = 0
    

## Method Descriptions 方法说明

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstancer/#) **debug\_dump\_as\_scene**( [String](https://docs.godotengine.org/en/stable/classes/class_string.html) fpath )  
    voiddebug\_dump\_as\_scene（ 字符串 fpath ）
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **debug\_get\_block\_count**( )  
    intdebug\_get\_block\_count（ ）
    
-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **debug\_get\_draw\_flag**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) flag )  
    booldebug\_get\_draw\_flag（ 国际标志 ）
    
-   [Dictionary](https://docs.godotengine.org/en/stable/classes/class_dictionary.html) **debug\_get\_instance\_counts**( )  
    Dictionarydebug\_get\_instance\_counts（ ）
    
-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **debug\_is\_draw\_enabled**( )  
    booldebug\_is\_draw\_enabled（ ）
    
-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstancer/#) **debug\_set\_draw\_enabled**( [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) enabled )  
    voiddebug\_set\_draw\_enabled（启用布尔值）
    
-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstancer/#) **debug\_set\_draw\_flag**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) flag, [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) enabled )  
    voiddebug\_set\_draw\_flag（ int 标志，启用布尔值）
    

_Generated on Sep 12, 2023  
生成于 Sep 12， 2023_
