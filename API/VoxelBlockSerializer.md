
# VoxelBlockSerializer

##  体素块序列化程序

 继承：引用计数

##  说明：

  
用于在体素缓冲区中保存和加载数据的低级实用程序。这对于通过网络发送数据或将其存储在文件中非常有用。

  
要存储到分配 PackedByteArray 的文件中：

```
# `voxels` is an existing `VoxelBuffer`
var data := VoxelBlockSerializer.serialize_to_byte_array(voxels, true)
file.store_32(len(data))
file.store_buffer(data)
```

  
要回读：

```
var size := file.get_32()
var data := file.get_buffer(size)
VoxelBlockSerializer.deserialize_from_byte_array(data, voxels, true)
```

  
要通过重用 StreamPeerBuffer 存储到文件中：

```
# Note, buffer can be re-used if you do this often
var stream_peer_buffer := StreamPeerBuffer.new()
var written_size = VoxelBlockSerializer.serialize_to_stream_peer(stream_peer_buffer, voxels, true)
file.store_32(written_size)
file.store_buffer(stream_peer_buffer.data_array)
```

  
要回读：

```
var size := file.get_32()
var stream_peer_buffer := StreamPeerBuffer.new()
# Unfortunately Godot will always allocate memory with this API, can't avoid that
stream_peer_buffer.data_array = file.get_buffer(size)
VoxelBlockSerializer.deserialize_from_stream_peer(stream_peer_buffer, voxels, size, true)
```

##  方法：

|  返回 |  签名 |
| --- | --- |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockSerializer/#) |   
deserialize\_from\_byte\_array （ PackedByteArray bytes， VoxelBuffer voxel\_buffer， bool decompress ） static |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockSerializer/#) |   
deserialize\_from\_stream\_peer （ StreamPeer ， VoxelBuffer voxel\_buffer， int size， bool decompress ） static |
| [PackedByteArray](https://docs.godotengine.org/en/stable/classes/class_packedbytearray.html) |   
serialize\_to\_byte\_array （体素缓冲区 voxel\_buffer， 布尔压缩） 静态 |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) |   
serialize\_to\_stream\_peer （ StreamPeer pear， VoxelBuffer voxel\_buffer， bool compress ） static |

##  方法说明

-     
    voiddeserialize\_from\_byte\_array（ PackedByteArray bytes， VoxelBuffer voxel\_buffer， bool decompress ）

  
从 PackedByteArray 读取体素缓冲区的数据。

-     
    voiddeserialize\_from\_stream\_peer（ StreamPeer peer， VoxelBuffer voxel\_buffer， int size， bool decompress ）

  
从 StreamPeer 读取 VoxelBuffer 的数据。您必须提供要读取的字节数。

-     
    PackedByteArrayserialize\_to\_byte\_array（体素缓冲voxel\_buffer，布尔压缩）

  
将体素缓冲区的数据存储到 PackedByteArray 中。

-     
    intserialize\_to\_stream\_peer（ StreamPeer pear， VoxelBuffer voxel\_buffer， bool compress ）

  
将 VoxelBuffer 的数据存储到 StreamPeer 中。返回写入的字节数。

_  
生成于 Oct 02， 2023_
