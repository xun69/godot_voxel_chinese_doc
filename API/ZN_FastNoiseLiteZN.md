---
created: 2023-09-27T00:01:21 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/ZN_FastNoiseLite/
author: 
---

# ZN_FastNoiseLiteZN_FastNoiseLite

> ## Excerpt
> Inherits: Resource 继承：资源

---
Inherits: [Resource](https://docs.godotengine.org/en/stable/classes/class_resource.html) 继承：资源

Generates coherent and fractal noise using the [FastNoiseLite](https://github.com/Auburn/FastNoise) library.  
使用 FastNoiseLite 库生成相干和分形噪声。

## Properties: 属性：

## Methods: 方法：

## Enumerations: 枚举：

enum **NoiseType**:  枚举噪声类型：

-   **TYPE\_OPEN\_SIMPLEX\_2** = **0**
-   **TYPE\_OPEN\_SIMPLEX\_2S** = **1**
-   **TYPE\_CELLULAR** = **2**
-   **TYPE\_PERLIN** = **3**
-   **TYPE\_VALUE\_CUBIC** = **4**
-   **TYPE\_VALUE** = **5**

enum **FractalType**:  枚举分形类型：

-   **FRACTAL\_NONE** = **0**
-   **FRACTAL\_FBM** = **1**
-   **FRACTAL\_RIDGED** = **2**
-   **FRACTAL\_PING\_PONG** = **3**

enum **RotationType3D**:  枚举旋转类型3D：

-   **ROTATION\_3D\_NONE** = **0**
-   **ROTATION\_3D\_IMPROVE\_XY\_PLANES** = **1**
-   **ROTATION\_3D\_IMPROVE\_XZ\_PLANES** = **2**

enum **CellularDistanceFunction**:  
枚举蜂窝距离函数：

-   **CELLULAR\_DISTANCE\_EUCLIDEAN** = **0**
-   **CELLULAR\_DISTANCE\_EUCLIDEAN\_SQ** = **1**
-   **CELLULAR\_DISTANCE\_MANHATTAN** = **2**
-   **CELLULAR\_DISTANCE\_HYBRID** = **3**

enum **CellularReturnType**:  
枚举蜂窝返回类型：

-   **CELLULAR\_RETURN\_CELL\_VALUE** = **0**
-   **CELLULAR\_RETURN\_DISTANCE** = **1**
-   **CELLULAR\_RETURN\_DISTANCE\_2** = **2**
-   **CELLULAR\_RETURN\_DISTANCE\_2\_ADD** = **3**
-   **CELLULAR\_RETURN\_DISTANCE\_2\_SUB** = **4**
-   **CELLULAR\_RETURN\_DISTANCE\_2\_MUL** = **5**
-   **CELLULAR\_RETURN\_DISTANCE\_2\_DIV** = **6**

## Property Descriptions 属性描述

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **cellular\_distance\_function** = 1  
    intcellular\_distance\_function = 1
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **cellular\_jitter** = 1.0  
    floatcellular\_jitter = 1.0
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **cellular\_return\_type** = 1  
    intcellular\_return\_type = 1
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **fractal\_gain** = 0.5 floatfractal\_gain = 0.5
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **fractal\_lacunarity** = 2.0  
    floatfractal\_lacunarity = 2.0
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **fractal\_octaves** = 3 intfractal\_octaves = 3
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **fractal\_ping\_pong\_strength** = 2.0  
    floatfractal\_ping\_pong\_strength = 2.0
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **fractal\_type** = 1 intfractal\_type = 1
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **fractal\_weighted\_strength** = 0.0  
    floatfractal\_weighted\_strength = 0.0
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **noise\_type** = 0 intnoise\_type = 0
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **period** = 64.0 浮点周期 = 64.0
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **rotation\_type\_3d** = 0 introtation\_type\_3d = 0
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **seed** = 0 intseed = 0
    
-   [ZN\_FastNoiseLiteGradient](https://voxel-tools.readthedocs.io/en/latest/api/ZN_FastNoiseLiteGradient/) **warp\_noise**  
    ZN\_FastNoiseLiteGradientwarp\_noise
    

## Method Descriptions 方法说明

-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html)
    
    **get\_noise\_2d**( [float](https://docs.godotengine.org/en/stable/classes/class_float.html) x, [float](https://docs.godotengine.org/en/stable/classes/class_float.html) y )  
    floatget\_noise\_2d（ 浮点 x， 浮点 y ）
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **get\_noise\_2dv**( [Vector2](https://docs.godotengine.org/en/stable/classes/class_vector2.html) position )  
    floatget\_noise\_2dv（ 矢量2位置 ）
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **get\_noise\_3d**( [float](https://docs.godotengine.org/en/stable/classes/class_float.html) x, [float](https://docs.godotengine.org/en/stable/classes/class_float.html) y, [float](https://docs.godotengine.org/en/stable/classes/class_float.html) z )  
    floatget\_noise\_3d（ 浮点 x， 浮点 y， 浮点 z ）
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **get\_noise\_3dv**( [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) position )  
    floatget\_noise\_3dv（ 矢量3位置 ）
    

_Generated on Sep 12, 2023  
生成于 Sep 12， 2023_
