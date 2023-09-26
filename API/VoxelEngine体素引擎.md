---
created: 2023-09-27T00:01:21 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelEngine/
author: 
---

# VoxelEngine体素引擎

> ## Excerpt
> Inherits: Object 继承：对象

---
Inherits: [Object](https://docs.godotengine.org/en/stable/classes/class_object.html) 继承：对象

Singleton holding common settings and handling voxel processing tasks in background threads.  
在后台线程中保存常用设置和处理体素处理任务的单一实例。

## Methods: 方法：

## Method Descriptions 方法说明

-   [Dictionary](https://docs.godotengine.org/en/stable/classes/class_dictionary.html) **get\_stats**( )  Dictionaryget\_stats（ ）

Gets debug information about shared voxel processing.  
获取有关共享体素处理的调试信息。

The returned dictionary has the following structure:  
返回的字典具有以下结构：

```
{
    "thread_pools": {
        "general": {
            "tasks": int,
            "active_threads": int,
            "thread_count": int
        }
    },
    "tasks": {
        "streaming": int,
        "meshing": int,
        "generation": int,
        "main_thread": int
    },
    "memory_pools": {
        "voxel_used": int,
        "voxel_total": int,
        "block_count": int
    }
}

```

_Generated on Sep 12, 2023  
生成于 Sep 12， 2023_
