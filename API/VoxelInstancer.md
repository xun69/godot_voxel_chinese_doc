---
created: 2023-10-09T22:38:26 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstancer/
author: 
---

# VoxelInstancer体素实例

> ## Excerpt
> 继承：节点3D

---
##  体素实例

 继承：节点3D

  
在体素表面的顶部生成项目。

##  说明：

  
附加到体素节点，允许在表面上生成元素。这些元素使用硬件实例化呈现，可以发生冲突，并且是持久性的。它必须是体素节点的子节点。

##  属性：

|  类型 |  名字 |  违约 |
| --- | --- | --- |
| `VoxelInstanceLibrary` |  [图书馆](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstancer/#i_library) |  |
| `int` | [up\_mode](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstancer/#i_up_mode) | 0 |

##  方法：

|  返回 |  签名 |
| --- | --- |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstancer/#) |   
debug\_dump\_as\_scene （ 字符串 fpath ） 常量 |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) |   
debug\_get\_block\_count （ ） 常量 |
|  [布尔](https://docs.godotengine.org/en/stable/classes/class_bool.html) |   
debug\_get\_draw\_flag （ int flag） const |
|  [字典](https://docs.godotengine.org/en/stable/classes/class_dictionary.html) |   
debug\_get\_instance\_counts （ ） 常量 |
|  [布尔](https://docs.godotengine.org/en/stable/classes/class_bool.html) |   
debug\_is\_draw\_enabled （ ） 常量 |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstancer/#) |   
debug\_set\_draw\_enabled （ 启用布尔值 ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstancer/#) |   
debug\_set\_draw\_flag （ int 标志，启用布尔值） |

##  枚举：

 枚举上行模式：

-   **UP\_MODE\_POSITIVE\_Y** = **0**
-   **UP\_MODE\_SPHERE** = **1**

 enum DebugDrawFlag：

-   **DEBUG\_DRAW\_ALL\_BLOCKS** = **0**
-   **DEBUG\_DRAW\_EDITED\_BLOCKS** = **1**
-   **DEBUG\_DRAW\_FLAGS\_COUNT** = **2**

##  常量：

-   **MAX\_LOD** = **8**

##  属性描述

-     
    体素实例库
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **up\_mode** = 0
    

##  方法说明

-     
    voiddebug\_dump\_as\_scene（ 字符串 fpath ）
    
-     
    intdebug\_get\_block\_count（ ）
    
-     
    booldebug\_get\_draw\_flag（ 国际标志 ）
    
-     
    Dictionarydebug\_get\_instance\_counts（ ）
    
-     
    booldebug\_is\_draw\_enabled（ ）
    
-     
    voiddebug\_set\_draw\_enabled（启用布尔值）
    
-     
    voiddebug\_set\_draw\_flag（ int 标志，启用布尔值）
    

_  
生成于 Oct 02， 2023_
