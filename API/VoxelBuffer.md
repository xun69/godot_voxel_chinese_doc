# VoxelBuffer体素缓冲区

> ## Excerpt
> 继承：引用计数

---
##  体素缓冲区

 继承：引用计数

  
存储体素数据的 3D 网格。

##  说明：

  
这包含密集的体素数据存储（每个单元格都保存数据，没有空间的稀疏优化）。工作方式类似于每个单元格中包含体素值的普通 3D 网格。组织在可配置位深度的通道中。值可以解释为无符号整数或规范化浮点数。有关更多信息，请参阅 VoxelBuffer.Depth。

  
还可以存储任意元数据，无论是整个缓冲区还是每个体素，成本更高。此元数据可以沿体素保存和加载，但是必须确保数据是可序列化的（即它不应包含节点或任意对象）。

##  方法：

|  返回 |  签名 |
| --- | --- |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) |  清除 （ ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) |   
clear\_voxel\_metadata （ ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) |   
clear\_voxel\_metadata\_in\_area （ Vector3i min\_pos， Vector3i max\_pos ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) |   
compress\_uniform\_channels （ ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) |   
copy\_channel\_from （ 体素缓冲器其他， int 通道 ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) |   
copy\_channel\_from\_area （ 体素缓冲区 其他， Vector3i src\_min， Vector3i src\_max， Vector3i dst\_min， int channel ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) |   
copy\_voxel\_metadata\_in\_area （ 体素缓冲区 src\_buffer， Vector3i src\_min\_pos， Vector3i src\_max\_pos， Vector3i dst\_min\_pos ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) |   
create （ int sx， int sy， int sz ） |
|  [数组](https://docs.godotengine.org/en/stable/classes/class_array.html) |   
debug\_print\_sdf\_y\_slices （浮子刻度） 常量 |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) |   
downscale\_to （ VoxelBuffer dst， Vector3i src\_min， Vector3i src\_max， Vector3i dst\_min ） const |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) |   
填充 （ 整数值， 整数通道=0 ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) |   
fill\_area （ 整数值， 矢量3i 最小值， 矢量3i 最大值， 整数通道=0 ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) |   
fill\_f （浮点值， 整数通道=0 ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) |   
for\_each\_voxel\_metadata （ 可调用回调 ） 常量 |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) |   
for\_each\_voxel\_metadata\_in\_area （ 可调用回调， Vector3i min\_pos， Vector3i max\_pos ） |
|  [变体](https://docs.godotengine.org/en/stable/classes/class_variant.html) |   
get\_block\_metadata （ ） 常量 |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) |   
get\_channel\_compression （ int channel ） const |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) |   
get\_channel\_depth （ int channel ） const |
|  [矢量3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) |   
get\_size （ ） 常量 |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) |   
get\_voxel （ int x， int y， int z， int channel=0 ） const |
|  [浮](https://docs.godotengine.org/en/stable/classes/class_float.html) |   
get\_voxel\_f （ int x， int y， int z， int channel=0 ） const |
|  [变体](https://docs.godotengine.org/en/stable/classes/class_variant.html) |   
get\_voxel\_metadata （ Vector3i pos ） const |
|  [体素工具](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/) |  get\_voxel\_tool （ ） |
|  [布尔](https://docs.godotengine.org/en/stable/classes/class_bool.html) |   
is\_uniform （ int channel ） const |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) |  优化 （ ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) |   
remap\_values （ int channel， PackedInt32Array map ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) |   
set\_block\_metadata （ 变种元 ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) |   
set\_channel\_depth （ int 通道， int 深度 ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) |   
set\_voxel （ int 值， int x， int y， int z， int channel=0 ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) |   
set\_voxel\_f （ 浮点值， 整数 x， 整数 y， 整数 z， 整数通道=0 ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) |   
set\_voxel\_metadata （ Vector3i pos， 变量值 ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/#) |   
set\_voxel\_v （ int 值， Vector3i pos， int channel=0 ） |

##  枚举：

 枚举通道 ID：

-     
    CHANNEL\_TYPE = 0 --- 用于存储体素类型的通道。由VoxelMesherBlocky使用。
-     
    CHANNEL\_SDF = 1 --- 用于存储 SDF 数据的通道（有符号距离字段）。由VoxelMesherTransvoxel和其他平滑网格划分器使用。值最好作为浮点数访问。负值在等值表面以下（物质内部），正值在表面上方（物质外部）。
