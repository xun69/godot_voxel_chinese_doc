---
created: 2023-09-27T00:01:21 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/
author: 
---

# VoxelBuffer体素缓冲区

> ## Excerpt
> Inherits: RefCounted 继承：引用计数

---
Inherits: [RefCounted](https://docs.godotengine.org/en/stable/classes/class_refcounted.html) 继承：引用计数

3D grid storing voxel data.  
存储体素数据的 3D 网格。

## Description: 说明：

This contains dense voxels data storage (every single cell holds data, there is no sparse optimization of space). Works like a normal 3D grid containing a voxel value in each cell. Organized in channels of configurable bit depth. Values can be interpreted either as unsigned integers or normalized floats. See [VoxelBuffer.Depth](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#enumerations) for more information.  
这包含密集的体素数据存储（每个单元格都保存数据，没有空间的稀疏优化）。工作方式类似于每个单元格中包含体素值的普通 3D 网格。组织在可配置位深度的通道中。值可以解释为无符号整数或规范化浮点数。有关更多信息，请参阅 VoxelBuffer.Depth。

Arbitrary metadata can also be stored, either for the whole buffer, or per-voxel, at higher cost. This metadata can get saved and loaded along voxels, however you must make sure the data is serializable (i.e it should not contain nodes or arbitrary objects).  
还可以存储任意元数据，无论是整个缓冲区还是每个体素，成本更高。此元数据可以沿体素保存和加载，但是必须确保数据是可序列化的（即它不应包含节点或任意对象）。

## Methods: 方法：

| Return 返回 | Signature 签名 |
| --- | --- |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) | [clear](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#i_clear) ( ) 清除 （ ） |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) | [clear\_voxel\_metadata](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#i_clear_voxel_metadata) ( )  
clear\_voxel\_metadata （ ） |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) | [clear\_voxel\_metadata\_in\_area](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#i_clear_voxel_metadata_in_area) ( [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) min\_pos, [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) max\_pos )  
clear\_voxel\_metadata\_in\_area （ Vector3i min\_pos， Vector3i max\_pos ） |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) | [compress\_uniform\_channels](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#i_compress_uniform_channels) ( )  
compress\_uniform\_channels （ ） |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) | [copy\_channel\_from](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#i_copy_channel_from) ( [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) other, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) channel )  
copy\_channel\_from （ 体素缓冲器其他， int 通道 ） |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) | [copy\_channel\_from\_area](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#i_copy_channel_from_area) ( [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) other, [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) src\_min, [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) src\_max, [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) dst\_min, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) channel )  
copy\_channel\_from\_area （ 体素缓冲区 其他， Vector3i src\_min， Vector3i src\_max， Vector3i dst\_min， int channel ） |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) | [copy\_voxel\_metadata\_in\_area](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#i_copy_voxel_metadata_in_area) ( [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) src\_buffer, [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) src\_min\_pos, [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) src\_max\_pos, [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) dst\_min\_pos )  
copy\_voxel\_metadata\_in\_area （ 体素缓冲区 src\_buffer， Vector3i src\_min\_pos， Vector3i src\_max\_pos， Vector3i dst\_min\_pos ） |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) | [create](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#i_create) ( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) sx, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) sy, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) sz )  
create （ int sx， int sy， int sz ） |
| [Array 数组](https://docs.godotengine.org/en/stable/classes/class_array.html) | [debug\_print\_sdf\_y\_slices](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#i_debug_print_sdf_y_slices) ( [float](https://docs.godotengine.org/en/stable/classes/class_float.html) scale ) const  
debug\_print\_sdf\_y\_slices （浮子刻度） 常量 |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) | [downscale\_to](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#i_downscale_to) ( [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) dst, [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) src\_min, [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) src\_max, [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) dst\_min ) const  
downscale\_to （ VoxelBuffer dst， Vector3i src\_min， Vector3i src\_max， Vector3i dst\_min ） const |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) | [fill](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#i_fill) ( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) value, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) channel=0 )  
填充 （ 整数值， 整数通道=0 ） |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) | [fill\_area](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#i_fill_area) ( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) value, [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) min, [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) max, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) channel=0 )  
fill\_area （ 整数值， 矢量3i 最小值， 矢量3i 最大值， 整数通道=0 ） |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) | [fill\_f](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#i_fill_f) ( [float](https://docs.godotengine.org/en/stable/classes/class_float.html) value, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) channel=0 )  
fill\_f （浮点值， 整数通道=0 ） |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) | [for\_each\_voxel\_metadata](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#i_for_each_voxel_metadata) ( [Callable](https://docs.godotengine.org/en/stable/classes/class_callable.html) callback ) const  
for\_each\_voxel\_metadata （ 可调用回调 ） 常量 |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) | [for\_each\_voxel\_metadata\_in\_area](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#i_for_each_voxel_metadata_in_area) ( [Callable](https://docs.godotengine.org/en/stable/classes/class_callable.html) callback, [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) min\_pos, [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) max\_pos )  
for\_each\_voxel\_metadata\_in\_area （ 可调用回调， Vector3i min\_pos， Vector3i max\_pos ） |
| [Variant 变体](https://docs.godotengine.org/en/stable/classes/class_variant.html) | [get\_block\_metadata](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#i_get_block_metadata) ( ) const  
get\_block\_metadata （ ） 常量 |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) | [get\_channel\_compression](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#i_get_channel_compression) ( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) channel ) const  
get\_channel\_compression （ int channel ） const |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) | [get\_channel\_depth](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#i_get_channel_depth) ( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) channel ) const  
get\_channel\_depth （ int channel ） const |
| [Vector3i 矢量3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) | [get\_size](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#i_get_size) ( ) const  
get\_size （ ） 常量 |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) | [get\_voxel](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#i_get_voxel) ( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) x, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) y, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) z, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) channel=0 ) const  
get\_voxel （ int x， int y， int z， int channel=0 ） const |
| [float 浮](https://docs.godotengine.org/en/stable/classes/class_float.html) | [get\_voxel\_f](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#i_get_voxel_f) ( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) x, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) y, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) z, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) channel=0 ) const  
get\_voxel\_f （ int x， int y， int z， int channel=0 ） const |
| [Variant 变体](https://docs.godotengine.org/en/stable/classes/class_variant.html) | [get\_voxel\_metadata](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#i_get_voxel_metadata) ( [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) pos ) const  
get\_voxel\_metadata （ Vector3i pos ） const |
| [VoxelTool 体素工具](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/) | [get\_voxel\_tool](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#i_get_voxel_tool) ( ) get\_voxel\_tool （ ） |
| [bool 布尔](https://docs.godotengine.org/en/stable/classes/class_bool.html) | [is\_uniform](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#i_is_uniform) ( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) channel ) const  
is\_uniform （ int channel ） const |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) | [optimize](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#i_optimize) ( ) 优化 （ ） |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) | [remap\_values](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#i_remap_values) ( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) channel, [PackedInt32Array](https://docs.godotengine.org/en/stable/classes/class_packedint32array.html) map )  
remap\_values （ int channel， PackedInt32Array map ） |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) | [set\_block\_metadata](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#i_set_block_metadata) ( [Variant](https://docs.godotengine.org/en/stable/classes/class_variant.html) meta )  
set\_block\_metadata （ 变种元 ） |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) | [set\_channel\_depth](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#i_set_channel_depth) ( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) channel, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) depth )  
set\_channel\_depth （ int 通道， int 深度 ） |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) | [set\_voxel](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#i_set_voxel) ( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) value, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) x, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) y, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) z, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) channel=0 )  
set\_voxel （ int 值， int x， int y， int z， int channel=0 ） |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) | [set\_voxel\_f](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#i_set_voxel_f) ( [float](https://docs.godotengine.org/en/stable/classes/class_float.html) value, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) x, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) y, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) z, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) channel=0 )  
set\_voxel\_f （ 浮点值， 整数 x， 整数 y， 整数 z， 整数通道=0 ） |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) | [set\_voxel\_metadata](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#i_set_voxel_metadata) ( [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) pos, [Variant](https://docs.godotengine.org/en/stable/classes/class_variant.html) value )  
set\_voxel\_metadata （ Vector3i pos， 变量值 ） |
| [void 无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) | [set\_voxel\_v](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#i_set_voxel_v) ( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) value, [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) pos, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) channel=0 )  
set\_voxel\_v （ int 值， Vector3i pos， int channel=0 ） |

## Enumerations: 枚举：

enum **ChannelId**:  枚举通道 ID：

-   **CHANNEL\_TYPE** = **0** --- Channel used to store voxel types. Used by \[VoxelMesherBlocky\].  
    CHANNEL\_TYPE = 0 --- 用于存储体素类型的通道。由\[VoxelMesherBlocky\]使用。
-   **CHANNEL\_SDF** = **1** --- Channel used to store SDF data (signed distance field). Used by \[VoxelMesherTransvoxel\] and other smooth meshers. Values should preferably be accessed as floats. Negative values are below the isosurface (inside matter), and positive values are above the surface (outside matter).  
    CHANNEL\_SDF = 1 --- 用于存储 SDF 数据的通道（有符号距离字段）。由\[VoxelMesherTransvoxel\]和其他平滑网格划分器使用。值最好作为浮点数访问。负值在等值表面以下（物质内部），正值在表面上方（物质外部）。
-   **CHANNEL\_COLOR** = **2** --- Channel used to store color data. Used by \[VoxelMesherCubes\].  
    CHANNEL\_COLOR = 2 --- 用于存储颜色数据的通道。由\[VoxelMesherCubes\]使用。
-   **CHANNEL\_INDICES** = **3**
-   **CHANNEL\_WEIGHTS** = **4**
-   **CHANNEL\_DATA5** = **5** --- Free channel. Not used by the engine yet.  
    CHANNEL\_DATA5 = 5 --- 个免费频道。尚未被引擎使用。
-   **CHANNEL\_DATA6** = **6** --- Free channel. Not used by the engine yet.  
    CHANNEL\_DATA6 = 6 --- 免费频道。尚未被引擎使用。
-   **CHANNEL\_DATA7** = **7** --- Free channel. Not used by the engine yet.  
    CHANNEL\_DATA7 = 7 --- 个免费频道。尚未被引擎使用。
-   **MAX\_CHANNELS** = **8** --- Maximum number of channels a \[VoxelBuffer\] can have.  
    MAX\_CHANNELS = 8 --- \[体素缓冲区\] 可以具有的最大通道数。

enum **Depth**:  枚举深度：

-   **DEPTH\_8\_BIT** = **0** --- Voxels will be stored with 8 bits. Raw values will range from 0 to 255, and float values will be normalized between -1 and 1 (but will still take 255 possible values). Values outside the range will be clamped. If you use this for smooth voxels, you may take care of scaling SDF data with a small number like 0.1 to reduce precision artifacts.  
    DEPTH\_8\_BIT = 0 ---体素将以 8 位存储。原始值的范围为 0 到 255，浮点值将在 -1 和 1 之间规范化（但仍需要 255 个可能的值）。超出范围的值将被钳制。如果将其用于平滑体素，则可以使用较小的数字（如 0.1）缩放 SDF 数据以减少精度伪影。
-   **DEPTH\_16\_BIT** = **1** --- Voxels will be stored with 16 bits. Raw values will range from 0 to 65,535, and float values will be normalized between -1 and 1 (but will still take 65535 possible values). Values outside the range will be clamped.  
    DEPTH\_16\_BIT = 1 ---体素将以 16 位存储。原始值的范围为 0 到 65,535，浮点值将在 -1 和 1 之间规范化（但仍需要 65535 个可能的值）。超出范围的值将被钳制。
-   **DEPTH\_32\_BIT** = **2** --- Voxels will be stored with 32 bits. Raw values will range from 0 to 4,294,967,295, and float values will use regular IEEE 754 representation (`float`).  
    DEPTH\_32\_BIT = 2 ---体素将以 32 位存储。原始值的范围为 0 到 4,294,967,295，浮点值将使用常规 IEEE 754 表示形式 （ `float` ）。
-   **DEPTH\_64\_BIT** = **3** --- Voxels will be stored with 64 bits. Raw values will range from 0 to 18,446,744,073,709,551,615, and float values will use regular IEEE 754 representation (`double`).  
    DEPTH\_64\_BIT = 3 ---体素将以 64 位存储。原始值的范围为 0 到 18,446,744,073,709,551,615，浮点值将使用常规 IEEE 754 表示形式 （ `double` ）。
-   **DEPTH\_COUNT** = **4** --- How many depth configuration there are.  
    DEPTH\_COUNT = 4 ---有多少深度配置。

enum **Compression**:  枚举压缩：

-   **COMPRESSION\_NONE** = **0** --- The channel is not compressed. Every value is stored individually inside an array in memory.  
    COMPRESSION\_NONE = 0 --- 通道未压缩。每个值都单独存储在内存中的数组中。
-   **COMPRESSION\_UNIFORM** = **1** --- All voxels of the channel have the same value, so they are stored as one single value, to save space.  
    COMPRESSION\_UNIFORM = 1 --- 通道的所有体素都具有相同的值，因此它们存储为单个值，以节省空间。
-   **COMPRESSION\_COUNT** = **2** --- How many compression modes there are.  
    COMPRESSION\_COUNT = 2 ---有多少种压缩模式。

## Constants: 常量：

-   **MAX\_SIZE** = **65535**

## Method Descriptions 方法说明

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) **clear**( )  空清（ ）

Erases all contents of the buffer and resets its size to zero. Channel depths and default values are preserved.  
擦除缓冲区的所有内容并将其大小重置为零。通道深度和默认值将保留。

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) **clear\_voxel\_metadata**( )  
    voidclear\_voxel\_metadata（ ）

Erases all per-voxel metadata.  
擦除所有每体素元数据。

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) **clear\_voxel\_metadata\_in\_area**( [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) min\_pos, [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) max\_pos )  
    voidclear\_voxel\_metadata\_in\_area（ Vector3i min\_pos， Vector3i max\_pos ）

Erases per-voxel metadata within the specified area.  
擦除指定区域内的每体素元数据。

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) **compress\_uniform\_channels**( )  
    voidcompress\_uniform\_channels（ ）

Finds channels that have the same value in all their voxels, and reduces memory usage by storing only one value instead. This is effective for example when large parts of the terrain are filled with air.  
查找在其所有体素中具有相同值的通道，并通过仅存储一个值来减少内存使用量。例如，当大部分地形充满空气时，这是有效的。

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) **copy\_channel\_from**( [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) other, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) channel )  
    voidcopy\_channel\_from（ 体素缓冲器其他， int 通道 ）

Copies all values from the channel of another [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) into the same channel for the current buffer. The depth formats must match.  
将所有值从另一个体素缓冲区的通道复制到当前缓冲区的同一通道中。深度格式必须匹配。

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) **copy\_channel\_from\_area**( [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) other, [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) src\_min, [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) src\_max, [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) dst\_min, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) channel )  
    voidcopy\_channel\_from\_area（ 体素缓冲区 其他， Vector3i src\_min， Vector3i src\_max， Vector3i dst\_min， int channel ）

Copies values from a channel's sub-region of another [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) into the same channel for the current buffer, at a specific location. The depth formats must match.  
将另一个体素缓冲区的通道子区域中的值复制到当前缓冲区的同一通道的特定位置。深度格式必须匹配。

If corners of the area represent a negative-size area, they will be sorted back.  
如果该区域的角表示负大小区域，则它们将被排序回去。

If coordinates are entirely or partially out of bounds, they will be clipped automatically.  
如果坐标完全或部分超出边界，它们将被自动裁剪。

Copying across the same buffer to overlapping areas is not supported. You may use an intermediary buffer in this case.  
不支持跨同一缓冲区复制到重叠区域。在这种情况下，您可以使用中间缓冲区。

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) **copy\_voxel\_metadata\_in\_area**( [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) src\_buffer, [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) src\_min\_pos, [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) src\_max\_pos, [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) dst\_min\_pos )  
    voidcopy\_voxel\_metadata\_in\_area（ 体素缓冲区 src\_buffer， Vector3i src\_min\_pos， Vector3i src\_max\_pos， Vector3i dst\_min\_pos ）

Copies per-voxel metadata from a sub-region of another [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) into the the current buffer, at a specific location. Values will be a shallow copy.  
将每个体素元数据从另一个体素缓冲区的子区域复制到当前缓冲区的特定位置。值将是浅拷贝。

If corners of the area represent a negative-size area, they will be sorted back.  
如果该区域的角表示负大小区域，则它们将被排序回去。

If coordinates are entirely or partially out of bounds, they will be clipped automatically.  
如果坐标完全或部分超出边界，它们将被自动裁剪。

Copying across the same buffer to overlapping areas is not supported. You may use an intermediary buffer in this case.  
不支持跨同一缓冲区复制到重叠区域。在这种情况下，您可以使用中间缓冲区。

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) **create**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) sx, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) sy, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) sz )  
    voidcreate（ int sx， int sy， int sz ）

