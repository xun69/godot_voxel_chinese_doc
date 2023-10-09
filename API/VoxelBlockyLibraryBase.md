# VoxelBlockyLibraryBase体素块库库

> ## Excerpt
> 继承：资源

---
##  体素块库库

 继承：资源

  
继承者：VoxelBlockyLibrary，VoxelBlockyTypeLibrary

  
包含可由VoxelMesherBlocky使用的模型列表。

##  说明：

  
VoxelMesherBlocky使用的模型必须先烘焙，然后才能在运行时有效使用。此过程发生的方式取决于此类的实现。它可以是模型的简单列表，也可以是生成变体模型的高级类型的列表。有关详细信息，请查看子类。

##  属性：

|  类型 |  名字 |  违约 |
| --- | --- | --- |
| `bool` | [bake\_tangents](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyLibraryBase/#i_bake_tangents) |  真 |

##  方法：

|  返回 |  签名 |
| --- | --- |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyLibraryBase/#) |  烘烤 （ ） |
|  [材料\[\]](https://docs.godotengine.org/en/stable/classes/class_material[].html) |   
get\_materials （ ） 常量 |

##  常量：

-   **MAX\_MODELS** = **65536**

##  属性描述

-     
    boolbake\_tangents = 真

  
如果需要体素上的法线映射，请启用此选项。如果您不需要它，禁用可以减少内存使用量并略微提高速度。

##  方法说明

-    虚空烘焙（ ）

  
烘焙库。优化模型数据，以便在生成体素网格时更有效地组合它们。

-     
    材料\[\]get\_materials（ ）

  
获取在库的所有模型中找到的所有不同材质的列表。

  
请注意，如果至少一个非空模型没有材质，则此列表中将有一个 `null` 条目表示“默认材质”。

_  
生成于 Oct 02， 2023_
