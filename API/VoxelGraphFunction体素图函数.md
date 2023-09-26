---
created: 2023-09-27T00:01:21 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/
author: 
---

# VoxelGraphFunction体素图函数

> ## Excerpt
> Inherits: Resource 继承：资源

---
Inherits: [Resource](https://docs.godotengine.org/en/stable/classes/class_resource.html) 继承：资源

Graph for generating or processing voxels.  
用于生成或处理体素的图形。

## Description: 说明：

Contains a graph that can be used to generate voxel data (when used as main function of a generator), or to be re-used into other graphs (like a sub-graph).  
包含一个图形，该图形可用于生成体素数据（用作生成器的主要功能时），或可重用于其他图形（如子图形）。

Currently this class only stores a graph, it cannot run actual processing on its own. To generate voxels with it, see [VoxelGeneratorGraph](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorGraph/).  
目前，此类仅存储图形，无法自行运行实际处理。要使用它生成体素，请参阅体素生成器图。

## Properties: 属性：

| Type 类型 | Name 名字 | Default 违约 |
| --- | --- | --- |
| `Array` | [input\_definitions input\_definitions](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#i_input_definitions) | \[\] |
| `Array` | [output\_definitions output\_definitions](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#i_output_definitions) | \[\] |

## Methods: 方法：

| Return 返回 | Signature 签名 |
| --- | --- |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#) | [add\_connection](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#i_add_connection) ( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) src\_node\_id, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) src\_port\_index, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) dst\_node\_id, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) dst\_port\_index )  
add\_connection （ int src\_node\_id， int src\_port\_index， int dst\_node\_id， int dst\_port\_index ） |
| [bool 布尔](https://docs.godotengine.org/en/stable/classes/class_bool.html) | [can\_connect](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#i_can_connect) ( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) src\_node\_id, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) src\_port\_index, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) dst\_node\_id, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) dst\_port\_index ) const  
can\_connect （ int src\_node\_id， int src\_port\_index， int dst\_node\_id， int dst\_port\_index ） const |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#) | [clear](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#i_clear) ( ) 清除 （ ） |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) | [create\_function\_node](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#i_create_function_node) ( [VoxelGraphFunction](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/) function, [Vector2](https://docs.godotengine.org/en/stable/classes/class_vector2.html) position, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) id=0 )  
create\_function\_node （ VoxelGraphFunction 函数， Vector2 position， int id=0 ） |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) | [create\_node](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#i_create_node) ( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) type\_id, [Vector2](https://docs.godotengine.org/en/stable/classes/class_vector2.html) position, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) id=0 )  
create\_node （ int type\_id， 矢量 2 位置， int id=0 ） |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) | [find\_node\_by\_name](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#i_find_node_by_name) ( [StringName](https://docs.godotengine.org/en/stable/classes/class_stringname.html) name ) const  
find\_node\_by\_name （ 字符串名称 ） 常量 |
| [Array 数组](https://docs.godotengine.org/en/stable/classes/class_array.html) | [get\_connections](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#i_get_connections) ( ) const  
get\_connections （ ） 常量 |
| [Variant 变体](https://docs.godotengine.org/en/stable/classes/class_variant.html) | [get\_node\_default\_input](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#i_get_node_default_input) ( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) node\_id, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) input\_index ) const  
get\_node\_default\_input （ int node\_id， int input\_index ） const |
| [bool 布尔](https://docs.godotengine.org/en/stable/classes/class_bool.html) | [get\_node\_default\_inputs\_autoconnect](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#i_get_node_default_inputs_autoconnect) ( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) node\_id ) const  
get\_node\_default\_inputs\_autoconnect （ int node\_id ） const |
| [Vector2 矢量2](https://docs.godotengine.org/en/stable/classes/class_vector2.html) | [get\_node\_gui\_position](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#i_get_node_gui_position) ( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) node\_id ) const  
get\_node\_gui\_position （ int node\_id ） const |
| [Vector2 矢量2](https://docs.godotengine.org/en/stable/classes/class_vector2.html) | [get\_node\_gui\_size](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#i_get_node_gui_size) ( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) node\_id ) const  
get\_node\_gui\_size （ int node\_id ） const |
| [PackedInt32Array PackedInt32Array](https://docs.godotengine.org/en/stable/classes/class_packedint32array.html) | [get\_node\_ids](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#i_get_node_ids) ( ) const  
get\_node\_ids （ ） 常量 |
| [StringName 字符串名称](https://docs.godotengine.org/en/stable/classes/class_stringname.html) | [get\_node\_name](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#i_get_node_name) ( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) node\_id ) const  
get\_node\_name （ int node\_id ） const |
| [Variant 变体](https://docs.godotengine.org/en/stable/classes/class_variant.html) | [get\_node\_param](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#i_get_node_param) ( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) node\_id, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) param\_index ) const  
get\_node\_param （ int node\_id， int param\_index ） const |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) | [get\_node\_type\_count](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#i_get_node_type_count) ( ) const  
get\_node\_type\_count （ ） 常量 |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) | [get\_node\_type\_id](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#i_get_node_type_id) ( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) node\_id ) const  
get\_node\_type\_id （ int node\_id ） const |
| [Dictionary 字典](https://docs.godotengine.org/en/stable/classes/class_dictionary.html) | [get\_node\_type\_info](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#i_get_node_type_info) ( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) type\_id ) const  
get\_node\_type\_info （ int type\_id ） const |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#) | [paste\_graph\_with\_pre\_generated\_ids](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#i_paste_graph_with_pre_generated_ids) ( [VoxelGraphFunction](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/) graph, [PackedInt32Array](https://docs.godotengine.org/en/stable/classes/class_packedint32array.html) node\_ids, [Vector2](https://docs.godotengine.org/en/stable/classes/class_vector2.html) gui\_offset )  
paste\_graph\_with\_pre\_generated\_ids （ VoxelGraphFunction graph， PackedInt32Array node\_ids， Vector2 gui\_offset ） |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#) | [remove\_connection](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#i_remove_connection) ( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) src\_node\_id, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) src\_port\_index, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) dst\_node\_id, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) dst\_port\_index )  
remove\_connection （ int src\_node\_id， int src\_port\_index， int dst\_node\_id， int dst\_port\_index ） |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#) | [remove\_node](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#i_remove_node) ( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) node\_id )  
remove\_node （ 国际 node\_id ） |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#) | [set\_expression\_node\_inputs](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#i_set_expression_node_inputs) ( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) node\_id, [PackedStringArray](https://docs.godotengine.org/en/stable/classes/class_packedstringarray.html) names )  
set\_expression\_node\_inputs （ int node\_id， 打包字符串数组名称 ） |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#) | [set\_node\_default\_input](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#i_set_node_default_input) ( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) node\_id, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) input\_index, [Variant](https://docs.godotengine.org/en/stable/classes/class_variant.html) value )  
set\_node\_default\_input （ int node\_id， int input\_index， 变量值 ） |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#) | [set\_node\_default\_inputs\_autoconnect](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#i_set_node_default_inputs_autoconnect) ( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) node\_id, [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) enabled )  
set\_node\_default\_inputs\_autoconnect （ int node\_id， bool 启用 ） |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#) | [set\_node\_gui\_position](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#i_set_node_gui_position) ( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) node\_id, [Vector2](https://docs.godotengine.org/en/stable/classes/class_vector2.html) position )  
set\_node\_gui\_position （ int node\_id， 矢量 2 位置 ） |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#) | [set\_node\_gui\_size](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#i_set_node_gui_size) ( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) node\_id, [Vector2](https://docs.godotengine.org/en/stable/classes/class_vector2.html) size )  
set\_node\_gui\_size （ int node\_id， 矢量 2 大小 ） |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#) | [set\_node\_name](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#i_set_node_name) ( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) node\_id, [StringName](https://docs.godotengine.org/en/stable/classes/class_stringname.html) name )  
set\_node\_name （ int node\_id， 字符串名称 ） |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#) | [set\_node\_param](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#i_set_node_param) ( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) node\_id, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) param\_index, [Variant](https://docs.godotengine.org/en/stable/classes/class_variant.html) value )  
set\_node\_param （ int node\_id， int param\_index， 变量值 ） |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#) | [set\_node\_param\_null](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#i_set_node_param_null) ( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) node\_id, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) param\_index )  
set\_node\_param\_null （ int node\_id， int param\_index ） |

## Signals: 信号：

-   compiled( )  编译（ ）

Emitted after the graph finished compiling, even if compiling failed.  
在图形完成编译后发出，即使编译失败也是如此。

-   node\_name\_changed( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) node\_id )  
    node\_name\_changed（ int node\_id ）

## Enumerations: 枚举：

enum **NodeTypeID**:  枚举节点类型ID：

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

## Property Descriptions 属性描述

-   [Array](https://docs.godotengine.org/en/stable/classes/class_array.html) **input\_definitions** = \[\]  
    Arrayinput\_definitions = \[\]
    
-   [Array](https://docs.godotengine.org/en/stable/classes/class_array.html) **output\_definitions** = \[\]  
    Arrayoutput\_definitions = \[\]
    

## Method Descriptions 方法说明

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#) **add\_connection**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) src\_node\_id, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) src\_port\_index, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) dst\_node\_id, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) dst\_port\_index )  
    voidadd\_connection（ int src\_node\_id， int src\_port\_index， int dst\_node\_id， int dst\_port\_index ）

Connects the outputs of a node to the input of another node. Connecting a node to itself, or in a way that can lead it back to itself, is not supported.  
将一个节点的输出连接到另一个节点的输入。不支持将节点连接到自身，或以可将其引导回自身的方式连接。

-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **can\_connect**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) src\_node\_id, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) src\_port\_index, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) dst\_node\_id, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) dst\_port\_index )  
    boolcan\_connect（ int src\_node\_id， int src\_port\_index， int dst\_node\_id， int dst\_port\_index ）

Tests if two ports can be connected together.  
测试两个端口是否可以连接在一起。

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#) **clear**( )  空清（ ）

Removes all nodes from the graph. Input and output definitions will not be cleared.  
从图形中删除所有节点。不会清除输入和输出定义。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **create\_function\_node**( [VoxelGraphFunction](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/) function, [Vector2](https://docs.godotengine.org/en/stable/classes/class_vector2.html) position, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) id=0 )  
    intcreate\_function\_node（ 体素图函数， 矢量2 位置， 整数 id=0 ）

Creates a node based on an existing graph (creates a "sub-graph instance").  
基于现有图创建节点（创建“子图实例”）。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **create\_node**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) type\_id, [Vector2](https://docs.godotengine.org/en/stable/classes/class_vector2.html) position, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) id=0 )  
    intcreate\_node（ int type\_id， Vector2 position， int id=0 ）

Creates a graph node of a given type at a specific visual position.  
在特定视觉位置创建给定类型的图形节点。

The `position` parameter does not affect how the graph will perform, however it helps organizing nodes.  
该 `position` 参数不会影响图形的性能，但它有助于组织节点。

An optional ID can be specified. If left to 0, the ID will be generated.  
可以指定可选 ID。如果保留为 0，将生成 ID。

This function then returns the ID of the node, which may be useful to modify other properties of the node later.  
然后，此函数返回节点的 ID，这对于以后修改节点的其他属性可能很有用。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **find\_node\_by\_name**( [StringName](https://docs.godotengine.org/en/stable/classes/class_stringname.html) name )  
    intfind\_node\_by\_name（ 字符串名称 ）
    
-   [Array](https://docs.godotengine.org/en/stable/classes/class_array.html) **get\_connections**( )  
    Arrayget\_connections（ ）
    
-   [Variant](https://docs.godotengine.org/en/stable/classes/class_variant.html) **get\_node\_default\_input**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) node\_id, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) input\_index )  
    Variantget\_node\_default\_input（ int node\_id， int input\_index ）
    
-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **get\_node\_default\_inputs\_autoconnect**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) node\_id )  
    boolget\_node\_default\_inputs\_autoconnect（ 国际 node\_id ）
    
-   [Vector2](https://docs.godotengine.org/en/stable/classes/class_vector2.html) **get\_node\_gui\_position**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) node\_id )  
    Vector2get\_node\_gui\_position（ 国际 node\_id ）
    
-   [Vector2](https://docs.godotengine.org/en/stable/classes/class_vector2.html) **get\_node\_gui\_size**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) node\_id )  
    Vector2get\_node\_gui\_size（ int node\_id ）
    
-   [PackedInt32Array](https://docs.godotengine.org/en/stable/classes/class_packedint32array.html) **get\_node\_ids**( )  
    PackedInt32Arrayget\_node\_ids（ ）
    
-   [StringName](https://docs.godotengine.org/en/stable/classes/class_stringname.html) **get\_node\_name**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) node\_id )  
    StringNameget\_node\_name（ 国际 node\_id ）
    
-   [Variant](https://docs.godotengine.org/en/stable/classes/class_variant.html) **get\_node\_param**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) node\_id, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) param\_index )  
    Variantget\_node\_param（ int node\_id， int param\_index ）
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **get\_node\_type\_count**( )  
    intget\_node\_type\_count（ ）
    

Get how many types of nodes exist in the graph system.  
获取图形系统中存在多少种类型的节点。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **get\_node\_type\_id**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) node\_id )  
    intget\_node\_type\_id（ int node\_id ）

Get the ID of the type of a node in the graph.  
获取图形中节点类型的 ID。

-   [Dictionary](https://docs.godotengine.org/en/stable/classes/class_dictionary.html) **get\_node\_type\_info**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) type\_id )  
    Dictionaryget\_node\_type\_info（ int type\_id ）
    
-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#) **paste\_graph\_with\_pre\_generated\_ids**( [VoxelGraphFunction](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/) graph, [PackedInt32Array](https://docs.godotengine.org/en/stable/classes/class_packedint32array.html) node\_ids, [Vector2](https://docs.godotengine.org/en/stable/classes/class_vector2.html) gui\_offset )  
    voidpaste\_graph\_with\_pre\_generated\_ids（ VoxelGraphFunction graph， PackedInt32Array node\_ids， Vector2 gui\_offset ）
    

Copies nodes into another graph, and connections between them only.  
将节点复制到另一个图形中，并且仅在它们之间建立连接。

Resources in node parameters will be duplicated if they don't have a file path.  
如果节点参数中的资源没有文件路径，则会重复这些资源。

If `node_ids` is provided with non-zero size, defines the IDs of copied nodes. Otherwise, they are generated.  
如果提供非零大小，则 `node_ids` 定义复制节点的 ID。否则，将生成它们。

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#) **remove\_connection**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) src\_node\_id, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) src\_port\_index, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) dst\_node\_id, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) dst\_port\_index )  
    voidremove\_connection（ int src\_node\_id， int src\_port\_index， int dst\_node\_id， int dst\_port\_index ）

Removes an existing connection between two nodes of the graph.  
删除图形的两个节点之间的现有连接。

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#) **remove\_node**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) node\_id )  
    voidremove\_node（ int node\_id ）

Removes a node from the graph.  
从图形中删除节点。

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#) **set\_expression\_node\_inputs**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) node\_id, [PackedStringArray](https://docs.godotengine.org/en/stable/classes/class_packedstringarray.html) names )  
    voidset\_expression\_node\_inputs（ int node\_id， PackedStringArray names ）

Configures inputs for an Expression node. `names` is the list of input names used in the expression.  
配置表达式节点的输入。 `names` 是表达式中使用的输入名称的列表。

`value` must be a `float` for now.  
`value` 现在一定是。 `float`

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#) **set\_node\_default\_input**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) node\_id, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) input\_index, [Variant](https://docs.godotengine.org/en/stable/classes/class_variant.html) value )  
    voidset\_node\_default\_input（ int node\_id， int input\_index， 变量值 ）
    
-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#) **set\_node\_default\_inputs\_autoconnect**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) node\_id, [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) enabled )  
    voidset\_node\_default\_inputs\_autoconnect（ int node\_id， bool 启用 ）
    

Sets wether a node input with no inbound connection will automatically create a default connection when the graph is compiled.  
设置没有入站连接的节点输入是否将在编译图形时自动创建默认连接。

This is only available on specific nodes. On other nodes, it has no effect.  
这仅在特定节点上可用。在其他节点上，它不起作用。

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#) **set\_node\_gui\_position**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) node\_id, [Vector2](https://docs.godotengine.org/en/stable/classes/class_vector2.html) position )  
    voidset\_node\_gui\_position（ int node\_id， 矢量 2 位置 ）

Sets the visual position of a node of the graph, as it will appear in the editor.  
设置图形节点的可视位置，因为它将显示在编辑器中。

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#) **set\_node\_gui\_size**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) node\_id, [Vector2](https://docs.godotengine.org/en/stable/classes/class_vector2.html) size )  
    voidset\_node\_gui\_size（ int node\_id， 矢量 2 大小 ）
    
-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#)
    
    **set\_node\_name**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) node\_id, [StringName](https://docs.godotengine.org/en/stable/classes/class_stringname.html) name )  
    voidset\_node\_name（ int node\_id， 字符串名称 ）

Sets a custom name for a node.  
设置节点的自定义名称。

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#) **set\_node\_param**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) node\_id, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) param\_index, [Variant](https://docs.godotengine.org/en/stable/classes/class_variant.html) value )  
    voidset\_node\_param（ int node\_id， int param\_index， 变量值 ）
    
-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/#) **set\_node\_param\_null**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) node\_id, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) param\_index )  
    voidset\_node\_param\_null（ int node\_id， int param\_index ）
    

_Generated on Sep 12, 2023  
生成于 Sep 12， 2023_