Clears the buffer and gives it the specified size.  
清除缓冲区并为其指定大小。

-   [Array](https://docs.godotengine.org/en/stable/classes/class_array.html) **debug\_print\_sdf\_y\_slices**( [float](https://docs.godotengine.org/en/stable/classes/class_float.html) scale )  
    Arraydebug\_print\_sdf\_y\_slices（浮子秤）
    
-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) **downscale\_to**( [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) dst, [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) src\_min, [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) src\_max, [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) dst\_min )  
    voiddownscale\_to（ VoxelBuffer dst， Vector3i src\_min， Vector3i src\_max， Vector3i dst\_min ）
    

Produces a downscaled version of this buffer, by a factor of 2, without any form of interpolation (i.e using nearest-neighbor).  
生成此缓冲区的缩小版本，系数为 2，无需任何形式的插值（即使用最近邻）。

Metadata is not copied.  
不复制元数据。

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) **fill**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) value, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) channel=0 )  
    voidfill（ int value， int channel=0 ）

Fills one channel of this buffer with a specific raw value.  
用特定的原始值填充此缓冲区的一个通道。

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) **fill\_area**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) value, [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) min, [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) max, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) channel=0 )  
    voidfill\_area（ int 值， 矢量 3i 最小值， 矢量 3i 最大值， 整数通道=0 ）

