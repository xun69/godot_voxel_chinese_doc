---
created: 2023-09-27T00:01:21 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyTypeLibrary/
author: 
---

# VoxelBlockyTypeLibrary体素块类型库

> ## Excerpt
> Inherits: VoxelBlockyLibraryBase继承：体素块库库

---
Inherits: [VoxelBlockyLibraryBase](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyLibraryBase/)  
继承：体素块库库

Warning 警告

This class is marked as experimental. It is subject to likely change or possible removal in future versions. Use at your own discretion.  
此类标记为实验性。在未来的版本中，它可能会发生变化或删除。自行决定使用。

## Properties: 属性：

| Type 类型 | Name 名字 | Default 违约 |
| --- | --- | --- |
| `PackedStringArray` | [\_id\_map\_data \_id\_map\_data](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyTypeLibrary/#i__id_map_data) | PackedStringArray() PackedStringArray（） |
| `VoxelBlockyType[]` | [types 类型](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyTypeLibrary/#i_types) | \[\] |

## Methods: 方法：

## Property Descriptions 属性描述

-   [PackedStringArray](https://docs.godotengine.org/en/stable/classes/class_packedstringarray.html) **\_id\_map\_data** = PackedStringArray()  
    PackedStringArray\_id\_map\_data = PackedStringArray（）
    
-   [VoxelBlockyType\[\]](https://docs.godotengine.org/en/stable/classes/class_voxelblockytype[].html) **types** = \[\]  
    体素块类型\[\]类型 = \[\]
    

## Method Descriptions 方法说明

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **get\_model\_index\_default**( [StringName](https://docs.godotengine.org/en/stable/classes/class_stringname.html) type\_name )  
    intget\_model\_index\_default（ 字符串名称 type\_name ）
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **get\_model\_index\_single\_attribute**( [StringName](https://docs.godotengine.org/en/stable/classes/class_stringname.html) type\_name, [Variant](https://docs.godotengine.org/en/stable/classes/class_variant.html) attrib\_value )  
    intget\_model\_index\_single\_attribute（ 字符串名称 type\_name，变体 attrib\_value ）
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **get\_model\_index\_with\_attributes**( [StringName](https://docs.godotengine.org/en/stable/classes/class_stringname.html) type\_name, [Dictionary](https://docs.godotengine.org/en/stable/classes/class_dictionary.html) attribs\_dict )  
    intget\_model\_index\_with\_attributes（ 字符串名称 type\_name， 字典 attribs\_dict ）
    
-   [VoxelBlockyType](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyType/) **get\_type\_from\_name**( [StringName](https://docs.godotengine.org/en/stable/classes/class_stringname.html) type\_name )  
    VoxelBlockyTypeget\_type\_from\_name（ 字符串名称 type\_name ）
    
-   [Array](https://docs.godotengine.org/en/stable/classes/class_array.html) **get\_type\_name\_and\_attributes\_from\_model\_index**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) model\_index )  
    Arrayget\_type\_name\_and\_attributes\_from\_model\_index（ int model\_index ）
    
-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **load\_id\_map\_from\_json**( [String](https://docs.godotengine.org/en/stable/classes/class_string.html) json )  
    boolload\_id\_map\_from\_json（ 字符串 json ）
    
-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **load\_id\_map\_from\_string\_array**( [PackedStringArray](https://docs.godotengine.org/en/stable/classes/class_packedstringarray.html) str\_array )  
    boolload\_id\_map\_from\_string\_array（ 打包字符串数组 str\_array ）
    
-   [String](https://docs.godotengine.org/en/stable/classes/class_string.html) **serialize\_id\_map\_to\_json**( )  
    Stringserialize\_id\_map\_to\_json（ ）
    
-   [PackedStringArray](https://docs.godotengine.org/en/stable/classes/class_packedstringarray.html) **serialize\_id\_map\_to\_string\_array**( )  
    PackedStringArrayserialize\_id\_map\_to\_string\_array（ ）
    

_Generated on Sep 12, 2023  
生成于 Sep 12， 2023_
