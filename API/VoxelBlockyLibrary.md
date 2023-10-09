# VoxelBlockyLibrary体素块库

> ## Excerpt
> 继承：体素块库库

---
##  体素块库

  
继承：体素块库库

  
包含可由VoxelMesherBlocky使用的模型列表。

##  说明：

  
提供可由 VoxelMesherBlocky 使用的模型列表。每个模型对应于体素数据中的一个 ID，并且通常从网格定义。还可以定义一些额外的属性，例如相邻体素如何剔除边，或者体素引擎的某些功能如何处理这些属性。

  
如果从代码创建此库，则需要在最后使用 VoxelBlockyLibraryBase.bake 函数对其进行烘焙。

  
第一个模型（索引 0）通常用于“空气”或“空”。

##  属性：

|  类型 |  名字 |  违约 |
| --- | --- | --- |
| `VoxelBlockyModel[]` |  [模型](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyLibrary/#i_models) | \[\] |

##  方法：

|  返回 |  签名 |
| --- | --- |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) |   
add\_model （ 体素块模型 \_unnamed\_arg0 ） |
|  [体素块模型](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModel/) |   
get\_model （ int index ） const |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) |   
get\_model\_index\_from\_resource\_name （字符串名称） 常量 |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) |   
get\_voxel\_index\_from\_name （字符串名称） 常量 |

##  属性描述

-     
    体素块模型\[\]模型 = \[\]

  
所有模型的数组。每个模型的索引对应于体素数据的 TYPE 通道中表示它们的值。

##  方法说明

-     
    intadd\_model（体素块模型\_unnamed\_arg0）

  
将模型添加到库中。返回其索引，该索引将是表示它的体素的值。

-     
    VoxelBlockyModelget\_model（ 整数 ）

  
从模型的索引中获取模型。

-     
    intget\_model\_index\_from\_resource\_name（ 字符串名称 ）

  
查找具有指定资源名称的第一个模型的索引。如果未找到，则返回 `null` 。

-     
    intget\_voxel\_index\_from\_name（ 字符串名称 ）

  
查找具有指定资源名称的第一个模型的索引。如果未找到，则返回 `null` 。

_  
生成于 Oct 02， 2023_