Fills an area of a channel in this buffer with a specific raw value.  
用特定的原始值填充此缓冲区中通道的某个区域。

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) **fill\_f**( [float](https://docs.godotengine.org/en/stable/classes/class_float.html) value, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) channel=0 )  
    voidfill\_f（浮点值，整数通道=0）

Fills one channel of this buffer with a specific float value.  
用特定的浮点值填充此缓冲区的一个通道。

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) **for\_each\_voxel\_metadata**( [Callable](https://docs.godotengine.org/en/stable/classes/class_callable.html) callback )  
    voidfor\_each\_voxel\_metadata（ 可调用回调 ）

Executes a function on every voxel in this buffer which have associated metadata.  
在此缓冲区中具有关联元数据的每个体素上执行函数。

The function's arguments must be (position: Vector3i, metadata: Variant).  
函数的参数必须是（位置：Vector3i，元数据：变体）。

IMPORTANT: inserting new or removing metadata from inside this function is not allowed.  
重要说明：不允许在此函数中插入新元数据或删除元数据。

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) **for\_each\_voxel\_metadata\_in\_area**( [Callable](https://docs.godotengine.org/en/stable/classes/class_callable.html) callback, [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) min\_pos, [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) max\_pos )  
    voidfor\_each\_voxel\_metadata\_in\_area（ 可调用回调， Vector3i min\_pos， Vector3i max\_pos ）

Executes a function on every voxel in this buffer which have associated metadata, within the specified area.  
在此缓冲区中具有指定区域内关联元数据的每个体素上执行函数。

-   [Variant](https://docs.godotengine.org/en/stable/classes/class_variant.html) **get\_block\_metadata**( )  
    Variantget\_block\_metadata（ ）

Gets metadata associated to this [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/).  
获取与此体素缓冲区关联的元数据。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **get\_channel\_compression**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) channel )  
    intget\_channel\_compression（ 整数频道 ）

Gets which compression mode the specified channel has.  
获取指定通道具有的压缩模式。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **get\_channel\_depth**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) channel )  
    intget\_channel\_depth（ 整数通道 ）

Gets which bit depth the specified channel has.  
获取指定通道具有的位深度。

-   [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) **get\_size**( )  Vector3iget\_size（ ）

Gets the 3D size of the buffer in voxels.  
获取缓冲区的 3D 大小（以体素为单位）。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **get\_voxel**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) x, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) y, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) z, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) channel=0 )  
    intget\_voxel（ int x， int y， int z， int channel=0 ）

