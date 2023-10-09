---
created: 2023-10-09T22:38:26 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/
author: 
---

# VoxelTool体素工具

> ## Excerpt
> 继承：引用计数

---
 继承：引用计数

  
继承者：VoxelToolBuffer， VoxelToolLodTerrain， VoxelToolTerrain

  
帮助程序类，可轻松访问和修改体素

##  说明：

  
用于访问和编辑体素的抽象界面。它允许访问单个体素，或执行批量操作，例如雕刻大块或复制/粘贴框。

  
它不是一个单独实例化的类，您可以从要使用的体素对象中获取它。

##  属性：

|  类型 |  名字 |  违约 |
| --- | --- | --- |
| `int` |  [渠道](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#i_channel) |  |
| `int` | [eraser\_value](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#i_eraser_value) |  |
| `int` |  [模式](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#i_mode) |  |
| `float` | [sdf\_scale](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#i_sdf_scale) |  |
| `float` | [sdf\_strength](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#i_sdf_strength) |  |
| `float` | [texture\_falloff](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#i_texture_falloff) |  |
| `int` | [texture\_index](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#i_texture_index) |  |
| `float` | [texture\_opacity](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#i_texture_opacity) |  |
| `int` |  [价值](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#i_value) |  |

##  方法：

|  返回 |  签名 |
| --- | --- |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) |   
color\_to\_u16 （ 颜色 ） 静态 |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) |   
color\_to\_u16\_weights （ 颜色 \_unnamed\_arg0 ） 静态 |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#) |   
copy （ Vector3i src\_pos， VoxelBuffer dst\_buffer， int channels\_mask ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#) |   
do\_box （ Vector3i 开始， Vector3i 结束 ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#) |   
do\_point （ Vector3i pos ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#) |   
do\_sphere（矢量3中心，浮点半径） |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) |   
get\_voxel （ Vector3i pos ） |
|  [浮](https://docs.godotengine.org/en/stable/classes/class_float.html) |   
get\_voxel\_f （ Vector3i pos ） |
|  [变体](https://docs.godotengine.org/en/stable/classes/class_variant.html) |   
get\_voxel\_metadata （ Vector3i pos ） const |
|  [布尔](https://docs.godotengine.org/en/stable/classes/class_bool.html) |   
is\_area\_editable （ AABB 框 ） 常量 |
|  [颜色](https://docs.godotengine.org/en/stable/classes/class_color.html) |   
normalize\_color （ 颜色 \_unnamed\_arg0 ） 静态 |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#) |   
paste （ Vector3i dst\_pos， VoxelBuffer src\_buffer， int channels\_mask ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#) |   
paste\_masked （ Vector3i dst\_pos， VoxelBuffer src\_buffer， int channels\_mask， int mask\_channel， int mask\_value ） |
|  [体素光线投射结果](https://voxel-tools.readthedocs.io/en/latest/api/VoxelRaycastResult/) |   
光线投射（矢量 3 原点、矢量 3 方向、浮点max\_distance=10.0、int collision\_mask=4294967295 ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#) |   
set\_voxel （ Vector3i pos， int v ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#) |   
set\_voxel\_f （ Vector3i pos， float v ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#) |   
set\_voxel\_metadata （ Vector3i pos， Variant meta ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#) |   
smooth\_sphere （ 矢量3 sphere\_center， 浮点sphere\_radius， 整数 blur\_radius ） |
|  [矢量4i](https://docs.godotengine.org/en/stable/classes/class_vector4i.html) |   
u16\_indices\_to\_vec4i （ int \_unnamed\_arg0 ） 静态 |
|  [颜色](https://docs.godotengine.org/en/stable/classes/class_color.html) |   
u16\_weights\_to\_color （ int \_unnamed\_arg0 ） 静态 |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) |   
vec4i\_to\_u16\_indices （ 矢量4i \_unnamed\_arg0 ） 静态 |

##  枚举：

 枚举模式：

-     
    MODE\_ADD = 0 --- 编辑VoxelBuffer.CHANNEL\_SDF时，会增加物质。对建筑很有用。
-     
    MODE\_REMOVE = 1 --- 编辑VoxelBuffer.CHANNEL\_SDF时，会减去物质。对挖掘很有用。
-     
    MODE\_SET = 2 --- 替换体素值而不进行任何混合。对块状体素很有用。
-   **MODE\_TEXTURE\_PAINT** = **3**

##  属性描述

-    国际通道

  
设置要编辑的频道。在地形节点上使用时，它将默认为第一个可用通道，具体取决于流和生成器。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **eraser\_value**

  
设置在VoxelTool.MODE\_REMOVE模式下编辑VoxelBuffer.CHANNEL\_TYPE通道时将用于擦除体素的值。

-    英特模式

  
设置函数的行为方式 `do_*` 。这可能因频道而异。

-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **sdf\_scale**

  
使用平滑体素时，将比例应用于有符号距离字段。高尺度（1 或更高）往往会产生块状结果，而低尺度（低于 1，但不太接近零）往往会更平滑。

  
这与体素上的VoxelBuffer.Depth配置有关。对于 8 位和 16 位，有符号距离字段可以采用的值范围有限，默认情况下它被钳制为 -1..1，因此梯度只能跨 2 个体素。但是，当使用LOD时，最好将该范围扩展到更长的距离，这是通过缩放SDF值来实现的。

-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **sdf\_strength**
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **texture\_falloff**
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **texture\_index**
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **texture\_opacity**
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **value**
    

  
设置将使用的体素值。这在编辑VoxelBuffer.CHANNEL\_SDF时无关紧要。

##  方法说明

-     
    intcolor\_to\_u16（ 颜色 ）

  
将规范化的 4 浮点颜色编码为 16 位整数数据。它与 COLOR 通道一起使用，在通道表示直接颜色（不使用调色板）的情况下。

-     
    intcolor\_to\_u16\_weights（ 颜色 \_unnamed\_arg0 ）

  
将规范化的 4 浮点颜色编码为 16 位整数数据，以便与 WEIGHTS 通道一起使用。

-     
    voidcopy（ Vector3i src\_pos， VoxelBuffer dst\_buffer， int channels\_mask ）

  
将体素复制到框中，并将其存储在传递的缓冲区中。

  
`src_pos` 是框的最低角，其大小由 的大小 `dst_buffer` 决定。

  
`channels_mask` 是一个位掩码，其中每个位都告诉将复制哪些通道。示例： `1 << VoxelBuffer.CHANNEL_SDF` 仅获取 SDF 数据。 `0xff` 如果您想要它们，请使用它们。

-     
    voiddo\_box（ Vector3i 开始，Vector3i 结束 ）

  
在地形的矩形长方体部分进行操作。 `begin` 并且 `end` 具有包容性。通过设置 `value` 和调用此函数 `mode` 之前选择操作以及要使用的体素。

-     
    voiddo\_point（ Vector3i pos ）
    
-     
    voiddo\_sphere（矢量3中心，浮点半径）
    
-     
    intget\_voxel（ Vector3i pos ）
    
-     
    floatget\_voxel\_f（ Vector3i pos ）
    
-     
    Variantget\_voxel\_metadata（ Vector3i pos ）
    
-     
    boolis\_area\_editable（ AABB 盒子 ）
    
-     
    Colornormalize\_color（ 彩色 \_unnamed\_arg0 ）
    
-     
    voidpaste（ Vector3i dst\_pos， VoxelBuffer src\_buffer， int channels\_mask ）
    

  
将体素粘贴到给定缓冲区中特定位置的框中。

  
`dst_pos` 是框的最低角，其大小由 的大小 `src_buffer` 决定。

  
`channels_mask` 是一个位掩码，其中每个位都指示将修改哪些通道。示例： `1 << VoxelBuffer.CHANNEL_SDF` 仅写入 SDF 数据。 `0xff` 如果您想要它们，请使用它们。

-     
    voidpaste\_masked（ Vector3i dst\_pos， VoxelBuffer src\_buffer， int channels\_mask， int mask\_channel， int mask\_value ）

  
将体素粘贴到给定缓冲区中特定位置的框中。不会粘贴在掩码通道中具有特定值的体素。

  
`dst_pos` 是框的最低角，其大小由 的大小 `src_buffer` 决定。

  
`channels_mask` 是一个位掩码，其中每个位都指示将修改哪些通道。示例： `1 << VoxelBuffer.CHANNEL_SDF` 仅写入 SDF 数据。 `0xff` 如果您想要它们，请使用它们。

  
`src_mask_channel` 将用于查找掩码值的通道。

  
`src_mask_value` 如果体素在为遮罩指定的通道中具有此值，则不会粘贴它们。

-     
    体素光线投射结果雷投射（ 矢量3 原点， 矢量3 方向， 浮点数 max\_distance=10.0， int collision\_mask=4294967295 ）

  
运行基于体素的光线投射，以查找来自原点和方向的第一个命中。

  
如果体素被命中，则返回结果对象，否则返回 `null` 。

  
当不能依赖碰撞体时，这很有用。它也可能更快（至少在短距离内），并且更精确地找到被击中的体素。它在内部使用 DDA 算法。

  
`collision_mask` 目前仅与块状体素一起使用。它与VoxelBlockyModel.collision\_mask相结合，以决定光线可以与哪种体素类型碰撞。

-     
    voidset\_voxel（ Vector3i pos， int v ）

  
设置当前通道上特定体素的原始整数值。

-     
    voidset\_voxel\_f（ Vector3i pos， float v ）

  
设置特定体素的规范化十进制值。在修改 SDF 通道上的体素时，最好使用此方法。

-     
    voidset\_voxel\_metadata（ Vector3i pos， Variant meta ）
    
-     
    voidsmooth\_sphere（ 矢量3 sphere\_center， 浮点sphere\_radius， 整数 blur\_radius ）
    

  
通过在球形区域中执行方框模糊来平滑地形。强度在球体中心处最大，在球体表面线性降低至零。球体外的体素不会受到影响。

  
`sphere_center` 是将平滑的地形中的位置。

  
`sphere_radius` 球体的半径从 `center` 体素值将受到影响的位置开始。应大于零。

  
`blur_radius` 将采样以计算平均体素值的框模糊长度的一半。值越高，平滑效果越强。应至少为 1。

  
注 1：目前仅适用于使用 SDF 数据（平滑体素）的地形。

  
注意2：当心使用高 `sphere_radius` 和高， `blur_radius` 因为如果每秒调用60次，性能会迅速下降。

-     
    Vector4iu16\_indices\_to\_vec4i（ 国际 \_unnamed\_arg0 ）

  
将来自 INDICES 通道的原始体素整数数据解码为 4 整数向量。

-     
    Coloru16\_weights\_to\_color（ 国际 \_unnamed\_arg0 ）

  
将来自 WEIGHTS 通道的原始体素整数数据解码为规范化的 4 浮点颜色。

-     
    intvec4i\_to\_u16\_indices（ 矢量4i \_unnamed\_arg0 ）

  
将 4 整数矢量编码为 16 位整数体素数据，以便在 INDICES 通道中使用。

_  
生成于 Oct 02， 2023_
