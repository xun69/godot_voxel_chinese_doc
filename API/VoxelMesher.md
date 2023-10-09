---
created: 2023-10-09T22:38:26 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesher/
author: 
---

# VoxelMesher体素网格器

> ## Excerpt
> 继承：资源

---
##  体素梅舍尔

 继承：资源

  
继承者：VoxelMesherBlocky，VoxelMesherCubes，VoxelMesherDMC，VoxelMesherTransvoxel

  
所有网格划分算法的基类。

##  说明：

  
为了由Godot渲染，体素可以转换为网格。有多种方法可以做到这一点，这就是为什么这个类只是其他专业类的基础。体素节点会自动使用网格划分器，但您也可以手动生成网格。为此，您可以使用派生类之一。网格划分器可以重复使用，这通常可以通过减少内存分配来产生更好的性能。

##  方法：

|  返回 |  签名 |
| --- | --- |
|  [网孔](https://docs.godotengine.org/en/stable/classes/class_mesh.html) |   
build\_mesh （ 体素缓冲区 voxel\_buffer， 材料\[\] 材料， 字典 additional\_data={} ） |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) |   
get\_maximum\_padding （ ） 常量 |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) |   
get\_minimum\_padding （ ） 常量 |

##  方法说明

-     
    Meshbuild\_mesh（ 体素缓冲液 voxel\_buffer， 材料\[\] 材料， 字典 additional\_data={} ）

  
从提供的体素构建网格。材料将根据提供的阵列附着到每个表面。材料的使用方式取决于网格划分器的类型。

-     
    intget\_maximum\_padding（ ）

  
了解体素在其下角之前必须填充多少才能使网格器工作。

-     
    intget\_minimum\_padding（ ）

  
获取体素在其上角后必须填充多少才能使网格器工作。

_  
生成于 Oct 02， 2023_
