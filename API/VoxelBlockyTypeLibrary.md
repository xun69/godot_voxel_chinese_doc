# VoxelBlockyTypeLibrary体素块类型库

> ## Excerpt
> 继承：体素块库库

---
##  体素块类型库

  
继承：体素块库库

 警告

  
此类标记为实验性。在未来的版本中，它可能会发生变化或删除。自行决定使用。

##  属性：

|  类型 |  名字 |  违约 |
| --- | --- | --- |
| `PackedStringArray` | [\_id\_map\_data](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyTypeLibrary/#i__id_map_data) |  PackedStringArray（） |
| `VoxelBlockyType[]` |  [类型](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyTypeLibrary/#i_types) | \[\] |

##  方法：

|  返回 |  签名 |
| --- | --- |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) |   
get\_model\_index\_default （字符串名称 type\_name ） 常量 |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) |   
get\_model\_index\_single\_attribute （字符串名称type\_name，变体attrib\_value） const |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) |   
get\_model\_index\_with\_attributes （ 字符串名称 type\_name， 字典 attribs\_dict ） 常量 |
|  [体素块类型](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyType/) |   
get\_type\_from\_name （ 字符串名称 type\_name ） 常量 |
|  [数组](https://docs.godotengine.org/en/stable/classes/class_array.html) |   
get\_type\_name\_and\_attributes\_from\_model\_index （ int model\_index ） const |
|  [布尔](https://docs.godotengine.org/en/stable/classes/class_bool.html) |   
load\_id\_map\_from\_json （ 字符串 json ） |
|  [布尔](https://docs.godotengine.org/en/stable/classes/class_bool.html) |   
load\_id\_map\_from\_string\_array （ PackedStringArray str\_array ） |
|  [字符串](https://docs.godotengine.org/en/stable/classes/class_string.html) |   
serialize\_id\_map\_to\_json （ ） 常量 |
| [PackedStringArray](https://docs.godotengine.org/en/stable/classes/class_packedstringarray.html) |   
serialize\_id\_map\_to\_string\_array （ ） 常量 |

##  属性描述

-     
    PackedStringArray\_id\_map\_data = PackedStringArray（）
    
-     
    体素块类型\[\]类型 = \[\]
    

##  方法说明

-     
    intget\_model\_index\_default（ 字符串名称 type\_name ）
    
-     
    intget\_model\_index\_single\_attribute（ 字符串名称 type\_name，变体 attrib\_value ）
    
-     
    intget\_model\_index\_with\_attributes（ 字符串名称 type\_name， 字典 attribs\_dict ）
    
-     
    VoxelBlockyTypeget\_type\_from\_name（ 字符串名称 type\_name ）
    
-     
    Arrayget\_type\_name\_and\_attributes\_from\_model\_index（ int model\_index ）
    
-     
    boolload\_id\_map\_from\_json（ 字符串 json ）
    
-     
    boolload\_id\_map\_from\_string\_array（ 打包字符串数组 str\_array ）
    
-     
    Stringserialize\_id\_map\_to\_json（ ）
    
-     
    PackedStringArrayserialize\_id\_map\_to\_string\_array（ ）
    

_  
生成于 Oct 02， 2023_
