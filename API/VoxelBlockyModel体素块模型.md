---
created: 2023-09-27T00:01:21 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModel/
author: 
---

# VoxelBlockyModel体素块模型

> ## Excerpt
> Inherits: Resource 继承：资源

---
Inherits: [Resource](https://docs.godotengine.org/en/stable/classes/class_resource.html) 继承：资源

Model stored in [VoxelBlockyLibrary](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyLibrary/) and used by [VoxelMesherBlocky](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherBlocky/).  
模型存储在VoxelBlockyLibrary中，由VoxelMesherBlocky使用。

## Description: 说明：

Represents a model to be used for voxels of a specific TYPE value. Such models must be contained within a [VoxelBlockyLibrary](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyLibrary/) to be used with [VoxelTerrain](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTerrain/) or directly with a [VoxelMesherBlocky](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherBlocky/).  
表示要用于特定 TYPE 值的体素的模型。此类模型必须包含在VoxelBlockyLibrary中，以便与VoxelTerrain一起使用或直接与VoxelMesherBlocky一起使用。

A model can be setup in various ways, see child classes.  
可以通过多种方式设置模型，请参阅子类。

## Properties: 属性：

| Type 类型 | Name 名字 | Default 违约 |
| --- | --- | --- |
| `AABB[]` | [collision\_aabbs collision\_aabbs](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModel/#i_collision_aabbs) | \[\] |
| `int` | [collision\_mask collision\_mask](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModel/#i_collision_mask) | 1 |
| `Color` | [color 颜色](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModel/#i_color) | Color(1, 1, 1, 1)  
颜色（1， 1， 1， 1） |
| `bool` | [random\_tickable random\_tickable](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModel/#i_random_tickable) | false 假 |
| `int` | [transparency\_index transparency\_index](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModel/#i_transparency_index) | 0 |
| `bool` | [culls\_neighbors culls\_neighbors](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModel/#i_culls_neighbors) | true 真 |
| `bool` | [transparent 透明](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModel/#i_transparent) | false 假 |

## Methods: 方法：

| Return 返回 | Signature 签名 |
| --- | --- |
| [Material 材料](https://docs.godotengine.org/en/stable/classes/class_material.html) | [get\_material\_override](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModel/#i_get_material_override) ( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) index ) const  
get\_material\_override （ int index ） const |
| [bool 布尔](https://docs.godotengine.org/en/stable/classes/class_bool.html) | [is\_mesh\_collision\_enabled](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModel/#i_is_mesh_collision_enabled) ( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) surface\_index ) const  
is\_mesh\_collision\_enabled （ int surface\_index ） const |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModel/#) | [rotate\_90](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModel/#i_rotate_90) ( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) \_unnamed\_arg0, [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) \_unnamed\_arg1 )  
rotate\_90 （ int \_unnamed\_arg0， bool \_unnamed\_arg1 ） |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModel/#) | [set\_material\_override](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModel/#i_set_material_override) ( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) index, [Material](https://docs.godotengine.org/en/stable/classes/class_material.html) material )  
set\_material\_override （ int 索引， 材料材料 ） |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModel/#) | [set\_mesh\_collision\_enabled](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModel/#i_set_mesh_collision_enabled) ( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) surface\_index, [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) enabled )  
set\_mesh\_collision\_enabled （ int surface\_index， 启用布尔值 ） |

## Enumerations: 枚举：

enum **Side**:  枚举侧：

-   **SIDE\_NEGATIVE\_X** = **1**
-   **SIDE\_POSITIVE\_X** = **0**
-   **SIDE\_NEGATIVE\_Y** = **2**
-   **SIDE\_POSITIVE\_Y** = **3**
-   **SIDE\_NEGATIVE\_Z** = **4**
-   **SIDE\_POSITIVE\_Z** = **5**
-   **SIDE\_COUNT** = **6**

## Property Descriptions 属性描述

-   [AABB\[\]](https://docs.godotengine.org/en/stable/classes/class_aabb[].html) **collision\_aabbs** = \[\]  
    AABB\[\]collision\_aabbs = \[\]

List of bounding boxes relative to the model. They are used for box-based collision, using [VoxelBoxMover](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBoxMover/). They are not used with mesh-based collision.  
相对于模型的边界框列表。它们用于基于盒子的碰撞，使用VoxelBoxMover。它们不与基于网格的碰撞一起使用。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **collision\_mask** = 1 intcollision\_mask = 1

Collision mask used for box-based collision [VoxelBoxMover](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBoxMover/) and voxel raycasts ([VoxelToolTerrain](https://voxel-tools.readthedocs.io/en/latest/api/VoxelToolTerrain/)). It is not used for mesh-based collisions.  
碰撞蒙版用于基于框的碰撞体素移体器和体素光线投射（体素工具地形）。它不用于基于网格的碰撞。

-   [Color](https://docs.godotengine.org/en/stable/classes/class_color.html) **color** = Color(1, 1, 1, 1)  
    颜色颜色 = 颜色（1， 1， 1， 1）

Color of the model. It will be used to modulate its color when built into a voxel mesh.  
模型的颜色。当内置到体素网格中时，它将用于调制其颜色。

-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **random\_tickable** = false  
    boolrandom\_tickable = 假

If enabled, voxels having this ID in the TYPE channel will be used by [VoxelToolTerrain.run\_blocky\_random\_tick](https://voxel-tools.readthedocs.io/en/latest/api/VoxelToolTerrain/#i_run_blocky_random_tick).  
如果启用，VoxelToolTerrain.run\_blocky\_random\_tick将使用在 TYPE 通道中具有此 ID 的体素。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **transparency\_index** = 0  
    inttransparency\_index = 0

Determines how transparency is handled when the sides of the model are culled by neighbor voxels.  
确定当相邻体素剔除模型的边时如何处理透明度。

Equal indices culls the face, different indexes doesn't.  
相等的索引会剔除人脸，不同的索引不会。

-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **culls\_neighbors** = true  
    boolculls\_neighbors = 真

If enabled, this voxel culls the faces of its neighbors. Disabling can be useful for denser transparent voxels, such as foliage.  
如果启用，此体素将剔除其相邻方的面部。禁用对于密度较大的透明体素（如植物）非常有用。

-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **transparent** = false 布尔透明 = 假

Tells if the model is transparent in the context of sides being culled by neighbor voxels.  
告知模型在被相邻体素剔除的边的上下文中是否透明。

This is a legacy property, [VoxelBlockyModel.transparency\_index](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModel/#i_transparency_index) may be used instead.  
这是一个旧属性，可以改用VoxelBlockyModel.transparency\_index。

## Method Descriptions 方法说明

-   [Material](https://docs.godotengine.org/en/stable/classes/class_material.html) **get\_material\_override**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) index )  
    Materialget\_material\_override（ 整数索引 ）

Gets the material override for a specific surface of the model.  
获取模型特定曲面的材质覆盖。

-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **is\_mesh\_collision\_enabled**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) surface\_index )  
    boolis\_mesh\_collision\_enabled（ 国际 surface\_index ）

Tells if a specific surface produces mesh-based collisions.  
告知特定曲面是否生成基于网格的碰撞。

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModel/#) **rotate\_90**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) \_unnamed\_arg0, [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) \_unnamed\_arg1 )  
    voidrotate\_90（int \_unnamed\_arg0， bool \_unnamed\_arg1 ）
    
-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModel/#) **set\_material\_override**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) index, [Material](https://docs.godotengine.org/en/stable/classes/class_material.html) material )  
    voidset\_material\_override（ int 索引， 材料材料 ）
    

Sets a material override for a specific surface of the model. It allows to use the same mesh on multiple models, but using different materials on each.  
为模型的特定曲面设置材质覆盖。它允许在多个模型上使用相同的网格，但在每个模型上使用不同的材料。

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModel/#) **set\_mesh\_collision\_enabled**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) surface\_index, [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) enabled )  
    voidset\_mesh\_collision\_enabled（ int surface\_index， bool 启用）

Enables or disables mesh-based collision on a specific surface. It allows a model to have solid parts and others where players can pass through.  
启用或禁用特定表面上基于网格的碰撞。它允许模型具有实体部分和其他玩家可以通过的部分。

_Generated on Sep 12, 2023  
生成于 Sep 12， 2023_
