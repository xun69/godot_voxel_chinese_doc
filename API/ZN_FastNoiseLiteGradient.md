---
created: 2023-10-09T22:38:26 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/ZN_FastNoiseLiteGradient/
author: 
---

# ZN_FastNoiseLiteGradientZN_FastNoiseLiteGradient

> ## Excerpt
> 继承：资源

---
 继承：资源

  
使用 FastNoiseLite 库生成相干和分形噪声梯度。

##  属性：

|  类型 |  名字 |  违约 |
| --- | --- | --- |
| `float` |  [波幅](https://voxel-tools.readthedocs.io/en/latest/api/ZN_FastNoiseLiteGradient/#i_amplitude) | 30.0 |
| `float` | [fractal\_gain](https://voxel-tools.readthedocs.io/en/latest/api/ZN_FastNoiseLiteGradient/#i_fractal_gain) | 0.5 |
| `float` | [fractal\_lacunarity](https://voxel-tools.readthedocs.io/en/latest/api/ZN_FastNoiseLiteGradient/#i_fractal_lacunarity) | 2.0 |
| `int` | [fractal\_octaves](https://voxel-tools.readthedocs.io/en/latest/api/ZN_FastNoiseLiteGradient/#i_fractal_octaves) | 3 |
| `int` | [fractal\_type](https://voxel-tools.readthedocs.io/en/latest/api/ZN_FastNoiseLiteGradient/#i_fractal_type) | 0 |
| `int` | [noise\_type](https://voxel-tools.readthedocs.io/en/latest/api/ZN_FastNoiseLiteGradient/#i_noise_type) | 2 |
| `float` |  [时期](https://voxel-tools.readthedocs.io/en/latest/api/ZN_FastNoiseLiteGradient/#i_period) | 64.0 |
| `int` | [rotation\_type\_3d](https://voxel-tools.readthedocs.io/en/latest/api/ZN_FastNoiseLiteGradient/#i_rotation_type_3d) | 0 |
| `int` |  [种子](https://voxel-tools.readthedocs.io/en/latest/api/ZN_FastNoiseLiteGradient/#i_seed) | 0 |

##  方法：

|  返回 |  签名 |
| --- | --- |
|  [矢量2](https://docs.godotengine.org/en/stable/classes/class_vector2.html) |   
warp\_2d （ 矢量2 位置 ） |
|  [矢量3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) |   
warp\_3d （ 矢量3位置 ） |

##  枚举：

 枚举噪声类型：

-   **TYPE\_OPEN\_SIMPLEX\_2** = **0**
-   **TYPE\_OPEN\_SIMPLEX\_2\_REDUCED** = **1**
-   **TYPE\_VALUE** = **2**

 枚举分形类型：

-   **FRACTAL\_NONE** = **0**
-   **FRACTAL\_DOMAIN\_WARP\_PROGRESSIVE** = **1**
-   **FRACTAL\_DOMAIN\_WARP\_INDEPENDENT** = **2**

 枚举旋转类型3D：

-   **ROTATION\_3D\_NONE** = **0**
-   **ROTATION\_3D\_IMPROVE\_XY\_PLANES** = **1**
-   **ROTATION\_3D\_IMPROVE\_XZ\_PLANES** = **2**

##  属性描述

-    浮点振幅 = 30.0
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **fractal\_gain** = 0.5
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **fractal\_lacunarity** = 2.0
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **fractal\_octaves** = 3
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **fractal\_type** = 0
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **noise\_type** = 2
    
-    浮点周期 = 64.0
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **rotation\_type\_3d** = 0
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **seed** = 0
    

##  方法说明

-     
    Vector2warp\_2d（ 矢量 2 位置 ）
    
-     
    Vector3warp\_3d（ 矢量3位置 ）
    

_  
生成于 Oct 02， 2023_
