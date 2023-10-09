# VoxelBlockyModel体素块模型

> ## Excerpt
> 继承：资源

---
##  体素块模型

 继承：资源

  
继承者：VoxelBlockyModelCube，VoxelBlockyModelEmpty，VoxelBlockyModelMesh

  
模型存储在VoxelBlockyLibrary中，由VoxelMesherBlocky使用。

##  说明：

  
表示要用于特定 TYPE 值的体素的模型。此类模型必须包含在VoxelBlockyLibrary中，以便与VoxelTerrain一起使用或直接与VoxelMesherBlocky一起使用。

  
可以通过多种方式设置模型，请参阅子类。

##  属性：

|  类型 |  名字 |  违约 |
| --- | --- | --- |
| `AABB[]` | [collision\_aabbs](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModel/#i_collision_aabbs) | \[\] |
| `int` | [collision\_mask](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModel/#i_collision_mask) | 1 |
| `Color` |  [颜色](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModel/#i_color) |   
颜色（1， 1， 1， 1） |
| `bool` | [random\_tickable](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModel/#i_random_tickable) |  假 |
| `int` | [transparency\_index](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModel/#i_transparency_index) | 0 |
| `bool` | [culls\_neighbors](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModel/#i_culls_neighbors) |  真 |
| `bool` |  [透明](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModel/#i_transparent) |  假 |

##  方法：

|  返回 |  签名 |
| --- | --- |
|  [材料](https://docs.godotengine.org/en/stable/classes/class_material.html) |   
get\_material\_override （ int index ） const |
|  [布尔](https://docs.godotengine.org/en/stable/classes/class_bool.html) |   
is\_mesh\_collision\_enabled （ int surface\_index ） const |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModel/#) |   
rotate\_90 （ int \_unnamed\_arg0， bool \_unnamed\_arg1 ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModel/#) |   
set\_material\_override （ int 索引， 材料材料 ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModel/#) |   
set\_mesh\_collision\_enabled （ int surface\_index， 启用布尔值 ） |

##  枚举：

 枚举侧：

-   **SIDE\_NEGATIVE\_X** = **1**
-   **SIDE\_POSITIVE\_X** = **0**
-   **SIDE\_NEGATIVE\_Y** = **2**
-   **SIDE\_POSITIVE\_Y** = **3**
-   **SIDE\_NEGATIVE\_Z** = **4**
-   **SIDE\_POSITIVE\_Z** = **5**
-   **SIDE\_COUNT** = **6**

##  属性描述

-   [AABB\[\]](https://docs.godotengine.org/en/stable/classes/class_aabb[].html) **collision\_aabbs** = \[\]

  
相对于模型的边界框列表。它们用于基于盒子的碰撞，使用VoxelBoxMover。它们不与基于网格的碰撞一起使用。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **collision\_mask** = 1

  
碰撞蒙版用于基于框的碰撞体素移体器和体素光线投射（体素工具地形）。它不用于基于网格的碰撞。

-     
    颜色颜色 = 颜色（1， 1， 1， 1）

  
模型的颜色。当内置到体素网格中时，它将用于调制其颜色。

-     
    boolrandom\_tickable = 假

  
如果启用，VoxelToolTerrain.run\_blocky\_random\_tick将使用在 TYPE 通道中具有此 ID 的体素。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **transparency\_index** = 0

  
确定当相邻体素剔除模型的边时如何处理透明度。

  
相等的索引会剔除人脸，不同的索引不会。

-     
    boolculls\_neighbors = 真

  
如果启用，此体素将剔除其相邻方的面部。禁用对于密度较大的透明体素（如植物）非常有用。

-    布尔透明 = 假

  
告知模型在被相邻体素剔除的边的上下文中是否透明。

  
这是一个旧属性，可以改用VoxelBlockyModel.transparency\_index。

##  方法说明

-     
    Materialget\_material\_override（ 整数索引 ）

  
获取模型特定曲面的材质覆盖。

-     
    boolis\_mesh\_collision\_enabled（ 国际 surface\_index ）

  
告知特定曲面是否生成基于网格的碰撞。

-     
    voidrotate\_90（int \_unnamed\_arg0， bool \_unnamed\_arg1 ）
    
-     
    voidset\_material\_override（ int 索引， 材料材料 ）
    

  
为模型的特定曲面设置材质覆盖。它允许在多个模型上使用相同的网格，但在每个模型上使用不同的材料。

-     
    voidset\_mesh\_collision\_enabled（ int surface\_index， bool 启用）

  
启用或禁用特定表面上基于网格的碰撞。它允许模型具有实体部分和其他玩家可以通过的部分。

_  
生成于 Oct 02， 2023_
