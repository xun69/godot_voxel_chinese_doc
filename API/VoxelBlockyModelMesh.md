# VoxelBlockyModelMesh体素块状模型网格

> ## Excerpt
> 继承：体素块模型

---
-   [](https://voxel-tools.readthedocs.io/en/latest/)
-   Scripting API
-   VoxelBlockyModelMesh

___

  
继承：体素块模型

  
基于自定义网格生成模型。

##  说明：

  
VoxelMesherBlocky不要求模型是立方体。归根结底，模型视觉对象都是网格。这是制作模型的最通用选项。工作流程是在3D编辑器（如Blender）中制作这些模型，确保它们被限制在从（0,0）到（1,1）的框中。纹理分配有经典的 UV 映射。

##  属性：

|  类型 |  名字 |  违约 |
| --- | --- | --- |
| `Mesh` |  [网孔](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModelMesh/#i_mesh) |  |
| `int` | [mesh\_ortho\_rotation\_index](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModelMesh/#i_mesh_ortho_rotation_index) | 0 |

##  属性描述

-    网状网格
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **mesh\_ortho\_rotation\_index** = 0
    

  
烘焙时应用于网格的正交旋转。值取自与网格图块相同的约定。

  
（ GridMap 提供了 Basis 的转换方法，不幸的是它不是静态方法，因此它需要一个 GridMap 实例才能存在。如果需要，将来可以添加帮助程序方法）

_  
生成于 Oct 02， 2023_
