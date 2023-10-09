# SQLite格式
  
本页介绍 使用的 `VoxelStreamSQLite` 数据库模式。

##  模式

### `meta`

```
meta {
    - version: INTEGER
    - block_size_po2: INTEGER
}
```

  
包含有关卷的一般信息。里面只有一行。

-     
    `version` 是架构的版本。目前 `0` .
-     
    `block_size_po2` 是块的大小作为 2 的幂。它们应该始终相同。默认情况下， `4` 它是（对于 16x16x16 的块）。

### `blocks`

```
blocks {
    - loc: INT64 PRIMARY KEY
    - vb: BLOB
    - instances: BLOB
}
```

  
包含卷的每个块。可能有数千个。

-     
    `loc` 是一个 64 位整数，使用小端序打包块的坐标和 LOD 索引。坐标等于块的原点（以体素为单位），除以块的大小 + 使用欧几里得除法 （ `coord >> (block_size_po2 + lod_index)` ） 的 lod 索引。XYZ 是 16 位有符号整数，LOD 是 8 位无符号整数： `0LXXYYZZ`
-     
    `vb` 包含使用块格式的压缩体素数据。
-     
    `instances` 包含使用实例格式的压缩实例数据。

### `channels`

```
channels {
    - idx: INTEGER PRIMARY KEY
    - depth: INTEGER
}
```

  
包含有关卷中应采用哪些通道格式的一般信息。每个使用的通道有一行。

 警告

  
目前实际上没有使用此表，因为引擎仍然需要工作来管理一般格式。目前，数据库接受任何格式的块，因为它们自版本 3 以来是独立的，但理想情况下它们必须是一致的。
