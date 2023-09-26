---
created: 2023-09-27T00:01:21 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesher/
author: 
---

# VoxelMesher体素网格器

> ## Excerpt
> Inherits: Resource 继承：资源

---
Inherits: [Resource](https://docs.godotengine.org/en/stable/classes/class_resource.html) 继承：资源

Base class for all meshing algorithms.  
所有网格划分算法的基类。

## Description: 说明：

In order to be rendered by Godot, voxels can be transformed into a mesh. There are various ways to do this, that's why this class is only a base for other, specialized ones. Voxel nodes automatically make use of meshers, but you can also produce meshes manually. For this, you may use one of the derived classes. Meshers can be re-used, which often yields better performance by reducing memory allocations.  
为了由Godot渲染，体素可以转换为网格。有多种方法可以做到这一点，这就是为什么这个类只是其他专业类的基础。体素节点会自动使用网格划分器，但您也可以手动生成网格。为此，您可以使用派生类之一。网格划分器可以重复使用，这通常可以通过减少内存分配来产生更好的性能。

## Methods: 方法：

| Return 返回 | Signature 签名 |
| --- | --- |
| [Mesh 网孔](https://docs.godotengine.org/en/stable/classes/class_mesh.html) | [build\_mesh](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesher/#i_build_mesh) ( [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) voxel\_buffer, [Material\[\]](https://docs.godotengine.org/en/stable/classes/class_material[].html) materials, [Dictionary](https://docs.godotengine.org/en/stable/classes/class_dictionary.html) additional\_data={} )  
build\_mesh （ 体素缓冲区 voxel\_buffer， 材料\[\] 材料， 字典 additional\_data={} ） |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) | [get\_maximum\_padding](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesher/#i_get_maximum_padding) ( ) const  
get\_maximum\_padding （ ） 常量 |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) | [get\_minimum\_padding](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesher/#i_get_minimum_padding) ( ) const  
get\_minimum\_padding （ ） 常量 |

## Method Descriptions 方法说明

-   [Mesh](https://docs.godotengine.org/en/stable/classes/class_mesh.html) **build\_mesh**( [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) voxel\_buffer, [Material\[\]](https://docs.godotengine.org/en/stable/classes/class_material[].html) materials, [Dictionary](https://docs.godotengine.org/en/stable/classes/class_dictionary.html) additional\_data={} )  
    Meshbuild\_mesh（ 体素缓冲液 voxel\_buffer， 材料\[\] 材料， 字典 additional\_data={} ）

Builds a mesh from the provided voxels. Materials will be attached to each surface based on the provided array. The way materials are used can depend on the type of mesher.  
从提供的体素构建网格。材料将根据提供的阵列附着到每个表面。材料的使用方式取决于网格划分器的类型。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **get\_maximum\_padding**( )  
    intget\_maximum\_padding（ ）

Gets by how much voxels must be padded before their lower corner in order for the mesher to work.  
了解体素在其下角之前必须填充多少才能使网格器工作。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **get\_minimum\_padding**( )  
    intget\_minimum\_padding（ ）

Gets by how much voxels must be padded after their upper corner in order for the mesher to work.  
获取体素在其上角后必须填充多少才能使网格器工作。

_Generated on Sep 12, 2023  
生成于 Sep 12， 2023_
