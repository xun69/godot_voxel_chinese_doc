---
created: 2023-09-27T00:01:21 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockSerializer/
author: 
---

# VoxelBlockSerializer体素块序列化程序

> ## Excerpt
> Inherits: RefCounted 继承：引用计数

---
Inherits: [RefCounted](https://docs.godotengine.org/en/stable/classes/class_refcounted.html) 继承：引用计数

## Description: 说明：

Low-level utility to save and load the data within a [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/). This can be useful to send data over the network, or to store it in a file.  
用于在体素缓冲区中保存和加载数据的低级实用程序。这对于通过网络发送数据或将其存储在文件中非常有用。

To store into a file allocating a PackedByteArray:  
要存储到分配 PackedByteArray 的文件中：

```
# `voxels` is an existing `VoxelBuffer`
var data := VoxelBlockSerializer.serialize_to_byte_array(voxels, true)
file.store_32(len(data))
file.store_buffer(data)

```

To read it back:  
要回读：

```
var size := file.get_32()
var data := file.get_buffer(size)
VoxelBlockSerializer.deserialize_from_byte_array(data, voxels, true)

```

To store into a file by re-using a StreamPeerBuffer:  
要通过重用 StreamPeerBuffer 存储到文件中：

```
# Note, buffer can be re-used if you do this often
var stream_peer_buffer := StreamPeerBuffer.new()
var written_size = VoxelBlockSerializer.serialize_to_stream_peer(stream_peer_buffer, voxels, true)
file.store_32(written_size)
file.store_buffer(stream_peer_buffer.data_array)

```

To read it back:  
要回读：

```
var size := file.get_32()
var stream_peer_buffer := StreamPeerBuffer.new()
# Unfortunately Godot will always allocate memory with this API, can't avoid that
stream_peer_buffer.data_array = file.get_buffer(size)
VoxelBlockSerializer.deserialize_from_stream_peer(stream_peer_buffer, voxels, size, true)

```

## Methods: 方法：

## Method Descriptions 方法说明

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockSerializer/#) **deserialize\_from\_byte\_array**( [PackedByteArray](https://docs.godotengine.org/en/stable/classes/class_packedbytearray.html) bytes, [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) voxel\_buffer, [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) decompress )  
    voiddeserialize\_from\_byte\_array（ PackedByteArray bytes， VoxelBuffer voxel\_buffer， bool decompress ）

Reads the data of a [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) from a [PackedByteArray](https://docs.godotengine.org/en/stable/classes/class_packedbytearray.html).  
从 PackedByteArray 读取体素缓冲区的数据。

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockSerializer/#) **deserialize\_from\_stream\_peer**( [StreamPeer](https://docs.godotengine.org/en/stable/classes/class_streampeer.html) peer, [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) voxel\_buffer, [int](https://docs.godotengine.org/en/stable/classes/class_int.html) size, [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) decompress )  
    voiddeserialize\_from\_stream\_peer（ StreamPeer peer， VoxelBuffer voxel\_buffer， int size， bool decompress ）

Reads the data of a [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) from a [StreamPeer](https://docs.godotengine.org/en/stable/classes/class_streampeer.html). You must provide the number of bytes to read.  
从 StreamPeer 读取 VoxelBuffer 的数据。您必须提供要读取的字节数。

-   [PackedByteArray](https://docs.godotengine.org/en/stable/classes/class_packedbytearray.html) **serialize\_to\_byte\_array**( [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) voxel\_buffer, [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) compress )  
    PackedByteArrayserialize\_to\_byte\_array（体素缓冲voxel\_buffer，布尔压缩）

Stores the data of a [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) into a [PackedByteArray](https://docs.godotengine.org/en/stable/classes/class_packedbytearray.html).  
将体素缓冲区的数据存储到 PackedByteArray 中。

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **serialize\_to\_stream\_peer**( [StreamPeer](https://docs.godotengine.org/en/stable/classes/class_streampeer.html) peer, [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) voxel\_buffer, [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) compress )  
    intserialize\_to\_stream\_peer（ StreamPeer pear， VoxelBuffer voxel\_buffer， bool compress ）

Stores the data of a [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/) into a [StreamPeer](https://docs.godotengine.org/en/stable/classes/class_streampeer.html). Returns the number of written bytes.  
将 VoxelBuffer 的数据存储到 StreamPeer 中。返回写入的字节数。

_Generated on Sep 12, 2023  
生成于 Sep 12， 2023_
