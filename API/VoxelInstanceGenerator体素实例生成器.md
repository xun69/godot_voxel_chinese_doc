---
created: 2023-09-27T00:01:21 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceGenerator/
author: 
---

# VoxelInstanceGenerator体素实例生成器

> ## Excerpt
> Inherits: Resource 继承：资源

---
Inherits: [Resource](https://docs.godotengine.org/en/stable/classes/class_resource.html) 继承：资源

Decides where to spawn instances on top of a voxel surface.  
决定在体素表面顶部生成实例的位置。

## Description: 说明：

Generates the necessary information to spawn instances on top of a voxel surface. This may be used by a [VoxelInstancer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstancer/).  
生成在体素表面顶部生成实例所需的信息。这可以由体素实例使用。

Note: to generate voxels, see [VoxelGenerator](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGenerator/).  
注： 要生成体素，请参阅体素生成器。

## Properties: 属性：

| Type 类型 | Name 名字 | Default 违约 |
| --- | --- | --- |
| `float` | [density 密度](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceGenerator/#i_density) | 0.1 |
| `int` | [emit\_mode emit\_mode](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceGenerator/#i_emit_mode) | 0 |
| `float` | [max\_height max\_height](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceGenerator/#i_max_height) | 3.40282e+38 3.40282e+38 |
| `float` | [max\_scale max\_scale](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceGenerator/#i_max_scale) | 1.0 |
| `float` | [max\_slope\_degrees max\_slope\_degrees](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceGenerator/#i_max_slope_degrees) | 180.0 |
| `float` | [min\_height min\_height](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceGenerator/#i_min_height) | 1.17549e-38 1.17549e-38 |
| `float` | [min\_scale min\_scale](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceGenerator/#i_min_scale) | 1.0 |
| `float` | [min\_slope\_degrees min\_slope\_degrees](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceGenerator/#i_min_slope_degrees) | 0.0 |
| `Noise` | [noise 噪声](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceGenerator/#i_noise) |  |
| `int` | [noise\_dimension noise\_dimension](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceGenerator/#i_noise_dimension) | 1 |
| `VoxelGraphFunction` | [noise\_graph noise\_graph](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceGenerator/#i_noise_graph) |  |
| `float` | [noise\_on\_scale noise\_on\_scale](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceGenerator/#i_noise_on_scale) | 0.0 |
| `float` | [offset\_along\_normal offset\_along\_normal](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceGenerator/#i_offset_along_normal) | 0.0 |
| `bool` | [random\_rotation random\_rotation](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceGenerator/#i_random_rotation) | true 真 |
| `bool` | [random\_vertical\_flip random\_vertical\_flip](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceGenerator/#i_random_vertical_flip) | false 假 |
| `int` | [scale\_distribution scale\_distribution](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceGenerator/#i_scale_distribution) | 1 |
| `float` | [vertical\_alignment vertical\_alignment](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceGenerator/#i_vertical_alignment) | 1.0 |

## Enumerations: 枚举：

enum **EmitMode**:  枚举发射模式：

-   **EMIT\_FROM\_VERTICES** = **0** --- Use vertices of the mesh to spawn instances. This is the fasted option, but can produce noticeable patterns.  
    EMIT\_FROM\_VERTICES = 0 --- 使用网格的顶点生成实例。这是禁食选项，但会产生明显的模式。
-   **EMIT\_FROM\_FACES\_FAST** = **1** --- Uses faces of the mesh to spawn instances. It is a balanced option with some shortcuts taken, without causing too noticeable patterns.  
    EMIT\_FROM\_FACES\_FAST = 1 --- 使用网格的面生成实例。这是一个平衡的选项，采取了一些捷径，而不会引起太明显的模式。
-   **EMIT\_FROM\_FACES** = **2** --- Uses faces of the mesh to spawn instances. This is the slowest option, but should produce no noticeable patterns.  
    EMIT\_FROM\_FACES = 2 --- 使用网格的面生成实例。这是最慢的选项，但应该不会产生明显的模式。
-   **EMIT\_MODE\_COUNT** = **3**

enum **Distribution**:  枚举分布：

-   **DISTRIBUTION\_LINEAR** = **0** --- Uniform distribution.  
    DISTRIBUTION\_LINEAR = 0 --- 均匀分布。
-   **DISTRIBUTION\_QUADRATIC** = **1** --- Distribution with more small items, and fewer big ones.  
    DISTRIBUTION\_QUADRATIC = 1 --- 小项目较多，大项目较少的分布。
-   **DISTRIBUTION\_CUBIC** = **2** --- Distribution with even more small items, and even fewer big ones.  
    DISTRIBUTION\_CUBIC = 2 --- 分发更多的小项目，甚至更少的大项目。
-   **DISTRIBUTION\_QUINTIC** = **3**
-   **DISTRIBUTION\_COUNT** = **4**

enum **Dimension**:  枚举维度：

-   **DIMENSION\_2D** = **0**
-   **DIMENSION\_3D** = **1**
-   **DIMENSION\_COUNT** = **2**

## Property Descriptions 属性描述

-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **density** = 0.1 浮点密度 = 0.1

Controls how many instances are generated. Might give different results depending on the type of emission chosen.  
控制生成的实例数。根据所选的发射类型，可能会给出不同的结果。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **emit\_mode** = 0 intemit\_mode = 0

In which way instances are primarily emitted.  
实例主要以何种方式发出。

-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **max\_height** = 3.40282e+38  
    floatmax\_height = 3.40282e+38

Instances will not be created above this height.  
不会创建超过此高度的实例。

This also depends on the chosen [VoxelInstancer.up\_mode](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstancer/#i_up_mode).  
这也取决于所选VoxelInstancer.up\_mode。

-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **max\_scale** = 1.0 floatmax\_scale = 1.0

Minimum scale instances will be randomized with.  
最小比例实例将随机化。

-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **max\_slope\_degrees** = 180.0  
    floatmax\_slope\_degrees = 180.0

Instances will not spawn if the ground has a slope higher than this angle.  
如果地面的坡度高于此角度，则不会生成实例。

This also depends on the chosen [VoxelInstancer.up\_mode](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstancer/#i_up_mode).  
这也取决于所选VoxelInstancer.up\_mode。

-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **min\_height** = 1.17549e-38  
    floatmin\_height = 1.17549e-38

Instances will not be created below this height. This also depends on the chosen [VoxelInstancer.up\_mode](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstancer/#i_up_mode).  
不会在此高度以下创建实例。这也取决于所选VoxelInstancer.up\_mode。

-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **min\_scale** = 1.0 floatmin\_scale = 1.0

Maximum scale instances will be randomized with.  
最大缩放实例将随机化。

-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **min\_slope\_degrees** = 0.0  
    floatmin\_slope\_degrees = 0.0

Instances will not spawn if the ground has a slope lower than this angle.  
如果地面的坡度低于此角度，则不会生成实例。

This also depends on the chosen [VoxelInstancer.up\_mode](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstancer/#i_up_mode).  
这也取决于所选VoxelInstancer.up\_mode。

-   [Noise](https://docs.godotengine.org/en/stable/classes/class_noise.html) **noise** 噪音噪声

Noise used to filter out spawned instances, so that they may spawn in patterns described by the noise.  
用于过滤掉生成的实例的干扰，以便它们可以以噪声描述的模式生成。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **noise\_dimension** = 1 intnoise\_dimension = 1

Which dimension should be used when evaluating [VoxelInstanceGenerator.noise](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceGenerator/#i_noise) and [VoxelInstanceGenerator.noise\_graph](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceGenerator/#i_noise_graph).  
在评估VoxelInstanceGenerator.noise和VoxelInstanceGenerator.noise\_graph时应使用哪个维度。

-   [VoxelGraphFunction](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/) **noise\_graph**  
    VoxelGraphFunctionnoise\_graph

Graph function used to filter out spawned instances, similar to [VoxelInstanceGenerator.noise](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceGenerator/#i_noise), but allows more custom noise computations.  
用于过滤掉生成的实例的图形函数，类似于VoxelInstanceGenerator.noise，但允许更多自定义噪声计算。

The graph must have 2 inputs (X and Z) if [VoxelInstanceGenerator.noise\_dimension](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceGenerator/#i_noise_dimension) is 2D, and 3 inputs (X, Y and Z) if 3D. There must be one SDF output.  
如果图形是 2D，则图形必须有 2 个输入（X 和 Z），VoxelInstanceGenerator.noise\_dimension如果是 3D，则图形必须有 3 个输入（X、Y 和 Z）。必须有一个 SDF 输出。

-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **noise\_on\_scale** = 0.0  
    floatnoise\_on\_scale = 0.0

How much [VoxelInstanceGenerator.noise](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceGenerator/#i_noise) also affects the scale of instances.  
VoxelInstanceGenerator.noise 的多少也会影响实例的规模。

-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **offset\_along\_normal** = 0.0  
    floatoffset\_along\_normal = 0.0

Offsets spawned instances along the normal of the ground.  
偏移沿地面法线生成实例。

The normal depends on [VoxelInstancer.up\_mode](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstancer/#i_up_mode) and is also affected by [VoxelInstanceGenerator.vertical\_alignment](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceGenerator/#i_vertical_alignment).  
正常取决于VoxelInstancer.up\_mode，也受VoxelInstanceGenerator.vertical\_alignment的影响。

-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **random\_rotation** = true  
    boolrandom\_rotation = 真

When enbabled, instances will be given a random rotation. If not, they will use a consistent rotation depending on the ground slope.  
启用后，实例将随机轮换。如果没有，他们将根据地面坡度使用一致的旋转。

-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **random\_vertical\_flip** = false  
    boolrandom\_vertical\_flip = 假

When enabled, instances will randomly be flipped upside down. This can be useful with small rocks to create illusion of more variety.  
启用后，实例将随机颠倒。这对于小石头很有用，可以创造更多种类的错觉。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **scale\_distribution** = 1  
    intscale\_distribution = 1

Sets how random scales are distributed.  
设置随机刻度的分布方式。

-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **vertical\_alignment** = 1.0  
    floatvertical\_alignment = 1.0

Sets how much instances will align with the ground.  
设置与地面对齐的实例数。

If 0, they will completely align with the ground.  
如果为 0，则它们将与地面完全对齐。

If 1, they will completely align with whichever direction is considered "up".  
如果为 1，它们将完全与被视为“向上”的方向对齐。

This depends on [VoxelInstancer.up\_mode](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstancer/#i_up_mode).  
这取决于VoxelInstancer.up\_mode。

_Generated on Sep 12, 2023  
生成于 Sep 12， 2023_