Gets the raw value of a voxel within this buffer.  
获取此缓冲区内体素的原始值。

-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **get\_voxel\_f**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) x, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) y, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) z, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) channel=0 )  
    floatget\_voxel\_f（ int x， int y， int z， int channel=0 ）

Gets the float value of a voxel within this buffer. You may use this function if you work with SDF volumes (smooth voxels).  
获取此缓冲区内体素的浮点值。如果使用 SDF 体积（平滑体素），则可以使用此函数。

-   [Variant](https://docs.godotengine.org/en/stable/classes/class_variant.html) **get\_voxel\_metadata**( [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) pos )  
    Variantget\_voxel\_metadata（ Vector3i pos ）

Gets the metadata attached to a specific voxel in this buffer.  
获取附加到此缓冲区中特定体素的元数据。

-   [VoxelTool](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/) **get\_voxel\_tool**( )  
    VoxelToolget\_voxel\_tool（ ）

Constructs a [VoxelTool](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/) instance bound to this buffer. This provides access to some extra common functions.  
构造绑定到此缓冲区的体素工具实例。这提供了对一些额外的常见功能的访问。

-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **is\_uniform**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) channel )  
    boolis\_uniform（ 整频道 ）

Checks if every voxel within a channel has the same value.  
检查通道中的每个体素是否具有相同的值。

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) **optimize**( )  虚空优化（ ）
    
