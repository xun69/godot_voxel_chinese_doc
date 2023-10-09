---
created: 2023-10-09T22:38:26 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelStreamSQLite/
author: 
---

# VoxelStreamSQLite体素流SQLite

> ## Excerpt
> 继承：体素流

---
-   [](https://voxel-tools.readthedocs.io/en/latest/)
-   Scripting API
-   VoxelStreamSQLite

___

 继承：体素流

  
将体素数据保存到单个 SQLite 数据库文件中。

##  属性：

|  类型 |  名字 |  违约 |
| --- | --- | --- |
| `String` | [database\_path](https://voxel-tools.readthedocs.io/en/latest/api/VoxelStreamSQLite/#i_database_path) | "" |

##  方法：

|  返回 |  签名 |
| --- | --- |
|  [布尔](https://docs.godotengine.org/en/stable/classes/class_bool.html) |   
is\_key\_cache\_enabled （ ） 常量 |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelStreamSQLite/#) |   
set\_key\_cache\_enabled （ 启用布尔值 ） |

##  属性描述

-     
    Stringdatabase\_path = “”

  
数据库文件的路径。 `res://` 并且 `user://` 目前不受支持。路径可以相对于游戏的可执行文件。路径中的目录必须存在。如果该文件不存在，则将创建该文件。

##  方法说明

-     
    boolis\_key\_cache\_enabled（ ）
    
-     
    voidset\_key\_cache\_enabled（启用布尔值）
    

_  
生成于 Oct 02， 2023_
