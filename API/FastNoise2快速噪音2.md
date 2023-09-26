# FastNoise2快速噪音2

Inherits: [Resource](https://docs.godotengine.org/en/stable/classes/class_resource.html) 继承：资源

Wrapper for the FastNoise2 library.  
FastNoise2 库的包装器。

## Properties: 属性：

## Methods: 方法：

## Enumerations: 枚举：

enum **NoiseType**:  枚举噪声类型：

-   **TYPE\_OPEN\_SIMPLEX\_2** = **0**
-   **TYPE\_SIMPLEX** = **1**
-   **TYPE\_PERLIN** = **2**
-   **TYPE\_VALUE** = **3**
-   **TYPE\_CELLULAR** = **4**
-   **TYPE\_ENCODED\_NODE\_TREE** = **5**

enum **FractalType**:  枚举分形类型：

-   **FRACTAL\_NONE** = **0**
-   **FRACTAL\_FBM** = **1**
-   **FRACTAL\_RIDGED** = **2**
-   **FRACTAL\_PING\_PONG** = **3**

enum **CellularDistanceFunction**:  
枚举蜂窝距离函数：

-   **CELLULAR\_DISTANCE\_EUCLIDEAN** = **0**
-   **CELLULAR\_DISTANCE\_EUCLIDEAN\_SQ** = **1**
-   **CELLULAR\_DISTANCE\_MANHATTAN** = **2**
-   **CELLULAR\_DISTANCE\_HYBRID** = **3**
-   **CELLULAR\_DISTANCE\_MAX\_AXIS** = **4**

enum **CellularReturnType**:  
枚举蜂窝返回类型：

-   **CELLULAR\_RETURN\_INDEX\_0** = **0**
-   **CELLULAR\_RETURN\_INDEX\_0\_ADD\_1** = **1**
-   **CELLULAR\_RETURN\_INDEX\_0\_SUB\_1** = **2**
-   **CELLULAR\_RETURN\_INDEX\_0\_MUL\_1** = **3**
-   **CELLULAR\_RETURN\_INDEX\_0\_DIV\_1** = **4**

enum **SIMDLevel**:  enum SIMDLevel：

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

## Property Descriptions 属性描述

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **cellular\_distance\_function** = 0  
    intcellular\_distance\_function = 0
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **cellular\_jitter** = 1.0  
    floatcellular\_jitter = 1.0
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html)
    
    **cellular\_return\_type** = 0  
    intcellular\_return\_type = 0
-   [String](https://docs.godotengine.org/en/stable/classes/class_string.html) **encoded\_node\_tree** = ""  
    Stringencoded\_node\_tree = “”
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **fractal\_gain** = 0.5 floatfractal\_gain = 0.5
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **fractal\_lacunarity** = 2.0  
    floatfractal\_lacunarity = 2.0
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **fractal\_octaves** = 3 intfractal\_octaves = 3
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **fractal\_ping\_pong\_strength** = 2.0  
    floatfractal\_ping\_pong\_strength = 2.0
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **fractal\_type** = 0 intfractal\_type = 0
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **noise\_type** = 0 intnoise\_type = 0
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **period** = 64.0 浮点周期 = 64.0
    
-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **remap\_enabled** = false  
    boolremap\_enabled = 假
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **remap\_input\_max** = 1.0  
    floatremap\_input\_max = 1.0
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **remap\_input\_min** = -1.0  
    floatremap\_input\_min = -1.0
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **remap\_output\_max** = 1.0  
    floatremap\_output\_max = 1.0
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **remap\_output\_min** = -1.0  
    floatremap\_output\_min = -1.0
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **seed** = 1337 intseed = 1337
    
-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **terrace\_enabled** = false  
    boolterrace\_enabled = 假
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **terrace\_multiplier** = 1.0  
    floatterrace\_multiplier = 1.0
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **terrace\_smoothness** = 0.0  
    floatterrace\_smoothness = 0.0
    

## Method Descriptions 方法说明

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/FastNoise2/#) **generate\_image**( [Image](https://docs.godotengine.org/en/stable/classes/class_image.html) image, [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) tileable )  
    voidgenerate\_image（图像图像，布尔可平铺）
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **get\_noise\_2d\_single**( [Vector2](https://docs.godotengine.org/en/stable/classes/class_vector2.html) pos )  
    floatget\_noise\_2d\_single（ 矢量2 位 ）
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **get\_noise\_3d\_single**( [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) pos )  
    floatget\_noise\_3d\_single（ 矢量3 位 ）
    
-   [String](https://docs.godotengine.org/en/stable/classes/class_string.html) **get\_simd\_level\_name**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) level )  
    Stringget\_simd\_level\_name（ 整数级 ）
    
-   [void](https://voxel-tools.readthedocs.io/en/latest/api/FastNoise2/#) **update\_generator**( )  
    voidupdate\_generator（ ）
    

_Generated on Sep 12, 2023  
生成于 Sep 12， 2023_
