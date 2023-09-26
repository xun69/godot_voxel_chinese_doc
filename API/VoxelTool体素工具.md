---
created: 2023-09-27T00:01:21 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/
author: 
---

# VoxelTool体素工具

> ## Excerpt
> Inherits: RefCounted 继承：引用计数

---
Inherits: [RefCounted](https://docs.godotengine.org/en/stable/classes/class_refcounted.html) 继承：引用计数

Helper class to easily access and modify voxels  
帮助程序类，可轻松访问和修改体素

## Description: 说明：

Abstract interface to access and edit voxels. It allows accessing individual voxels, or doing bulk operations such as carving large chunks or copy/paste boxes.  
用于访问和编辑体素的抽象界面。它允许访问单个体素，或执行批量操作，例如雕刻大块或复制/粘贴框。

It's not a class to instantiate alone, you may get it from the voxel objects you want to work with.  
它不是一个单独实例化的类，您可以从要使用的体素对象中获取它。

## Properties: 属性：

## Methods: 方法：

| Return 返回 | Signature 签名 |
| --- | --- |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) | [color\_to\_u16](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#i_color_to_u16) ( [Color](https://docs.godotengine.org/en/stable/classes/class_color.html) color ) static  
color\_to\_u16 （ 颜色 ） 静态 |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) | [color\_to\_u16\_weights](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#i_color_to_u16_weights) ( [Color](https://docs.godotengine.org/en/stable/classes/class_color.html) \_unnamed\_arg0 ) static  
color\_to\_u16\_weights （ 颜色 \_unnamed\_arg0 ） 静态 |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#) | [copy](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#i_copy) ( [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) src\_pos, [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) dst\_buffer, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) channels\_mask )  
copy （ Vector3i src\_pos， VoxelBuffer dst\_buffer， int channels\_mask ） |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#) | [do\_box](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#i_do_box) ( [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) begin, [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) end )  
do\_box （ Vector3i 开始， Vector3i 结束 ） |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#) | [do\_point](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#i_do_point) ( [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) pos )  
do\_point （ Vector3i pos ） |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#) | [do\_sphere](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#i_do_sphere) ( [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) center, [float](https://docs.godotengine.org/en/stable/classes/class_float.html) radius )  
do\_sphere（矢量3中心，浮点半径） |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) | [get\_voxel](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#i_get_voxel) ( [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) pos )  
get\_voxel （ Vector3i pos ） |
| [float 浮](https://docs.godotengine.org/en/stable/classes/class_float.html) | [get\_voxel\_f](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#i_get_voxel_f) ( [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) pos )  
get\_voxel\_f （ Vector3i pos ） |
| [Variant 变体](https://docs.godotengine.org/en/stable/classes/class_variant.html) | [get\_voxel\_metadata](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#i_get_voxel_metadata) ( [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) pos ) const  
get\_voxel\_metadata （ Vector3i pos ） const |
| [bool 布尔](https://docs.godotengine.org/en/stable/classes/class_bool.html) | [is\_area\_editable](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#i_is_area_editable) ( [AABB](https://docs.godotengine.org/en/stable/classes/class_aabb.html) box ) const  
is\_area\_editable （ AABB 框 ） 常量 |
| [Color 颜色](https://docs.godotengine.org/en/stable/classes/class_color.html) | [normalize\_color](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#i_normalize_color) ( [Color](https://docs.godotengine.org/en/stable/classes/class_color.html) \_unnamed\_arg0 ) static  
normalize\_color （ 颜色 \_unnamed\_arg0 ） 静态 |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#) | [paste](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#i_paste) ( [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) dst\_pos, [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) src\_buffer, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) channels\_mask )  
paste （ Vector3i dst\_pos， VoxelBuffer src\_buffer， int channels\_mask ） |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#) | [paste\_masked](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#i_paste_masked) ( [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) dst\_pos, [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) src\_buffer, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) channels\_mask, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) mask\_channel, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) mask\_value )  
paste\_masked （ Vector3i dst\_pos， VoxelBuffer src\_buffer， int channels\_mask， int mask\_channel， int mask\_value ） |
| [VoxelRaycastResult 体素光线投射结果](https://voxel-tools.readthedocs.io/en/latest/api/VoxelRaycastResult/) | [raycast](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#i_raycast) ( [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) origin, [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) direction, [float](https://docs.godotengine.org/en/stable/classes/class_float.html) max\_distance=10.0, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) collision\_mask=4294967295 )  
光线投射（矢量 3 原点、矢量 3 方向、浮点max\_distance=10.0、int collision\_mask=4294967295 ） |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#) | [set\_voxel](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#i_set_voxel) ( [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) pos, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) v )  
set\_voxel （ Vector3i pos， int v ） |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#) | [set\_voxel\_f](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#i_set_voxel_f) ( [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) pos, [float](https://docs.godotengine.org/en/stable/classes/class_float.html) v )  
set\_voxel\_f （ Vector3i pos， float v ） |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#) | [set\_voxel\_metadata](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#i_set_voxel_metadata) ( [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) pos, [Variant](https://docs.godotengine.org/en/stable/classes/class_variant.html) meta )  
set\_voxel\_metadata （ Vector3i pos， Variant meta ） |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#) | [smooth\_sphere](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#i_smooth_sphere) ( [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) sphere\_center, [float](https://docs.godotengine.org/en/stable/classes/class_float.html) sphere\_radius, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) blur\_radius )  
smooth\_sphere （ 矢量3 sphere\_center， 浮点sphere\_radius， 整数 blur\_radius ） |
| [Vector4i 矢量4i](https://docs.godotengine.org/en/stable/classes/class_vector4i.html) | [u16\_indices\_to\_vec4i](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#i_u16_indices_to_vec4i) ( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) \_unnamed\_arg0 ) static  
u16\_indices\_to\_vec4i （ int \_unnamed\_arg0 ） 静态 |
| [Color 颜色](https://docs.godotengine.org/en/stable/classes/class_color.html) | [u16\_weights\_to\_color](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#i_u16_weights_to_color) ( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) \_unnamed\_arg0 ) static  
u16\_weights\_to\_color （ int \_unnamed\_arg0 ） 静态 |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) | [vec4i\_to\_u16\_indices](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#i_vec4i_to_u16_indices) ( [Vector4i](https://docs.godotengine.org/en/stable/classes/class_vector4i.html) \_unnamed\_arg0 ) static  
vec4i\_to\_u16\_indices （ 矢量4i \_unnamed\_arg0 ） 静态 |

## Enumerations: 枚举：

enum **Mode**:  枚举模式：

-   **MODE\_ADD** = **0** --- When editing \[enum VoxelBuffer.CHANNEL\_SDF\], will add matter. Useful for building.  
    MODE\_ADD = 0 --- 编辑 \[enum VoxelBuffer.CHANNEL\_SDF\] 时，会增加物质。对建筑很有用。
-   **MODE\_REMOVE** = **1** --- When editing \[enum VoxelBuffer.CHANNEL\_SDF\], will subtract matter. Useful for digging.  
    MODE\_REMOVE = 1 --- 编辑 \[枚举VoxelBuffer.CHANNEL\_SDF\] 时，将减去物质。对挖掘很有用。
-   **MODE\_SET** = **2** --- Replace voxel values without any blending. Useful for blocky voxels.  
    MODE\_SET = 2 --- 替换体素值而不进行任何混合。对块状体素很有用。
-   **MODE\_TEXTURE\_PAINT** = **3**

## Property Descriptions 属性描述

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **channel** 国际通道

Set which channel will be edited. When used on a terrain node, it will default to the first available channel, based on the stream and generator.  
设置要编辑的频道。在地形节点上使用时，它将默认为第一个可用通道，具体取决于流和生成器。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **eraser\_value** interaser\_value

Sets which value will be used to erase voxels when editing the [VoxelBuffer.CHANNEL\_TYPE](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#enumerations) channel in [VoxelTool.MODE\_REMOVE](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#enumerations) mode.  
设置在VoxelTool.MODE\_REMOVE模式下编辑VoxelBuffer.CHANNEL\_TYPE通道时将用于擦除体素的值。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **mode** 英特模式

Sets how `do_*` functions will behave. This may vary depending on the channel.  
设置函数的行为方式 `do_*` 。这可能因频道而异。

-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **sdf\_scale** floatsdf\_scale

When working with smooth voxels, applies a scale to the signed distance field. A high scale (1 or higher) will tend to produce blocky results, and a low scale (below 1, but not too close to zero) will tend to be smoother.  
使用平滑体素时，将比例应用于有符号距离字段。高尺度（1 或更高）往往会产生块状结果，而低尺度（低于 1，但不太接近零）往往会更平滑。

This is related to the [VoxelBuffer.Depth](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#enumerations) configuration on voxels. For 8-bit and 16-bit, there is a limited range of values the Signed Distance Field can take, and by default it is clamped to -1..1, so the gradient can only range across 2 voxels. But when LOD is used, it is better to stretch that range over a longer distance, and this is achieved by scaling SDF values.  
这与体素上的VoxelBuffer.Depth配置有关。对于 8 位和 16 位，有符号距离字段可以采用的值范围有限，默认情况下它被钳制为 -1..1，因此梯度只能跨 2 个体素。但是，当使用LOD时，最好将该范围扩展到更长的距离，这是通过缩放SDF值来实现的。

-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **sdf\_strength** floatsdf\_strength
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **texture\_falloff** floattexture\_falloff
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **texture\_index** inttexture\_index
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **texture\_opacity** floattexture\_opacity
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **value** intvalue
    

Sets which voxel value will be used. This is not relevant when editing [VoxelBuffer.CHANNEL\_SDF](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#enumerations).  
设置将使用的体素值。这在编辑VoxelBuffer.CHANNEL\_SDF时无关紧要。

## Method Descriptions 方法说明

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **color\_to\_u16**( [Color](https://docs.godotengine.org/en/stable/classes/class_color.html) color )  
    intcolor\_to\_u16（ 颜色 ）

Encodes normalized 4-float color into 16-bit integer data. It is used with the COLOR channel, in cases where the channel represents direct colors (without using a palette).  
将规范化的 4 浮点颜色编码为 16 位整数数据。它与 COLOR 通道一起使用，在通道表示直接颜色（不使用调色板）的情况下。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **color\_to\_u16\_weights**( [Color](https://docs.godotengine.org/en/stable/classes/class_color.html) \_unnamed\_arg0 )  
    intcolor\_to\_u16\_weights（ 颜色 \_unnamed\_arg0 ）

Encodes normalized 4-float color into 16-bit integer data, for use with the WEIGHTS channel.  
将规范化的 4 浮点颜色编码为 16 位整数数据，以便与 WEIGHTS 通道一起使用。

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#) **copy**( [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) src\_pos, [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) dst\_buffer, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) channels\_mask )  
    voidcopy（ Vector3i src\_pos， VoxelBuffer dst\_buffer， int channels\_mask ）

Copies voxels in a box and stores them in the passed buffer.  
将体素复制到框中，并将其存储在传递的缓冲区中。

`src_pos` is the lowest corner of the box, and its size is determined by the size of `dst_buffer`.  
`src_pos` 是框的最低角，其大小由 的大小 `dst_buffer` 决定。

`channels_mask` is a bitmask where each bit tells which channels will be copied. Example: `1 << VoxelBuffer.CHANNEL_SDF` to get only SDF data. Use `0xff` if you want them all.  
`channels_mask` 是一个位掩码，其中每个位都告诉将复制哪些通道。示例： `1 << VoxelBuffer.CHANNEL_SDF` 仅获取 SDF 数据。 `0xff` 如果您想要它们，请使用它们。

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#) **do\_box**( [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) begin, [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) end )  
    voiddo\_box（ Vector3i 开始，Vector3i 结束 ）

Operate on a rectangular cuboid section of the terrain. `begin` and `end` are inclusive. Choose operation and which voxel to use by setting `value` and `mode` before calling this function.  
在地形的矩形长方体部分进行操作。 `begin` 并且 `end` 具有包容性。通过设置 `value` 和调用此函数 `mode` 之前选择操作以及要使用的体素。

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#) **do\_point**( [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) pos )  
    voiddo\_point（ Vector3i pos ）
    
-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#) **do\_sphere**( [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) center, [float](https://docs.godotengine.org/en/stable/classes/class_float.html) radius )  
    voiddo\_sphere（矢量3中心，浮点半径）
    
-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **get\_voxel**( [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) pos )  
    intget\_voxel（ Vector3i pos ）
    
-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **get\_voxel\_f**( [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) pos )  
    floatget\_voxel\_f（ Vector3i pos ）
    
-   [Variant](https://docs.godotengine.org/en/stable/classes/class_variant.html) **get\_voxel\_metadata**( [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) pos )  
    Variantget\_voxel\_metadata（ Vector3i pos ）
    
-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **is\_area\_editable**( [AABB](https://docs.godotengine.org/en/stable/classes/class_aabb.html) box )  
    boolis\_area\_editable（ AABB 盒子 ）
    
-   [Color](https://docs.godotengine.org/en/stable/classes/class_color.html) **normalize\_color**( [Color](https://docs.godotengine.org/en/stable/classes/class_color.html) \_unnamed\_arg0 )  
    Colornormalize\_color（ 彩色 \_unnamed\_arg0 ）
    
-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#) **paste**( [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) dst\_pos, [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) src\_buffer, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) channels\_mask )  
    voidpaste（ Vector3i dst\_pos， VoxelBuffer src\_buffer， int channels\_mask ）
    

Paste voxels in a box from the given buffer at a specific location.  
将体素粘贴到给定缓冲区中特定位置的框中。

`dst_pos` is the lowest corner of the box, and its size is determined by the size of `src_buffer`.  
`dst_pos` 是框的最低角，其大小由 的大小 `src_buffer` 决定。

`channels_mask` is a bitmask where each bit tells which channels will be modified. Example: `1 << VoxelBuffer.CHANNEL_SDF` only write SDF data. Use `0xff` if you want them all.  
`channels_mask` 是一个位掩码，其中每个位都指示将修改哪些通道。示例： `1 << VoxelBuffer.CHANNEL_SDF` 仅写入 SDF 数据。 `0xff` 如果您想要它们，请使用它们。

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#) **paste\_masked**( [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) dst\_pos, [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) src\_buffer, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) channels\_mask, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) mask\_channel, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) mask\_value )  
    voidpaste\_masked（ Vector3i dst\_pos， VoxelBuffer src\_buffer， int channels\_mask， int mask\_channel， int mask\_value ）

Paste voxels in a box from the given buffer at a specific location. Voxels having a specific value in a mask channel will not be pasted.  
将体素粘贴到给定缓冲区中特定位置的框中。不会粘贴在掩码通道中具有特定值的体素。

`dst_pos` is the lowest corner of the box, and its size is determined by the size of `src_buffer`.  
`dst_pos` 是框的最低角，其大小由 的大小 `src_buffer` 决定。

`channels_mask` is a bitmask where each bit tells which channels will be modified. Example: `1 << VoxelBuffer.CHANNEL_SDF` only write SDF data. Use `0xff` if you want them all.  
`channels_mask` 是一个位掩码，其中每个位都指示将修改哪些通道。示例： `1 << VoxelBuffer.CHANNEL_SDF` 仅写入 SDF 数据。 `0xff` 如果您想要它们，请使用它们。

`src_mask_channel` channel that will be used to lookup mask values.  
`src_mask_channel` 将用于查找掩码值的通道。

`src_mask_value` if voxels have this value in the channel specified for masking, then they won't be pasted.  
`src_mask_value` 如果体素在为遮罩指定的通道中具有此值，则不会粘贴它们。

-   [VoxelRaycastResult](https://voxel-tools.readthedocs.io/en/latest/api/VoxelRaycastResult/) **raycast**( [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) origin, [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) direction, [float](https://docs.godotengine.org/en/stable/classes/class_float.html) max\_distance=10.0, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) collision\_mask=4294967295 )  
    体素光线投射结果雷投射（ 矢量3 原点， 矢量3 方向， 浮点数 max\_distance=10.0， int collision\_mask=4294967295 ）

Runs a voxel-based raycast to find the first hit from an origin and a direction.  
运行基于体素的光线投射，以查找来自原点和方向的第一个命中。

Returns a result object if a voxel got hit, otherwise returns `null`.  
如果体素被命中，则返回结果对象，否则返回 `null` 。

This is useful when colliders cannot be relied upon. It might also be faster (at least at short range), and is more precise to find which voxel is hit. It internally uses the DDA algorithm.  
当不能依赖碰撞体时，这很有用。它也可能更快（至少在短距离内），并且更精确地找到被击中的体素。它在内部使用 DDA 算法。

`collision_mask` is currently only used with blocky voxels. It is combined with [VoxelBlockyModel.collision\_mask](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModel/#i_collision_mask) to decide which voxel types the ray can collide with.  
`collision_mask` 目前仅与块状体素一起使用。它与VoxelBlockyModel.collision\_mask相结合，以决定光线可以与哪种体素类型碰撞。

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#) **set\_voxel**( [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) pos, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) v )  
    voidset\_voxel（ Vector3i pos， int v ）

Sets the raw integer value of a specific voxel on the current channel.  
设置当前通道上特定体素的原始整数值。

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#) **set\_voxel\_f**( [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) pos, [float](https://docs.godotengine.org/en/stable/classes/class_float.html) v )  
    voidset\_voxel\_f（ Vector3i pos， float v ）

Sets the normalized decimal value of a specific voxel. This should preferably be used when modifying voxels on the SDF channel.  
设置特定体素的规范化十进制值。在修改 SDF 通道上的体素时，最好使用此方法。

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#) **set\_voxel\_metadata**( [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) pos, [Variant](https://docs.godotengine.org/en/stable/classes/class_variant.html) meta )  
    voidset\_voxel\_metadata（ Vector3i pos， Variant meta ）
    
-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/#)
    
    **smooth\_sphere**( [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) sphere\_center, [float](https://docs.godotengine.org/en/stable/classes/class_float.html) sphere\_radius, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) blur\_radius )  
    voidsmooth\_sphere（ 矢量3 sphere\_center， 浮点sphere\_radius， 整数 blur\_radius ）

Smoothens out terrain by performing box blur in a spherical area. Strength will be maximal at the center of the sphere, and decreases linearly to zero at the surface of the sphere. Voxels outside the sphere will not be affected.  
通过在球形区域中执行方框模糊来平滑地形。强度在球体中心处最大，在球体表面线性降低至零。球体外的体素不会受到影响。

`sphere_center` is position in the terrain that will be smoothed out.  
`sphere_center` 是将平滑的地形中的位置。

`sphere_radius` radius of a sphere from the `center` where voxel values will be affected. Should be greater than zero.  
`sphere_radius` 球体的半径从 `center` 体素值将受到影响的位置开始。应大于零。

`blur_radius` half the box blur length that will be sampled to calculate average voxel values. Higher values results in more aggressive smoothing. Should be at least 1.  
`blur_radius` 将采样以计算平均体素值的框模糊长度的一半。值越高，平滑效果越强。应至少为 1。

Note 1: This is currently implemented only for terrain that uses SDF data (smooth voxels).  
注 1：目前仅适用于使用 SDF 数据（平滑体素）的地形。

Note 2: Beware of using high `sphere_radius` and high `blur_radius` as the performance can drop quickly if this is called 60 times a second.  
注意2：当心使用高 `sphere_radius` 和高， `blur_radius` 因为如果每秒调用60次，性能会迅速下降。

-   [Vector4i](https://docs.godotengine.org/en/stable/classes/class_vector4i.html) **u16\_indices\_to\_vec4i**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) \_unnamed\_arg0 )  
    Vector4iu16\_indices\_to\_vec4i（ 国际 \_unnamed\_arg0 ）

Decodes raw voxel integer data from the INDICES channel into a 4-integer vector.  
将来自 INDICES 通道的原始体素整数数据解码为 4 整数向量。

-   [Color](https://docs.godotengine.org/en/stable/classes/class_color.html) **u16\_weights\_to\_color**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) \_unnamed\_arg0 )  
    Coloru16\_weights\_to\_color（ 国际 \_unnamed\_arg0 ）

Decodes raw voxel integer data from the WEIGHTS channel into a normalized 4-float color.  
将来自 WEIGHTS 通道的原始体素整数数据解码为规范化的 4 浮点颜色。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **vec4i\_to\_u16\_indices**( [Vector4i](https://docs.godotengine.org/en/stable/classes/class_vector4i.html) \_unnamed\_arg0 )  
    intvec4i\_to\_u16\_indices（ 矢量4i \_unnamed\_arg0 ）

Encodes a 4-integer vector into 16-bit integer voxel data, for use in the INDICES channel.  
将 4 整数矢量编码为 16 位整数体素数据，以便在 INDICES 通道中使用。

_Generated on Sep 12, 2023  
生成于 Sep 12， 2023_