-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#)
    
    **remap\_values**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) channel, [PackedInt32Array](https://docs.godotengine.org/en/stable/classes/class_packedint32array.html) map )  
    voidremap\_values（ int channel， PackedInt32Array map ）
-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) **set\_block\_metadata**( [Variant](https://docs.godotengine.org/en/stable/classes/class_variant.html) meta )  
    voidset\_block\_metadata（ 变种元 ）
    

Sets arbitrary data on this buffer. Old data is replaced. Note, this is separate storage from per-voxel metadata.  
设置此缓冲区上的任意数据。替换旧数据。请注意，这是与每体素元数据分开的存储。

If this [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) is saved, this metadata will also be saved along voxels, so make sure the data supports serialization (i.e you can't put nodes or arbitrary objects in it).  
如果保存了此体素缓冲区，则此元数据也将沿体素保存，因此请确保数据支持序列化（即不能在其中放置节点或任意对象）。

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) **set\_channel\_depth**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) channel, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) depth )  
    voidset\_channel\_depth（ int channel， int depth ）

Changes the bit depth of a given channel. This controls the range of values a channel can hold. See [VoxelBuffer.Depth](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#enumerations) for more information.  
更改给定通道的位深度。这控制通道可以容纳的值范围。有关更多信息，请参阅 VoxelBuffer.Depth。

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) **set\_voxel**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) value, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) x, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) y, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) z, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) channel=0 )  
    voidset\_voxel（ int value， int x， int y， int z， int channel=0 ）

