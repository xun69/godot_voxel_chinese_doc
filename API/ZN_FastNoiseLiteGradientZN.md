---
created: 2023-09-27T00:01:21 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/ZN_FastNoiseLiteGradient/
author: 
---

# ZN_FastNoiseLiteGradientZN_FastNoiseLiteGradient

> ## Excerpt
> Inherits: Resource 继承：资源

---
Inherits: [Resource](https://docs.godotengine.org/en/stable/classes/class_resource.html) 继承：资源

Generates coherent and fractal noise gradients using the [FastNoiseLite](https://github.com/Auburn/FastNoise) library.  
使用 FastNoiseLite 库生成相干和分形噪声梯度。

## Properties: 属性：

| Type 类型 | Name 名字 | Default 违约 |
| --- | --- | --- |
| `float` | [amplitude 波幅](https://voxel-tools.readthedocs.io/en/latest/api/ZN_FastNoiseLiteGradient/#i_amplitude) | 30.0 |
| `float` | [fractal\_gain fractal\_gain](https://voxel-tools.readthedocs.io/en/latest/api/ZN_FastNoiseLiteGradient/#i_fractal_gain) | 0.5 |
| `float` | [fractal\_lacunarity fractal\_lacunarity](https://voxel-tools.readthedocs.io/en/latest/api/ZN_FastNoiseLiteGradient/#i_fractal_lacunarity) | 2.0 |
| `int` | [fractal\_octaves fractal\_octaves](https://voxel-tools.readthedocs.io/en/latest/api/ZN_FastNoiseLiteGradient/#i_fractal_octaves) | 3 |
| `int` | [fractal\_type fractal\_type](https://voxel-tools.readthedocs.io/en/latest/api/ZN_FastNoiseLiteGradient/#i_fractal_type) | 0 |
| `int` | [noise\_type noise\_type](https://voxel-tools.readthedocs.io/en/latest/api/ZN_FastNoiseLiteGradient/#i_noise_type) | 2 |
| `float` | [period 时期](https://voxel-tools.readthedocs.io/en/latest/api/ZN_FastNoiseLiteGradient/#i_period) | 64.0 |
| `int` | [rotation\_type\_3d rotation\_type\_3d](https://voxel-tools.readthedocs.io/en/latest/api/ZN_FastNoiseLiteGradient/#i_rotation_type_3d) | 0 |
| `int` | [seed 种子](https://voxel-tools.readthedocs.io/en/latest/api/ZN_FastNoiseLiteGradient/#i_seed) | 0 |

## Methods: 方法：

## Enumerations: 枚举：

enum **NoiseType**:  枚举噪声类型：

-   **TYPE\_OPEN\_SIMPLEX\_2** = **0**
-   **TYPE\_OPEN\_SIMPLEX\_2\_REDUCED** = **1**
-   **TYPE\_VALUE** = **2**

enum **FractalType**:  枚举分形类型：

-   **FRACTAL\_NONE** = **0**
-   **FRACTAL\_DOMAIN\_WARP\_PROGRESSIVE** = **1**
-   **FRACTAL\_DOMAIN\_WARP\_INDEPENDENT** = **2**

enum **RotationType3D**:  枚举旋转类型3D：

-   **ROTATION\_3D\_NONE** = **0**
-   **ROTATION\_3D\_IMPROVE\_XY\_PLANES** = **1**
-   **ROTATION\_3D\_IMPROVE\_XZ\_PLANES** = **2**

## Property Descriptions 属性描述

-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **amplitude** = 30.0 浮点振幅 = 30.0
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **fractal\_gain** = 0.5 floatfractal\_gain = 0.5
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **fractal\_lacunarity** = 2.0  
    floatfractal\_lacunarity = 2.0
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html)
    
    **fractal\_octaves** = 3 intfractal\_octaves = 3
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **fractal\_type** = 0 intfractal\_type = 0
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **noise\_type** = 2 intnoise\_type = 2
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **period** = 64.0 浮点周期 = 64.0
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **rotation\_type\_3d** = 0 introtation\_type\_3d = 0
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **seed** = 0 intseed = 0
    

## Method Descriptions 方法说明

-   [Vector2](https://docs.godotengine.org/en/stable/classes/class_vector2.html) **warp\_2d**( [Vector2](https://docs.godotengine.org/en/stable/classes/class_vector2.html) position )  
    Vector2warp\_2d（ 矢量 2 位置 ）
    
-   [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) **warp\_3d**( [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) position )  
    Vector3warp\_3d（ 矢量3位置 ）
    

_Generated on Sep 12, 2023  
生成于 Sep 12， 2023_
