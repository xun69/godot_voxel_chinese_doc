---
created: 2023-10-09T22:38:26 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceLibrary/
author: 
---

# VoxelInstanceLibrary体素实例库

> ## Excerpt
> 继承：资源

---
##  体素实例库

 继承：资源

  
包含可由 VoxelInstancer 使用的模型列表，这些模型与唯一 ID 相关联。

##  方法：

|  返回 |  签名 |
| --- | --- |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceLibrary/#) |   
add\_item （ int id， VoxelInstanceLibraryItem item ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceLibrary/#) |  清除 （ ） |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) |   
find\_item\_by\_name （字符串名称） 常量 |
| [PackedInt32Array](https://docs.godotengine.org/en/stable/classes/class_packedint32array.html) |   
get\_all\_item\_ids （ ） 常量 |
| [  
体素实例库项](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceLibraryItem/) |   
get\_item （ int id ） const |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceLibrary/#) |   
remove\_item （ 整数 ID ） |

##  常量：

-   **MAX\_ID** = **65535**

##  方法说明

-     
    voidadd\_item（ int id， VoxelInstanceLibraryItem item ）
    
-    空清（ ）
    
-     
    intfind\_item\_by\_name（ 字符串名称 ）
    
-     
    PackedInt32Arrayget\_all\_item\_ids（ ）
    
-     
    VoxelInstanceLibraryItemget\_item（ 整数 ID ）
    
-     
    voidremove\_item（ 整数 ID ）
    

_  
生成于 Oct 02， 2023_
