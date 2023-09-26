---
created: 2023-09-27T00:01:21 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorScript/
author: 
---

# VoxelGeneratorScript体素生成器脚本

> ## Excerpt
> Inherits: VoxelGenerator 继承：体素生成器

---
Inherits: [VoxelGenerator](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGenerator/) 继承：体素生成器

Base class for custom generators defined with a script.  
使用脚本定义的自定义生成器的基类。

## Description: 说明：

Important: this engine makes heavy use of threads. Generators will run in one of them, so make sure you don't access the scene tree or other unsafe APIs from within a generator.  
重要提示：此引擎大量使用线程。生成器将在其中一个中运行，因此请确保不要从生成器中访问场景树或其他不安全的 API。

## Methods: 方法：

| Return 返回 | Signature 签名 |
| --- | --- |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorScript/#) | [\_generate\_block](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorScript/#i__generate_block) ( [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) out\_buffer, [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) origin\_in\_voxels, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) lod ) virtual  
\_generate\_block （ VoxelBuffer out\_buffer， Vector3i origin\_in\_voxels， int lod ） virtual |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) | [\_get\_used\_channels\_mask](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorScript/#i__get_used_channels_mask) ( ) virtual const  
\_get\_used\_channels\_mask （ ） 虚拟常量 |

## Method Descriptions 方法说明

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorScript/#) **\_generate\_block**( [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) out\_buffer, [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) origin\_in\_voxels, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) lod )  
    void\_generate\_block（ VoxelBuffer out\_buffer， Vector3i origin\_in\_voxels， int lod ）

`out_buffer`: Buffer in which to populate voxel data. It will never be `null` and will have the requested size. It is only valid for this function, do not store it anywhere after the end.  
`out_buffer` ：用于填充体素数据的缓冲区。它永远不会是 `null` ，并且将具有请求的大小。它仅对此功能有效，请勿将其存储在结束后的任何地方。

`origin_in_voxels`: Coordinates of the lower corner of the box to generate, relative to LOD0. The size of the box is known from `out_buffer`.  
`origin_in_voxels` ：要生成的框下角相对于 LOD0 的坐标。盒子的大小可从 中 `out_buffer` 知道。

`lod`: Level of detail index to use for this block. It can be ignored if you don't use LOD. This may be used as a power of two, telling how big is one voxel. For example, if you use a loop to fill the buffer using noise, you should sample that noise at steps of 2^lod, starting from `origin_in_voxels` (in code you can use `1 << lod` for fast computation, instead of `pow(2, lod)`). You may want to separate variables that iterate the coordinates in `out_buffer` and variables used to generate voxel values in space.  
`lod` ：用于此块的详细级别索引。如果不使用 LOD，则可以忽略它。这可以用作 2 的幂，告诉一个体素有多大。例如，如果使用循环通过噪声填充缓冲区，则应从 （在代码 `1 << lod` 中可用于快速计算而不是 `pow(2, lod)` ）开始，以 `origin_in_voxels` 2^lod 的步长对该噪声进行采样。您可能希望将迭代坐标的变量 `out_buffer` 和用于在空间中生成体素值的变量分开。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **\_get\_used\_channels\_mask**( )  
    int\_get\_used\_channels\_mask（ ）

Use this to indicate which channels your generator will use. It returns a bitmask, so for example you may provide information like this: `(1 << channel1) | (1 << channel2)`  
使用此选项来指示生成器将使用哪些通道。它返回一个位掩码，因此例如，您可以提供如下信息： `(1 << channel1) | (1 << channel2)`

_Generated on Sep 12, 2023  
生成于 Sep 12， 2023_