-     
    CHANNEL\_COLOR = 2 --- 用于存储颜色数据的通道。由VoxelMesherCubes使用。
-   **CHANNEL\_INDICES** = **3**
-   **CHANNEL\_WEIGHTS** = **4**
-     
    CHANNEL\_DATA5 = 5 --- 个免费频道。尚未被引擎使用。
-     
    CHANNEL\_DATA6 = 6 --- 免费频道。尚未被引擎使用。
-     
    CHANNEL\_DATA7 = 7 --- 个免费频道。尚未被引擎使用。
-     
    MAX\_CHANNELS = 8 --- 体素缓冲区可以具有的最大通道数。

 枚举深度：

-     
    DEPTH\_8\_BIT = 0 ---体素将以 8 位存储。原始值的范围为 0 到 255，浮点值将在 -1 和 1 之间规范化（但仍需要 255 个可能的值）。超出范围的值将被钳制。如果将其用于平滑体素，则可以使用较小的数字（如 0.1）缩放 SDF 数据以减少精度伪影。
-     
    DEPTH\_16\_BIT = 1 ---体素将以 16 位存储。原始值的范围为 0 到 65,535，浮点值将在 -1 和 1 之间规范化（但仍需要 65535 个可能的值）。超出范围的值将被钳制。
-     
    DEPTH\_32\_BIT = 2 ---体素将以 32 位存储。原始值的范围为 0 到 4,294,967,295，浮点值将使用常规 IEEE 754 表示形式 （ `float` ）。
-     
    DEPTH\_64\_BIT = 3 ---体素将以 64 位存储。原始值的范围为 0 到 18,446,744,073,709,551,615，浮点值将使用常规 IEEE 754 表示形式 （ `double` ）。
-     
    DEPTH\_COUNT = 4 ---有多少深度配置。

 枚举压缩：

-     
    COMPRESSION\_NONE = 0 --- 通道未压缩。每个值都单独存储在内存中的数组中。
-     
    COMPRESSION\_UNIFORM = 1 --- 通道的所有体素都具有相同的值，因此它们存储为单个值，以节省空间。
-     
    COMPRESSION\_COUNT = 2 ---有多少种压缩模式。

##  常量：

-   **MAX\_SIZE** = **65535**

##  方法说明

-    空清（ ）

  
擦除缓冲区的所有内容并将其大小重置为零。通道深度和默认值将保留。

-     
    voidclear\_voxel\_metadata（ ）

  
擦除所有每体素元数据。

-     
    voidclear\_voxel\_metadata\_in\_area（ Vector3i min\_pos， Vector3i max\_pos ）

  
擦除指定区域内的每体素元数据。

-     
    voidcompress\_uniform\_channels（ ）

  
查找在其所有体素中具有相同值的通道，并通过仅存储一个值来减少内存使用量。例如，当大部分地形充满空气时，这是有效的。

-     
    voidcopy\_channel\_from（ 体素缓冲器其他， int 通道 ）

  
将所有值从另一个体素缓冲区的通道复制到当前缓冲区的同一通道中。深度格式必须匹配。

-     
    voidcopy\_channel\_from\_area（ 体素缓冲区 其他， Vector3i src\_min， Vector3i src\_max， Vector3i dst\_min， int channel ）

  
将另一个体素缓冲区的通道子区域中的值复制到当前缓冲区的同一通道的特定位置。深度格式必须匹配。

  
如果该区域的角表示负大小区域，则它们将被排序回去。

  
如果坐标完全或部分超出边界，它们将被自动裁剪。

  
不支持跨同一缓冲区复制到重叠区域。在这种情况下，您可以使用中间缓冲区。

-     
    voidcopy\_voxel\_metadata\_in\_area（ 体素缓冲区 src\_buffer， Vector3i src\_min\_pos， Vector3i src\_max\_pos， Vector3i dst\_min\_pos ）

  
将每个体素元数据从另一个体素缓冲区的子区域复制到当前缓冲区的特定位置。值将是浅拷贝。

  
如果该区域的角表示负大小区域，则它们将被排序回去。

  
如果坐标完全或部分超出边界，它们将被自动裁剪。

  
不支持跨同一缓冲区复制到重叠区域。在这种情况下，您可以使用中间缓冲区。

