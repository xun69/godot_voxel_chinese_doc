# VoxelGenerator体素生成器

> ## Excerpt
> 继承：资源

---
##  体素生成器

 继承：资源

  
继承者： VoxelGeneratorFlat， VoxelGeneratorGraph， VoxelGeneratorHeightmap， VoxelGeneratorNoise， VoxelGeneratorScript

  
所有体素过程生成器的基类。

##  方法：

|  返回 |  签名 |
| --- | --- |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGenerator/#) |   
generate\_block （ VoxelBuffer out\_buffer， Vector3 origin\_in\_voxels， int lod ） |

##  方法说明

-     
    voidgenerate\_block（ VoxelBuffer out\_buffer， Vector3 origin\_in\_voxels， int lod ）

  
在指定的世界区域内生成体素块。

  
`out_buffer` ：将在其中生成体素数据的缓冲区。它不应该并且 `null` 应该具有非空大小。通话后不要保留参考。注意：此缓冲区可以具有任何非空大小，但可以根据您使用的地形节点进行一些假设。VoxelTerrain 将始终请求大小为 16x16x16 的块，但 VoxelLodTerrain 可以请求不同大小的块。

  
`origin_in_voxels` ：要生成的框下角相对于 LOD0 的坐标。

  
`lod` ：用于此块的详细级别索引。某些发生器可能不支持 LOD，在这种情况下，它可以保留为 0。在 LOD 0 处，传递的缓冲区的每个单元格跨越 1 个空间单元。在LOD 1,2个单位。在 LOD 2、4 个单位，依此类推。

_  
生成于 Oct 02， 2023_
