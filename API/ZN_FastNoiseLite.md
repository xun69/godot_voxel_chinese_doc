---
created: 2023-10-09T22:38:26 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/ZN_FastNoiseLite/
author: 
---

# ZN_FastNoiseLiteZN_FastNoiseLite

> ## Excerpt
> 继承：资源

---
 继承：资源

  
使用 FastNoiseLite 库生成相干和分形噪声。

##  属性：

|  类型 |  名字 |  违约 |
| --- | --- | --- |
| `int` | [cellular\_distance\_function](https://voxel-tools.readthedocs.io/en/latest/api/ZN_FastNoiseLite/#i_cellular_distance_function) | 1 |
| `float` | [cellular\_jitter](https://voxel-tools.readthedocs.io/en/latest/api/ZN_FastNoiseLite/#i_cellular_jitter) | 1.0 |
| `int` | [cellular\_return\_type](https://voxel-tools.readthedocs.io/en/latest/api/ZN_FastNoiseLite/#i_cellular_return_type) | 1 |
| `float` | [fractal\_gain](https://voxel-tools.readthedocs.io/en/latest/api/ZN_FastNoiseLite/#i_fractal_gain) | 0.5 |
| `float` | [fractal\_lacunarity](https://voxel-tools.readthedocs.io/en/latest/api/ZN_FastNoiseLite/#i_fractal_lacunarity) | 2.0 |
| `int` | [fractal\_octaves](https://voxel-tools.readthedocs.io/en/latest/api/ZN_FastNoiseLite/#i_fractal_octaves) | 3 |
| `float` | [fractal\_ping\_pong\_strength](https://voxel-tools.readthedocs.io/en/latest/api/ZN_FastNoiseLite/#i_fractal_ping_pong_strength) | 2.0 |
| `int` | [fractal\_type](https://voxel-tools.readthedocs.io/en/latest/api/ZN_FastNoiseLite/#i_fractal_type) | 1 |
| `float` | [fractal\_weighted\_strength](https://voxel-tools.readthedocs.io/en/latest/api/ZN_FastNoiseLite/#i_fractal_weighted_strength) | 0.0 |
| `int` | [noise\_type](https://voxel-tools.readthedocs.io/en/latest/api/ZN_FastNoiseLite/#i_noise_type) | 0 |
| `float` |  [时期](https://voxel-tools.readthedocs.io/en/latest/api/ZN_FastNoiseLite/#i_period) | 64.0 |
| `int` | [rotation\_type\_3d](https://voxel-tools.readthedocs.io/en/latest/api/ZN_FastNoiseLite/#i_rotation_type_3d) | 0 |
| `int` |  [种子](https://voxel-tools.readthedocs.io/en/latest/api/ZN_FastNoiseLite/#i_seed) | 0 |
| `ZN_FastNoiseLiteGradient` | [warp\_noise](https://voxel-tools.readthedocs.io/en/latest/api/ZN_FastNoiseLite/#i_warp_noise) |  |

##  方法：

|  返回 |  签名 |
| --- | --- |
|  [浮](https://docs.godotengine.org/en/stable/classes/class_float.html) |   
get\_noise\_2d （ 浮点 x， 浮点 y ） |
|  [浮](https://docs.godotengine.org/en/stable/classes/class_float.html) |   
get\_noise\_2dv （ 矢量 2 位置 ） |
|  [浮](https://docs.godotengine.org/en/stable/classes/class_float.html) |   
get\_noise\_3d （ 浮点 x， 浮点数 y， 浮点数 z ） |
|  [浮](https://docs.godotengine.org/en/stable/classes/class_float.html) |   
get\_noise\_3dv （ 矢量3位置 ） |

##  枚举：

 枚举噪声类型：

-   **TYPE\_OPEN\_SIMPLEX\_2** = **0**
-   **TYPE\_OPEN\_SIMPLEX\_2S** = **1**
-   **TYPE\_CELLULAR** = **2**
-   **TYPE\_PERLIN** = **3**
-   **TYPE\_VALUE\_CUBIC** = **4**
-   **TYPE\_VALUE** = **5**

 枚举分形类型：

-   **FRACTAL\_NONE** = **0**
-   **FRACTAL\_FBM** = **1**
-   **FRACTAL\_RIDGED** = **2**
-   **FRACTAL\_PING\_PONG** = **3**

 枚举旋转类型3D：

-   **ROTATION\_3D\_NONE** = **0**
-   **ROTATION\_3D\_IMPROVE\_XY\_PLANES** = **1**
-   **ROTATION\_3D\_IMPROVE\_XZ\_PLANES** = **2**

  
枚举蜂窝距离函数：

-   **CELLULAR\_DISTANCE\_EUCLIDEAN** = **0**
-   **CELLULAR\_DISTANCE\_EUCLIDEAN\_SQ** = **1**
-   **CELLULAR\_DISTANCE\_MANHATTAN** = **2**
-   **CELLULAR\_DISTANCE\_HYBRID** = **3**

  
枚举蜂窝返回类型：

-   **CELLULAR\_RETURN\_CELL\_VALUE** = **0**
-   **CELLULAR\_RETURN\_DISTANCE** = **1**
-   **CELLULAR\_RETURN\_DISTANCE\_2** = **2**
-   **CELLULAR\_RETURN\_DISTANCE\_2\_ADD** = **3**
-   **CELLULAR\_RETURN\_DISTANCE\_2\_SUB** = **4**
-   **CELLULAR\_RETURN\_DISTANCE\_2\_MUL** = **5**
-   **CELLULAR\_RETURN\_DISTANCE\_2\_DIV** = **6**

##  属性描述

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **cellular\_distance\_function** = 1
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **cellular\_jitter** = 1.0
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **cellular\_return\_type** = 1
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **fractal\_gain** = 0.5
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **fractal\_lacunarity** = 2.0
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **fractal\_octaves** = 3
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **fractal\_ping\_pong\_strength** = 2.0
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **fractal\_type** = 1
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **fractal\_weighted\_strength** = 0.0
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **noise\_type** = 0
    
-    浮点周期 = 64.0
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **rotation\_type\_3d** = 0
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **seed** = 0
    
-   [ZN\_FastNoiseLiteGradient](https://voxel-tools.readthedocs.io/en/latest/api/ZN_FastNoiseLiteGradient/) **warp\_noise**
    

##  方法说明

-     
    floatget\_noise\_2d（ 浮点 x， 浮点 y ）
    
-     
    floatget\_noise\_2dv（ 矢量2位置 ）
    
-     
    floatget\_noise\_3d（ 浮点 x， 浮点 y， 浮点 z ）
    
-     
    floatget\_noise\_3dv（ 矢量3位置 ）
    

_  
生成于 Oct 02， 2023_
