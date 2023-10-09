---
created: 2023-10-09T22:38:26 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/
author: 
---

# VoxelGraphFunction体素图函数

> ## Excerpt
> 继承：资源

---
##  体素图函数

 继承：资源

  
用于生成或处理体素的图形。

##  说明：

  
包含一个图形，该图形可用于生成体素数据（用作生成器的主要功能时），或可重用于其他图形（如子图形）。

  
目前，此类仅存储图形，无法自行运行实际处理。要使用它生成体素，请参阅体素生成器图。

##  属性：

|  类型 |  名字 |  违约 |
| --- | --- | --- |
| `Array` | [input\_definitions](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#i_input_definitions) | \[\] |
| `Array` | [output\_definitions](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#i_output_definitions) | \[\] |

##  方法：

|  返回 |  签名 |
| --- | --- |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#) |   
add\_connection （ int src\_node\_id， int src\_port\_index， int dst\_node\_id， int dst\_port\_index ） |
|  [布尔](https://docs.godotengine.org/en/stable/classes/class_bool.html) |   
can\_connect （ int src\_node\_id， int src\_port\_index， int dst\_node\_id， int dst\_port\_index ） const |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#) |  清除 （ ） |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) |   
create\_function\_node （ VoxelGraphFunction 函数， Vector2 position， int id=0 ） |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) |   
create\_node （ int type\_id， 矢量 2 位置， int id=0 ） |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) |   
find\_node\_by\_name （ 字符串名称 ） 常量 |
|  [数组](https://docs.godotengine.org/en/stable/classes/class_array.html) |   
get\_connections （ ） 常量 |
|  [变体](https://docs.godotengine.org/en/stable/classes/class_variant.html) |   
get\_node\_default\_input （ int node\_id， int input\_index ） const |
|  [布尔](https://docs.godotengine.org/en/stable/classes/class_bool.html) |   
get\_node\_default\_inputs\_autoconnect （ int node\_id ） const |
|  [矢量2](https://docs.godotengine.org/en/stable/classes/class_vector2.html) |   
get\_node\_gui\_position （ int node\_id ） const |
|  [矢量2](https://docs.godotengine.org/en/stable/classes/class_vector2.html) |   
get\_node\_gui\_size （ int node\_id ） const |
| [PackedInt32Array](https://docs.godotengine.org/en/stable/classes/class_packedint32array.html) |   
get\_node\_ids （ ） 常量 |
|  [字符串名称](https://docs.godotengine.org/en/stable/classes/class_stringname.html) |   
get\_node\_name （ int node\_id ） const |
|  [变体](https://docs.godotengine.org/en/stable/classes/class_variant.html) |   
get\_node\_param （ int node\_id， int param\_index ） const |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) |   
get\_node\_type\_count （ ） 常量 |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) |   
get\_node\_type\_id （ int node\_id ） const |
|  [字典](https://docs.godotengine.org/en/stable/classes/class_dictionary.html) |   
get\_node\_type\_info （ int type\_id ） const |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#) |   
paste\_graph\_with\_pre\_generated\_ids （ VoxelGraphFunction graph， PackedInt32Array node\_ids， Vector2 gui\_offset ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#) |   
remove\_connection （ int src\_node\_id， int src\_port\_index， int dst\_node\_id， int dst\_port\_index ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#) |   
remove\_node （ 国际 node\_id ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#) |   
set\_expression\_node\_inputs （ int node\_id， 打包字符串数组名称 ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#) |   
set\_node\_default\_input （ int node\_id， int input\_index， 变量值 ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#) |   
set\_node\_default\_inputs\_autoconnect （ int node\_id， bool 启用 ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#) |   
set\_node\_gui\_position （ int node\_id， 矢量 2 位置 ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#) |   
set\_node\_gui\_size （ int node\_id， 矢量 2 大小 ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#) |   
set\_node\_name （ int node\_id， 字符串名称 ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#) |   
set\_node\_param （ int node\_id， int param\_index， 变量值 ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#) |   
set\_node\_param\_null （ int node\_id， int param\_index ） |

##  信号：

-    编译（ ）

  
在图形完成编译后发出，即使编译失败也是如此。

-     
    node\_name\_changed（ int node\_id ）

##  枚举：

 枚举节点类型ID：

-   **NODE\_CONSTANT** = **0**
-   **NODE\_INPUT\_X** = **1**
-   **NODE\_INPUT\_Y** = **2**
-   **NODE\_INPUT\_Z** = **3**
-   **NODE\_OUTPUT\_SDF** = **4**
-   **NODE\_CUSTOM\_INPUT** = **54**
-   **NODE\_CUSTOM\_OUTPUT** = **55**
-   **NODE\_ADD** = **5**
-   **NODE\_SUBTRACT** = **6**
-   **NODE\_MULTIPLY** = **7**
-   **NODE\_DIVIDE** = **8**
-   **NODE\_SIN** = **9**
-   **NODE\_FLOOR** = **10**
-   **NODE\_ABS** = **11**
-   **NODE\_SQRT** = **12**
-   **NODE\_FRACT** = **13**
-   **NODE\_STEPIFY** = **14**
-   **NODE\_WRAP** = **15**
-   **NODE\_MIN** = **16**
-   **NODE\_MAX** = **17**
-   **NODE\_DISTANCE\_2D** = **18**
-   **NODE\_DISTANCE\_3D** = **19**
-   **NODE\_CLAMP** = **20**
-   **NODE\_MIX** = **22**
-   **NODE\_REMAP** = **23**
-   **NODE\_SMOOTHSTEP** = **24**
-   **NODE\_CURVE** = **25**
-   **NODE\_SELECT** = **26**
-   **NODE\_NOISE\_2D** = **27**
-   **NODE\_NOISE\_3D** = **28**
-   **NODE\_IMAGE\_2D** = **29**
-   **NODE\_SDF\_PLANE** = **30**
-   **NODE\_SDF\_BOX** = **31**
-   **NODE\_SDF\_SPHERE** = **32**
-   **NODE\_SDF\_TORUS** = **33**
-   **NODE\_SDF\_PREVIEW** = **34**
-   **NODE\_SDF\_SPHERE\_HEIGHTMAP** = **35**
-   **NODE\_SDF\_SMOOTH\_UNION** = **36**
-   **NODE\_SDF\_SMOOTH\_SUBTRACT** = **37**
-   **NODE\_NORMALIZE\_3D** = **38**
-   **NODE\_FAST\_NOISE\_2D** = **39**
-   **NODE\_FAST\_NOISE\_3D** = **40**
-   **NODE\_FAST\_NOISE\_GRADIENT\_2D** = **41**
-   **NODE\_FAST\_NOISE\_GRADIENT\_3D** = **42**
-   **NODE\_OUTPUT\_WEIGHT** = **43**
-   **NODE\_FAST\_NOISE\_2\_2D** = **45**
-   **NODE\_FAST\_NOISE\_2\_3D** = **46**
-   **NODE\_OUTPUT\_SINGLE\_TEXTURE** = **47**
-   **NODE\_EXPRESSION** = **48**
-   **NODE\_POWI** = **49**
-   **NODE\_POW** = **50**
-   **NODE\_INPUT\_SDF** = **51**
-   **NODE\_COMMENT** = **52**
-   **NODE\_FUNCTION** = **53**
-   **NODE\_RELAY** = **56**
-   **NODE\_SPOTS\_2D** = **57**
-   **NODE\_SPOTS\_3D** = **58**
-   **NODE\_TYPE\_COUNT** = **59**

##  属性描述

-   [Array](https://docs.godotengine.org/en/stable/classes/class_array.html) **input\_definitions** = \[\]
    
-   [Array](https://docs.godotengine.org/en/stable/classes/class_array.html) **output\_definitions** = \[\]
    

##  方法说明

-     
    voidadd\_connection（ int src\_node\_id， int src\_port\_index， int dst\_node\_id， int dst\_port\_index ）

  
将一个节点的输出连接到另一个节点的输入。不支持将节点连接到自身，或以可将其引导回自身的方式连接。

-     
    boolcan\_connect（ int src\_node\_id， int src\_port\_index， int dst\_node\_id， int dst\_port\_index ）

  
测试两个端口是否可以连接在一起。

-    空清（ ）

  
从图形中删除所有节点。不会清除输入和输出定义。

-     
    intcreate\_function\_node（ 体素图函数， 矢量2 位置， 整数 id=0 ）

  
基于现有图创建节点（创建“子图实例”）。

-     
    intcreate\_node（ int type\_id， Vector2 position， int id=0 ）

  
在特定视觉位置创建给定类型的图形节点。

  
该 `position` 参数不会影响图形的性能，但它有助于组织节点。

  
可以指定可选 ID。如果保留为 0，将生成 ID。

  
然后，此函数返回节点的 ID，这对于以后修改节点的其他属性可能很有用。

-     
    intfind\_node\_by\_name（ 字符串名称 ）
    
-     
    Arrayget\_connections（ ）
    
-     
    Variantget\_node\_default\_input（ int node\_id， int input\_index ）
    
-     
    boolget\_node\_default\_inputs\_autoconnect（ 国际 node\_id ）
    
-     
    Vector2get\_node\_gui\_position（ 国际 node\_id ）
    
-     
    Vector2get\_node\_gui\_size（ int node\_id ）
    
-     
    PackedInt32Arrayget\_node\_ids（ ）
    
-     
    StringNameget\_node\_name（ 国际 node\_id ）
    
-     
    Variantget\_node\_param（ int node\_id， int param\_index ）
    
-     
    intget\_node\_type\_count（ ）
    

  
获取图形系统中存在多少种类型的节点。

-     
    intget\_node\_type\_id（ int node\_id ）

  
获取图形中节点类型的 ID。

-     
    Dictionaryget\_node\_type\_info（ int type\_id ）
    
-     
    voidpaste\_graph\_with\_pre\_generated\_ids（ VoxelGraphFunction graph， PackedInt32Array node\_ids， Vector2 gui\_offset ）
    

  
将节点复制到另一个图形中，并且仅在它们之间建立连接。

  
如果节点参数中的资源没有文件路径，则会重复这些资源。

  
如果提供非零大小，则 `node_ids` 定义复制节点的 ID。否则，将生成它们。

-     
    voidremove\_connection（ int src\_node\_id， int src\_port\_index， int dst\_node\_id， int dst\_port\_index ）

  
删除图形的两个节点之间的现有连接。

-     
    voidremove\_node（ int node\_id ）

  
从图形中删除节点。

-     
    voidset\_expression\_node\_inputs（ int node\_id， PackedStringArray names ）

  
配置表达式节点的输入。 `names` 是表达式中使用的输入名称的列表。

  
`value` 现在一定是。 `float`

-     
    voidset\_node\_default\_input（ int node\_id， int input\_index， 变量值 ）
    
-     
    voidset\_node\_default\_inputs\_autoconnect（ int node\_id， bool 启用 ）
    

  
设置没有入站连接的节点输入是否将在编译图形时自动创建默认连接。

  
这仅在特定节点上可用。在其他节点上，它不起作用。

-     
    voidset\_node\_gui\_position（ int node\_id， 矢量 2 位置 ）

  
设置图形节点的可视位置，因为它将显示在编辑器中。

-     
    voidset\_node\_gui\_size（ int node\_id， 矢量 2 大小 ）
    
-     
    voidset\_node\_name（ int node\_id， 字符串名称 ）
    

  
设置节点的自定义名称。

-     
    voidset\_node\_param（ int node\_id， int param\_index， 变量值 ）
    
-     
    voidset\_node\_param\_null（ int node\_id， int param\_index ）
    

_  
生成于 Oct 02， 2023_
