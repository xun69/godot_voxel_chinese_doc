---
created: 2023-10-09T22:38:26 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorScript/
author: 
---

# VoxelGeneratorScript体素生成器脚本

> ## Excerpt
> 继承：体素生成器

---
##  体素生成器脚本

 继承：体素生成器

  
使用脚本定义的自定义生成器的基类。

##  说明：

  
重要提示：此引擎大量使用线程。生成器将在其中一个中运行，因此请确保不要从生成器中访问场景树或其他不安全的 API。

##  方法：

|  返回 |  签名 |
| --- | --- |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorScript/#) |   
\_generate\_block （ VoxelBuffer out\_buffer， Vector3i origin\_in\_voxels， int lod ） virtual |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) |   
\_get\_used\_channels\_mask （ ） 虚拟常量 |

##  方法说明

-     
    void\_generate\_block（ VoxelBuffer out\_buffer， Vector3i origin\_in\_voxels， int lod ）

  
`out_buffer` ：用于填充体素数据的缓冲区。它永远不会是 `null` ，并且将具有请求的大小。它仅对此功能有效，请勿将其存储在结束后的任何地方。

  
`origin_in_voxels` ：要生成的框下角相对于 LOD0 的坐标。盒子的大小可从 中 `out_buffer` 知道。

  
`lod` ：用于此块的详细级别索引。如果不使用 LOD，则可以忽略它。这可以用作 2 的幂，告诉一个体素有多大。例如，如果使用循环通过噪声填充缓冲区，则应从 （在代码 `1 << lod` 中可用于快速计算而不是 `pow(2, lod)` ）开始，以 `origin_in_voxels` 2^lod 的步长对该噪声进行采样。您可能希望将迭代坐标的变量 `out_buffer` 和用于在空间中生成体素值的变量分开。

-     
    int\_get\_used\_channels\_mask（ ）

  
使用此选项来指示生成器将使用哪些通道。它返回一个位掩码，因此例如，您可以提供如下信息： `(1 << channel1) | (1 << channel2)`

_  
生成于 Oct 02， 2023_
