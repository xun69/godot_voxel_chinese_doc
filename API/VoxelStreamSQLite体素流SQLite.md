---
created: 2023-09-27T00:01:21 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelStreamSQLite/
author: 
---

# VoxelStreamSQLite体素流SQLite

> ## Excerpt
> Inherits: VoxelStream 继承：体素流

---
Inherits: [VoxelStream](https://voxel-tools.readthedocs.io/en/latest/api/VoxelStream/) 继承：体素流

Saves voxel data into a single SQLite database file.  
将体素数据保存到单个 SQLite 数据库文件中。

## Properties: 属性：

| Type 类型 | Name 名字 | Default 违约 |
| --- | --- | --- |
| `String` | [database\_path database\_path](https://voxel-tools.readthedocs.io/en/latest/api/VoxelStreamSQLite/#i_database_path) | "" |

## Methods: 方法：

| Return 返回 | Signature 签名 |
| --- | --- |
| [bool 布尔](https://docs.godotengine.org/en/stable/classes/class_bool.html) | [is\_key\_cache\_enabled](https://voxel-tools.readthedocs.io/en/latest/api/VoxelStreamSQLite/#i_is_key_cache_enabled) ( ) const  
is\_key\_cache\_enabled （ ） 常量 |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelStreamSQLite/#) | [set\_key\_cache\_enabled](https://voxel-tools.readthedocs.io/en/latest/api/VoxelStreamSQLite/#i_set_key_cache_enabled) ( [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) enabled )  
set\_key\_cache\_enabled （ 启用布尔值 ） |

## Property Descriptions 属性描述

-   [String](https://docs.godotengine.org/en/stable/classes/class_string.html) **database\_path** = ""  
    Stringdatabase\_path = “”

Path to the database file. `res://` and `user://` are not supported at the moment. The path can be relative to the game's executable. Directories in the path must exist. If the file does not exist, it will be created.  
数据库文件的路径。 `res://` 并且 `user://` 目前不受支持。路径可以相对于游戏的可执行文件。路径中的目录必须存在。如果该文件不存在，则将创建该文件。

## Method Descriptions 方法说明

-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **is\_key\_cache\_enabled**( )  
    boolis\_key\_cache\_enabled（ ）
    
-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelStreamSQLite/#) **set\_key\_cache\_enabled**( [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) enabled )  
    voidset\_key\_cache\_enabled（启用布尔值）
    

_Generated on Sep 12, 2023  
生成于 Sep 12， 2023_
