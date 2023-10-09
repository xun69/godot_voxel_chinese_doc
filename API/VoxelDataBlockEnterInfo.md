# VoxelDataBlockEnterInfo体素数据块输入信息

> ## Excerpt
> 继承：对象

---
##   
体素数据块输入信息

 继承：对象

  
当地形的一个数据块进入体素查看器区域时，地形发送的信息。

##  说明：

  
当地形的一个数据块进入体素查看器区域时，地形发送的信息。请参阅VoxelTerrain.\_on\_data\_block\_entered。

  
不得存储此类的实例，因为它们在调用后将变得无效。

##  方法：

|  返回 |  签名 |
| --- | --- |
|  [布尔](https://docs.godotengine.org/en/stable/classes/class_bool.html) |   
are\_voxels\_edited （ ） 常量 |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) |   
get\_lod\_index （ ） 常量 |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) |   
get\_network\_peer\_id （ ） 常量 |
|  [矢量3i](https://docs.godotengine.org/en/stable/classes/class_vector3i.html) |   
get\_position （ ） 常量 |
|  [体素缓冲器](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) |   
get\_voxels （ ） 常量 |

##  方法说明

-     
    boolare\_voxels\_edited（ ）

  
告知块中的体素是否曾经被编辑过。如果不是，则意味着可以通过运行生成器获得相同的数据。

-    intget\_lod\_index（ ）

  
获取数据块所在的 LOD 索引。

-     
    intget\_network\_peer\_id（ ）

  
获取导致块被引用的体素查看器的网络对等 ID。

-     
    Vector3iget\_position（ ）

  
获取数据块在数据块坐标中的位置（体素坐标是通过将这些坐标乘以数据块大小获得的）。

-     
    VoxelBufferget\_voxels（ ）

  
获取对块中体素的访问权限。

_  
生成于 Oct 02， 2023_
