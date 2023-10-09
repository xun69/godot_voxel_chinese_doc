
# FastNoise2

继承：资源

  
FastNoise2 库的包装器。

##  属性：

|  类型 |  名字 |  违约 |
| --- | --- | --- |
| `int` | [cellular\_distance\_function](https://voxel-tools.readthedocs.io/en/latest/api/FastNoise2/#i_cellular_distance_function) | 0 |
| `float` | [cellular\_jitter](https://voxel-tools.readthedocs.io/en/latest/api/FastNoise2/#i_cellular_jitter) | 1.0 |
| `int` | [cellular\_return\_type](https://voxel-tools.readthedocs.io/en/latest/api/FastNoise2/#i_cellular_return_type) | 0 |
| `String` | [encoded\_node\_tree](https://voxel-tools.readthedocs.io/en/latest/api/FastNoise2/#i_encoded_node_tree) | "" |
| `float` | [fractal\_gain](https://voxel-tools.readthedocs.io/en/latest/api/FastNoise2/#i_fractal_gain) | 0.5 |
| `float` | [fractal\_lacunarity](https://voxel-tools.readthedocs.io/en/latest/api/FastNoise2/#i_fractal_lacunarity) | 2.0 |
| `int` | [fractal\_octaves](https://voxel-tools.readthedocs.io/en/latest/api/FastNoise2/#i_fractal_octaves) | 3 |
| `float` | [fractal\_ping\_pong\_strength](https://voxel-tools.readthedocs.io/en/latest/api/FastNoise2/#i_fractal_ping_pong_strength) | 2.0 |
| `int` | [fractal\_type](https://voxel-tools.readthedocs.io/en/latest/api/FastNoise2/#i_fractal_type) | 0 |
| `int` | [noise\_type](https://voxel-tools.readthedocs.io/en/latest/api/FastNoise2/#i_noise_type) | 0 |
| `float` |  [时期](https://voxel-tools.readthedocs.io/en/latest/api/FastNoise2/#i_period) | 64.0 |
| `bool` | [remap\_enabled](https://voxel-tools.readthedocs.io/en/latest/api/FastNoise2/#i_remap_enabled) |  假 |
| `float` | [remap\_input\_max](https://voxel-tools.readthedocs.io/en/latest/api/FastNoise2/#i_remap_input_max) | 1.0 |
| `float` | [remap\_input\_min](https://voxel-tools.readthedocs.io/en/latest/api/FastNoise2/#i_remap_input_min) | \-1.0 |
| `float` | [remap\_output\_max](https://voxel-tools.readthedocs.io/en/latest/api/FastNoise2/#i_remap_output_max) | 1.0 |
| `float` | [remap\_output\_min](https://voxel-tools.readthedocs.io/en/latest/api/FastNoise2/#i_remap_output_min) | \-1.0 |
| `int` |  [种子](https://voxel-tools.readthedocs.io/en/latest/api/FastNoise2/#i_seed) | 1337 |
| `bool` | [terrace\_enabled](https://voxel-tools.readthedocs.io/en/latest/api/FastNoise2/#i_terrace_enabled) |  假 |
| `float` | [terrace\_multiplier](https://voxel-tools.readthedocs.io/en/latest/api/FastNoise2/#i_terrace_multiplier) | 1.0 |
| `float` | [terrace\_smoothness](https://voxel-tools.readthedocs.io/en/latest/api/FastNoise2/#i_terrace_smoothness) | 0.0 |

##  方法：

|  返回 |  签名 |
| --- | --- |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/FastNoise2/#) |   
generate\_image （ 图像图像， 布尔可平铺 ） 常量 |
|  [浮](https://docs.godotengine.org/en/stable/classes/class_float.html) |   
get\_noise\_2d\_single （ Vector2 pos ） const |
|  [浮](https://docs.godotengine.org/en/stable/classes/class_float.html) |   
get\_noise\_3d\_single （ Vector3 pos ） const |
|  [字符串](https://docs.godotengine.org/en/stable/classes/class_string.html) |   
get\_simd\_level\_name （ 国际级 ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/FastNoise2/#) |  update\_generator （ ） |

##  枚举：

 枚举噪声类型：

-   **TYPE\_OPEN\_SIMPLEX\_2** = **0**
-   **TYPE\_SIMPLEX** = **1**
-   **TYPE\_PERLIN** = **2**
-   **TYPE\_VALUE** = **3**
-   **TYPE\_CELLULAR** = **4**
-   **TYPE\_ENCODED\_NODE\_TREE** = **5**

 枚举分形类型：

-   **FRACTAL\_NONE** = **0**
-   **FRACTAL\_FBM** = **1**
-   **FRACTAL\_RIDGED** = **2**
-   **FRACTAL\_PING\_PONG** = **3**

  
枚举蜂窝距离函数：

-   **CELLULAR\_DISTANCE\_EUCLIDEAN** = **0**
-   **CELLULAR\_DISTANCE\_EUCLIDEAN\_SQ** = **1**
-   **CELLULAR\_DISTANCE\_MANHATTAN** = **2**
-   **CELLULAR\_DISTANCE\_HYBRID** = **3**
-   **CELLULAR\_DISTANCE\_MAX\_AXIS** = **4**

  
枚举蜂窝返回类型：

-   **CELLULAR\_RETURN\_INDEX\_0** = **0**
-   **CELLULAR\_RETURN\_INDEX\_0\_ADD\_1** = **1**
-   **CELLULAR\_RETURN\_INDEX\_0\_SUB\_1** = **2**
-   **CELLULAR\_RETURN\_INDEX\_0\_MUL\_1** = **3**
-   **CELLULAR\_RETURN\_INDEX\_0\_DIV\_1** = **4**

 enum SIMDLevel：

-   **SIMD\_NULL** = **0**
-   **SIMD\_SCALAR** = **1**
-   **SIMD\_SSE** = **2**
-   **SIMD\_SSE2** = **4**
-   **SIMD\_SSE3** = **8**
-   **SIMD\_SSSE3** = **16**
-   **SIMD\_SSE41** = **32**
-   **SIMD\_SSE42** = **64**
-   **SIMD\_AVX** = **128**
-   **SIMD\_AVX2** = **256**
-   **SIMD\_AVX512** = **512**
-   **SIMD\_NEON** = **65536**

##  属性描述

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **cellular\_distance\_function** = 0
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **cellular\_jitter** = 1.0
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **cellular\_return\_type** = 0
    
-     
    Stringencoded\_node\_tree = “”
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **fractal\_gain** = 0.5
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **fractal\_lacunarity** = 2.0
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **fractal\_octaves** = 3
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **fractal\_ping\_pong\_strength** = 2.0
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **fractal\_type** = 0
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **noise\_type** = 0
    
-    浮点周期 = 64.0
    
-     
    boolremap\_enabled = 假
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **remap\_input\_max** = 1.0
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **remap\_input\_min** = -1.0
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **remap\_output\_max** = 1.0
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **remap\_output\_min** = -1.0
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **seed** = 1337
    
-     
    boolterrace\_enabled = 假
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **terrace\_multiplier** = 1.0
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **terrace\_smoothness** = 0.0
    

##  方法说明

-     
    voidgenerate\_image（图像图像，布尔可平铺）
    
-     
    floatget\_noise\_2d\_single（ 矢量2 位 ）
    
-     
    floatget\_noise\_3d\_single（ 矢量3 位 ）
    
-     
    Stringget\_simd\_level\_name（ 整数级 ）
    
-     
    voidupdate\_generator（ ）
    

_  
生成于 Oct 02， 2023_
