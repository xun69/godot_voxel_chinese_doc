---
created: 2023-10-09T22:38:26 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceGenerator/
author: 
---

# VoxelInstanceGenerator体素实例生成器

> ## Excerpt
> 继承：资源

---
##  体素实例生成器

 继承：资源

  
决定在体素表面顶部生成实例的位置。

##  说明：

  
生成在体素表面顶部生成实例所需的信息。这可以由体素实例使用。

  
注： 要生成体素，请参阅体素生成器。

##  属性：

|  类型 |  名字 |  违约 |
| --- | --- | --- |
| `float` |  [密度](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceGenerator/#i_density) | 0.1 |
| `int` | [emit\_mode](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceGenerator/#i_emit_mode) | 0 |
| `float` | [max\_height](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceGenerator/#i_max_height) | 3.40282e+38 |
| `float` | [max\_scale](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceGenerator/#i_max_scale) | 1.0 |
| `float` | [max\_slope\_degrees](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceGenerator/#i_max_slope_degrees) | 180.0 |
| `float` | [min\_height](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceGenerator/#i_min_height) | 1.17549e-38 |
| `float` | [min\_scale](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceGenerator/#i_min_scale) | 1.0 |
| `float` | [min\_slope\_degrees](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceGenerator/#i_min_slope_degrees) | 0.0 |
| `Noise` |  [噪声](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceGenerator/#i_noise) |  |
| `int` | [noise\_dimension](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceGenerator/#i_noise_dimension) | 1 |
| `VoxelGraphFunction` | [noise\_graph](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceGenerator/#i_noise_graph) |  |
| `float` | [noise\_on\_scale](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceGenerator/#i_noise_on_scale) | 0.0 |
| `float` | [offset\_along\_normal](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceGenerator/#i_offset_along_normal) | 0.0 |
| `bool` | [random\_rotation](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceGenerator/#i_random_rotation) |  真 |
| `bool` | [random\_vertical\_flip](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceGenerator/#i_random_vertical_flip) |  假 |
| `int` | [scale\_distribution](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceGenerator/#i_scale_distribution) | 1 |
| `float` | [vertical\_alignment](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceGenerator/#i_vertical_alignment) | 1.0 |

##  枚举：

 枚举发射模式：

-     
    EMIT\_FROM\_VERTICES = 0 --- 使用网格的顶点生成实例。这是禁食选项，但会产生明显的模式。
-     
    EMIT\_FROM\_FACES\_FAST = 1 --- 使用网格的面生成实例。这是一个平衡的选项，采取了一些捷径，而不会引起太明显的模式。
-     
    EMIT\_FROM\_FACES = 2 --- 使用网格的面生成实例。这是最慢的选项，但应该不会产生明显的模式。
-   **EMIT\_MODE\_COUNT** = **3**

 枚举分布：

-     
    DISTRIBUTION\_LINEAR = 0 --- 均匀分布。
-     
    DISTRIBUTION\_QUADRATIC = 1 --- 小项目较多，大项目较少的分布。
-     
    DISTRIBUTION\_CUBIC = 2 --- 分发更多的小项目，甚至更少的大项目。
-   **DISTRIBUTION\_QUINTIC** = **3**
-   **DISTRIBUTION\_COUNT** = **4**

 枚举维度：

-   **DIMENSION\_2D** = **0**
-   **DIMENSION\_3D** = **1**
-   **DIMENSION\_COUNT** = **2**

##  属性描述

-    浮点密度 = 0.1

  
控制生成的实例数。根据所选的发射类型，可能会给出不同的结果。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **emit\_mode** = 0

  
实例主要以何种方式发出。

-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **max\_height** = 3.40282e+38

  
不会创建超过此高度的实例。

  
这也取决于所选VoxelInstancer.up\_mode。

-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **max\_scale** = 1.0

  
最小比例实例将随机化。

-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **max\_slope\_degrees** = 180.0

  
如果地面的坡度高于此角度，则不会生成实例。

  
这也取决于所选VoxelInstancer.up\_mode。

-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **min\_height** = 1.17549e-38

  
不会在此高度以下创建实例。这也取决于所选VoxelInstancer.up\_mode。

-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **min\_scale** = 1.0

  
最大缩放实例将随机化。

-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **min\_slope\_degrees** = 0.0

  
如果地面的坡度低于此角度，则不会生成实例。

  
这也取决于所选VoxelInstancer.up\_mode。

-    噪音噪声

  
用于过滤掉生成的实例的干扰，以便它们可以以噪声描述的模式生成。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **noise\_dimension** = 1

  
在评估VoxelInstanceGenerator.noise和VoxelInstanceGenerator.noise\_graph时应使用哪个维度。

-   [VoxelGraphFunction](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/) **noise\_graph**

  
用于过滤掉生成的实例的图形函数，类似于VoxelInstanceGenerator.noise，但允许更多自定义噪声计算。

  
如果图形是 2D，则图形必须有 2 个输入（X 和 Z），VoxelInstanceGenerator.noise\_dimension如果是 3D，则图形必须有 3 个输入（X、Y 和 Z）。必须有一个 SDF 输出。

-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **noise\_on\_scale** = 0.0

  
VoxelInstanceGenerator.noise 的多少也会影响实例的规模。

-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **offset\_along\_normal** = 0.0

  
偏移沿地面法线生成实例。

  
正常取决于VoxelInstancer.up\_mode，也受VoxelInstanceGenerator.vertical\_alignment的影响。

-     
    boolrandom\_rotation = 真

  
启用后，实例将随机轮换。如果没有，他们将根据地面坡度使用一致的旋转。

-     
    boolrandom\_vertical\_flip = 假

  
启用后，实例将随机颠倒。这对于小石头很有用，可以创造更多种类的错觉。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **scale\_distribution** = 1

  
设置随机刻度的分布方式。

-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **vertical\_alignment** = 1.0

  
设置与地面对齐的实例数。

  
如果为 0，则它们将与地面完全对齐。

  
如果为 1，它们将完全与被视为“向上”的方向对齐。

  
这取决于VoxelInstancer.up\_mode。

_  
生成于 Oct 02， 2023_