-     
    voidcreate（ int sx， int sy， int sz ）

  
清除缓冲区并为其指定大小。

-     
    Arraydebug\_print\_sdf\_y\_slices（浮子秤）
    
-     
    voiddownscale\_to（ VoxelBuffer dst， Vector3i src\_min， Vector3i src\_max， Vector3i dst\_min ）
    

  
生成此缓冲区的缩小版本，系数为 2，无需任何形式的插值（即使用最近邻）。

  
不复制元数据。

-     
    voidfill（ int value， int channel=0 ）

  
用特定的原始值填充此缓冲区的一个通道。

-     
    voidfill\_area（ int 值， 矢量 3i 最小值， 矢量 3i 最大值， 整数通道=0 ）

  
用特定的原始值填充此缓冲区中通道的某个区域。

-     
    voidfill\_f（浮点值，整数通道=0）

  
用特定的浮点值填充此缓冲区的一个通道。

-     
    voidfor\_each\_voxel\_metadata（ 可调用回调 ）

  
在此缓冲区中具有关联元数据的每个体素上执行函数。

  
函数的参数必须是（位置：Vector3i，元数据：变体）。

  
重要说明：不允许在此函数中插入新元数据或删除元数据。

-     
    voidfor\_each\_voxel\_metadata\_in\_area（ 可调用回调， Vector3i min\_pos， Vector3i max\_pos ）

  
在此缓冲区中具有指定区域内关联元数据的每个体素上执行函数。

-     
    Variantget\_block\_metadata（ ）

  
获取与此体素缓冲区关联的元数据。

-     
    intget\_channel\_compression（ 整数频道 ）

  
获取指定通道具有的压缩模式。

-     
    intget\_channel\_depth（ 整数通道 ）

  
获取指定通道具有的位深度。

-    Vector3iget\_size（ ）

  
获取缓冲区的 3D 大小（以体素为单位）。

-     
    intget\_voxel（ int x， int y， int z， int channel=0 ）

  
获取此缓冲区内体素的原始值。

-     
    floatget\_voxel\_f（ int x， int y， int z， int channel=0 ）

  
获取此缓冲区内体素的浮点值。如果使用 SDF 体积（平滑体素），则可以使用此函数。

-     
    Variantget\_voxel\_metadata（ Vector3i pos ）

  
获取附加到此缓冲区中特定体素的元数据。

-     
    VoxelToolget\_voxel\_tool（ ）

  
构造绑定到此缓冲区的体素工具实例。这提供了对一些额外的常见功能的访问。

-     
    boolis\_uniform（ 整频道 ）

  
检查通道中的每个体素是否具有相同的值。

-    虚空优化（ ）
    
-     
    voidremap\_values（ int channel， PackedInt32Array map ）
    
-     
    voidset\_block\_metadata（ 变种元 ）
    

  
设置此缓冲区上的任意数据。替换旧数据。请注意，这是与每体素元数据分开的存储。

  
如果保存了此体素缓冲区，则此元数据也将沿体素保存，因此请确保数据支持序列化（即不能在其中放置节点或任意对象）。

-     
    voidset\_channel\_depth（ int channel， int depth ）

  
更改给定通道的位深度。这控制通道可以容纳的值范围。有关更多信息，请参阅 VoxelBuffer.Depth。

-     
    voidset\_voxel（ int value， int x， int y， int z， int channel=0 ）

  
设置体素的原始值。如果使用平滑体素，则可能更喜欢使用VoxelBuffer.set\_voxel\_f。

-     
    voidset\_voxel\_f（ 浮点值， 整数 x， 整数 y， 整数 z， 整数通道=0 ）

  
设置体素的浮点值。如果处理 SDF 数据（平滑体素），则应使用此方法。

-     
    voidset\_voxel\_metadata（ Vector3i pos， 变量值 ）

  
在特定体素上附加任意数据。替换旧数据。

  
如果保存了此体素缓冲区，则此元数据也将沿体素保存，因此请确保数据支持序列化（即不能在其中放置节点或任意对象）。

-     
    voidset\_voxel\_v（ int value， Vector3i pos， int channel=0 ）

_  
生成于 Oct 02， 2023_