Sets the raw value of a voxel. If you use smooth voxels, you may prefer using [VoxelBuffer.set\_voxel\_f](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#i_set_voxel_f).  
设置体素的原始值。如果使用平滑体素，则可能更喜欢使用VoxelBuffer.set\_voxel\_f。

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) **set\_voxel\_f**( [float](https://docs.godotengine.org/en/stable/classes/class_float.html) value, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) x, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) y, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) z, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) channel=0 )  
    voidset\_voxel\_f（ 浮点值， 整数 x， 整数 y， 整数 z， 整数通道=0 ）

Sets the float value of a voxel. This method should be used if you work on SDF data (smooth voxels).  
设置体素的浮点值。如果处理 SDF 数据（平滑体素），则应使用此方法。

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) **set\_voxel\_metadata**( [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) pos, [Variant](https://docs.godotengine.org/en/stable/classes/class_variant.html) value )  
    voidset\_voxel\_metadata（ Vector3i pos， 变量值 ）

Attaches arbitrary data on a specific voxel. Old data is replaced.  
在特定体素上附加任意数据。替换旧数据。

If this [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) is saved, this metadata will also be saved along voxels, so make sure the data supports serialization (i.e you can't put nodes or arbitrary objects in it).  
如果保存了此体素缓冲区，则此元数据也将沿体素保存，因此请确保数据支持序列化（即不能在其中放置节点或任意对象）。

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) **set\_voxel\_v**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) value, [Vector3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) pos, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) channel=0 )  
    voidset\_voxel\_v（ int value， Vector3i pos， int channel=0 ）

_Generated on Sep 12, 2023  
生成于 Sep 12， 2023_
