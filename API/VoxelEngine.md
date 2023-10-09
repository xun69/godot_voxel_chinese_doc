---
created: 2023-10-09T22:38:26 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelEngine/
author: 
---

# VoxelEngine体素引擎

> ## Excerpt
> 继承：对象

---
-   [](https://voxel-tools.readthedocs.io/en/latest/)
  
脚本 API 体素引擎

___

##  体素引擎

 继承：对象

  
在后台线程中保存常用设置和处理体素处理任务的单一实例。

##  方法：

|  返回 |  签名 |
| --- | --- |
|  [字典](https://docs.godotengine.org/en/stable/classes/class_dictionary.html) |   
get\_stats （ ） 常量 |

##  方法说明

-    Dictionaryget\_stats（ ）

  
获取有关共享体素处理的调试信息。

  
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

_  
生成于 Oct 02， 2023_
