---
created: 2023-09-27T00:01:21 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModelMesh/
author: 
---

# VoxelBlockyModelMesh体素块状模型网格

> ## Excerpt
> Inherits: VoxelBlockyModel继承：体素块模型

---
Inherits: [VoxelBlockyModel](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModel/)  
继承：体素块模型

Generates a model based on a custom mesh.  
基于自定义网格生成模型。

## Description: 说明：

[VoxelMesherBlocky](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherBlocky/) does not require models to be cubes. Ultimately, model visuals are all meshes. This is the most versatile option to make a model. The workflow is to make these models in a 3D editor such as Blender, making sure they are confined in a box going from (0,0) to (1,1). Textures are assigned with classic UV-mapping.  
VoxelMesherBlocky不要求模型是立方体。归根结底，模型视觉对象都是网格。这是制作模型的最通用选项。工作流程是在3D编辑器（如Blender）中制作这些模型，确保它们被限制在从（0,0）到（1,1）的框中。纹理分配有经典的 UV 映射。

## Properties: 属性：

| Type 类型 | Name 名字 | Default 违约 |
| --- | --- | --- |
| `Mesh` | [mesh 网孔](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModelMesh/#i_mesh) |  |
| `int` | [mesh\_ortho\_rotation\_index  
mesh\_ortho\_rotation\_index](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModelMesh/#i_mesh_ortho_rotation_index) | 0 |

## Property Descriptions 属性描述

-   [Mesh](https://docs.godotengine.org/en/stable/classes/class_mesh.html) **mesh** 网状网格
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **mesh\_ortho\_rotation\_index** = 0  
    intmesh\_ortho\_rotation\_index = 0
    

Orthogonal rotation applied to the mesh when baking. Values are taken from the same convention as [GridMap](https://docs.godotengine.org/en/stable/classes/class_gridmap.html) tiles.  
烘焙时应用于网格的正交旋转。值取自与网格图块相同的约定。

([GridMap](https://docs.godotengine.org/en/stable/classes/class_gridmap.html) provides a conversion method from [Basis](https://docs.godotengine.org/en/stable/classes/class_basis.html), unfortunately it is not a static method so it requires a [GridMap](https://docs.godotengine.org/en/stable/classes/class_gridmap.html) instance to exist. A helper method could be added in the future if requested)  
（ GridMap 提供了 Basis 的转换方法，不幸的是它不是静态方法，因此它需要一个 GridMap 实例才能存在。如果需要，将来可以添加帮助程序方法）

_Generated on Sep 12, 2023  
生成于 Sep 12， 2023_
