# VoxelGeneratorGraph节点

---
This page lists all nodes that can be used in [VoxelGeneratorGraph](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorGraph/) and [VoxelGraphFunction](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/).

## Input[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#input "Permanent link")

### CustomInput[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#custominput "Permanent link")

Outputs: `value`

Outputs values from the custom input having the same name as the node. May be used in [VoxelGraphFunction](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/). It won't be used in [VoxelGeneratorGraph](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorGraph/).

### InputSDF[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#inputsdf "Permanent link")

Outputs: `sdf`

Outputs the existing signed distance at the current voxel. This may only be used in specific situations, such as using the graph as a procedural brush.

### InputX[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#inputx "Permanent link")

Outputs: `x`

Outputs the X coordinate of the current voxel.

### InputY[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#inputy "Permanent link")

Outputs: `y`

Outputs the Y coordinate of the current voxel.

### InputZ[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#inputz "Permanent link")

Outputs: `z`

Outputs the Z coordinate of the current voxel.

## Mapping[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#mapping "Permanent link")

### Curve[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#curve "Permanent link")

Inputs: `x` Outputs: `out` Parameters: `curve`

Returns the value of a custom `curve` at coordinate `x`, where `x` is in the range `[0..1]`. The `curve` is specified with a [Curve](https://docs.godotengine.org/en/stable/classes/class_curve.html) resource.

### Image[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#image "Permanent link")

Inputs: `x`, `y` Outputs: `out` Parameters: `image`

Returns the value of the red channel of an image at coordinates `(x, y)`, where `x` and `y` are in pixels and the return value is in the range `[0..1]` (or more if the image has an HDR format). If coordinates are outside the image, they will be wrapped around. No filtering is performed. The image must have an uncompressed format.

## Math[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#math "Permanent link")

### Abs[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#abs "Permanent link")

Inputs: `x` Outputs: `out`

If `x` is negative, returns `x` as a positive number. Otherwise, returns `x`.

### Clamp[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#clamp "Permanent link")

Inputs: `x`, `min`, `max` Outputs: `out`

If `x` is lower than `min`, returns `min`. If `x` is higher than `max`, returns `max`. Otherwise, returns `x`.

### ClampC[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#clampc "Permanent link")

Inputs: `x` Outputs: `out` Parameters: `min`, `max`

If `x` is lower than `min`, returns `min`. If `x` is higher than `max`, returns `max`. Otherwise, returns `x`. This node is an alternative to `Clamp`, used internally as an optimization if `min` and `max` are constant.

### Expression[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#expression "Permanent link")

Outputs: `out` Parameters: `expression`

Evaluates a math expression. Variable names can be written as inputs of the node. Some functions can be used, but they must be supported graph nodes in the first place, as the expression will be converted to nodes internally. Available functions:

```
sin(x)
floor(x)
abs(x)
sqrt(x)
fract(x)
stepify(x, step)
wrap(x, length)
min(a, b)
max(a, b)
clamp(x, min, max)
lerp(a, b, ratio)
```

### Floor[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#floor "Permanent link")

Inputs: `x` Outputs: `out`

Returns the result of `floor(x)`, the nearest integer that is equal or lower to `x`.

### Fract[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#fract "Permanent link")

Inputs: `x` Outputs: `out`

Returns the decimal part of `x`. The result is always positive regardless of sign.

### Max[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#max "Permanent link")

Inputs: `a`, `b` Outputs: `out`

Returns the highest value between `a` and `b`.

### Min[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#min "Permanent link")

Inputs: `a`, `b` Outputs: `out`

Returns the lowest value between `a` and `b`.

### Mix[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#mix "Permanent link")

Inputs: `a`, `b`, `ratio` Outputs: `out`

Interpolates between `a` and `b`, using parameter value `t`. If `t` is `0`, `a` will be returned. If `t` is `1`, `b` will be returned. If `t` is beyond the `[0..1]` range, the returned value will be an extrapolation.

### Pow[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#pow "Permanent link")

Inputs: `x`, `p` Outputs: `out`

Returns the result of the power function (`x ^ power`). It can be relatively slow.

### Powi[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#powi "Permanent link")

Inputs: `x` Outputs: `out` Parameters: `power`

Returns the result of the power function (`x ^ power`), where the exponent is a constant positive integer. May be faster than `Pow`.

### Remap[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#remap "Permanent link")

Inputs: `x` Outputs: `out` Parameters: `min0`, `max0`, `min1`, `max1`

For an input value `x` in the range `[min0, max0]`, converts linearly into the `[min1, max1]` range. For example, if `x` is `min0`, then `min1` will be returned. If `x` is `max0`, then `max1` will be returned. If `x` is beyond the `[min0, max0]` range, the result will be an extrapolation.

### Select[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#select "Permanent link")

Inputs: `a`, `b`, `t` Outputs: `out` Parameters: `threshold`

If `t` is lower than `threshold`, returns `a`. Otherwise, returns `b`.

### Sin[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#sin "Permanent link")

Inputs: `x` Outputs: `out`

Returns the result of `sin(x)`

### Smoothstep[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#smoothstep "Permanent link")

Inputs: `x` Outputs: `out` Parameters: `edge0`, `edge1`

Returns the result of smoothly interpolating the value of `x` between `0` and `1`, based on the where `x` lies with respect to the edges `egde0` and `edge1`. The return value is `0` if `x <= edge0`, and `1` if `x >= edge1`. If `x` lies between `edge0` and `edge1`, the returned value follows an S-shaped curve that maps `x` between `0` and `1`. This S-shaped curve is the cubic Hermite interpolator, given by `f(y) = 3*y^2 - 2*y^3` where `y = (x-edge0) / (edge1-edge0)`.

### Sqrt[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#sqrt "Permanent link")

Inputs: `x` Outputs: `out`

Returns the square root of `x`. Note: unlike classic square root, if `x` is negative, this function returns `0` instead of `NaN`.

### Stepify[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#stepify "Permanent link")

Inputs: `x`, `step` Outputs: `out`

Snaps `x` to a given step, similar to GDScript's function `stepify`.

### Wrap[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#wrap "Permanent link")

Inputs: `x`, `length` Outputs: `out`

Wraps `x` between `0` and `length`, similar to GDScript's function `wrapf(x, 0, max)`. Note: if `length` is 0, this node will return `NaN`. If it happens, it should not crash, but results will be messed up.

## Misc[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#misc "Permanent link")

Parameters: `text`

A rectangular area with a description, to help organizing a graph.

### Constant[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#constant "Permanent link")

Outputs: `value` Parameters: `value`

Outputs a constant number.

### Function[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#function "Permanent link")

Parameters: `_function`

Runs a custom function, like a re-usable sub-graph. The first parameter (parameter 0) of this node is a reference to a [VoxelGraphFunction](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/). Further parameters (starting from 1) are those exposed by the function.

### Relay[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#relay "Permanent link")

Inputs: `in` Outputs: `out`

Pass-through node, allowing to better organize the path of long connections.

## Noise[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#noise "Permanent link")

### FastNoise2D[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#fastnoise2d "Permanent link")

Inputs: `x`, `y` Outputs: `out` Parameters: `noise`

Returns computation of 2D noise at coordinates `(x, y)` using the FastNoiseLite library. The `noise` parameter is specified with an instance of the [ZN\_FastNoiseLite](https://voxel-tools.readthedocs.io/en/latest/api/ZN_FastNoiseLite/) resource. Note: this node might be a little faster than `Noise2D`.

### FastNoise2\_2D[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#fastnoise2_2d "Permanent link")

Inputs: `x`, `y` Outputs: `out` Parameters: `noise`

Returns computation of 2D SIMD noise at coordinates `(x, y)` using the FastNoise2 library. The `noise` parameter is specified with an instance of the [FastNoise2](https://voxel-tools.readthedocs.io/en/latest/api/FastNoise2/) resource. This is the fastest noise currently supported.

### FastNoise2\_3D[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#fastnoise2_3d "Permanent link")

Inputs: `x`, `y`, `z` Outputs: `out` Parameters: `noise`

Returns computation of 3D SIMD noise at coordinates `(x, y, z)` using the FastNoise2 library. The `noise` parameter is specified with an instance of the [FastNoise2](https://voxel-tools.readthedocs.io/en/latest/api/FastNoise2/) resource. This is the fastest noise currently supported.

### FastNoise3D[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#fastnoise3d "Permanent link")

Inputs: `x`, `y`, `z` Outputs: `out` Parameters: `noise`

Returns computation of 3D noise at coordinates `(x, y, z)` using the FastNoiseLite library. The `noise` parameter is specified with an instance of the [ZN\_FastNoiseLite](https://voxel-tools.readthedocs.io/en/latest/api/ZN_FastNoiseLite/) resource. Note: this node might be a little faster than `Noise3D`.

### FastNoiseGradient2D[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#fastnoisegradient2d "Permanent link")

Inputs: `x`, `y` Outputs: `out_x`, `out_y` Parameters: `noise`

Warps 2D coordinates `(x, y)` using a noise gradient from the FastNoiseLite library. The `noise` parameter is specified with an instance of the [FastNoiseLiteGradient](https://docs.godotengine.org/en/stable/classes/class_fastnoiselitegradient.html) resource.

### FastNoiseGradient3D[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#fastnoisegradient3d "Permanent link")

Inputs: `x`, `y`, `z` Outputs: `out_x`, `out_y`, `out_z` Parameters: `noise`

Warps 3D coordinates `(x, y, z)` using a noise gradient from the FastNoiseLite library. The `noise` parameter is specified with an instance of the [FastNoiseLiteGradient](https://docs.godotengine.org/en/stable/classes/class_fastnoiselitegradient.html) resource.

### Noise2D[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#noise2d "Permanent link")

Inputs: `x`, `y` Outputs: `out` Parameters: `noise`

Returns 2D noise at coordinates `(x, y)` using one of the [Noise](https://docs.godotengine.org/en/stable/classes/class_noise.html) subclasses provided by Godot.

### Noise3D[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#noise3d "Permanent link")

Inputs: `x`, `y`, `z` Outputs: `out` Parameters: `noise`

Returns 3D noise at coordinates `(x, y, z)` using one of the [Noise](https://docs.godotengine.org/en/stable/classes/class_noise.html) subclasses provided by Godot.

### Spots2D[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#spots2d "Permanent link")

Inputs: `x`, `y`, `spot_radius` Outputs: `out` Parameters: `seed`, `cell_size`, `jitter`

Cellular noise optimized for "ore patch" generation: divides space into a 2D grid where each cell contains a circular "spot". Returns 1 when the position is inside the spot, 0 otherwise. `jitter` more or less randomizes the position of the spot inside each cell. Limitation: high jitter can make spots clip with cell borders. This is intentional. If you need more generic cellular noise, use another node.

### Spots3D[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#spots3d "Permanent link")

Inputs: `x`, `y`, `z`, `spot_radius` Outputs: `out` Parameters: `seed`, `cell_size`, `jitter`

Cellular noise optimized for "ore patch" generation: divides space into a 3D grid where each cell contains a circular "spot". Returns 1 when the position is inside the spot, 0 otherwise. `jitter` more or less randomizes the position of the spot inside each cell. Limitation: high jitter can make spots clip with cell borders. This is intentional. If you need more generic cellular noise, use another node.

## Ops[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#ops "Permanent link")

### Add[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#add "Permanent link")

Inputs: `a`, `b` Outputs: `out`

Returns the sum of `a` and `b`

### Divide[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#divide "Permanent link")

Inputs: `a`, `b` Outputs: `out`

Returns the result of `a / b`. Note: dividing by zero outputs NaN. It should not cause crashes, but will likely mess up results. Consider using Multiply when possible.

### Multiply[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#multiply "Permanent link")

Inputs: `a`, `b` Outputs: `out`

Returns the result of `a * b`.

### Subtract[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#subtract "Permanent link")

Inputs: `a`, `b` Outputs: `out`

Returns the result of `a - b`

## Output[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#output "Permanent link")

### CustomOutput[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#customoutput "Permanent link")

Inputs: `value`

Sets the value of the custom output having the same name as the node. May be used in [VoxelGraphFunction](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/). It won't be used in [VoxelGeneratorGraph](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorGraph/).

### OutputSDF[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#outputsdf "Permanent link")

Inputs: `sdf`

Sets the Signed Distance Field value of the current voxel.

### OutputSingleTexture[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#outputsingletexture "Permanent link")

Inputs: `index`

Sets the texture index of the current voxel. This is an alternative to using `OutputWeight` nodes, if your voxels only have one texture. This is easier to use but does not allow for long gradients. Using this node in combination with `OutputWeight` is not supported.

### OutputType[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#outputtype "Permanent link")

Inputs: `type`

Sets the TYPE index of the current voxel. This is for use with [VoxelMesherBlocky](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherBlocky/). If you use this output, you don't need to use `OutputSDF`.

### OutputWeight[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#outputweight "Permanent link")

Inputs: `weight` Parameters: `layer`

Sets the value of a specific texture weight for the current voxel. The texture is specified as an index with the `layer` parameter. There can only be one output using a given layer index.

## SDF[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#sdf "Permanent link")

### SdfBox[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#sdfbox "Permanent link")

Inputs: `x`, `y`, `z` Outputs: `sdf` Parameters: `size_x`, `size_y`, `size_z`

Returns the signed distance field of an axis-aligned box centered at the origin, of size `(size_x, size_y, size_z)`, at coordinates `(x, y, z)`.

### SdfPlane[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#sdfplane "Permanent link")

Inputs: `y`, `height` Outputs: `sdf`

Returns the signed distance field of a plane facing the Y axis located at a given `height`, at coordinate `y`.

### SdfPreview[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#sdfpreview "Permanent link")

Inputs: `value` Parameters: `min_value`, `max_value`, `fraction_period`, `mode`

Debug node, not used in the final result. In the editor, shows a slice of the values emitted from the output it is connected to, according to boundary `[min_value, max_value]`. The slice will be either along the XY plane or the XZ plane, depending on current settings.

### SdfSmoothSubtract[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#sdfsmoothsubtract "Permanent link")

Inputs: `a`, `b` Outputs: `sdf` Parameters: `smoothness`

Subtracts signed distance field `b` from `a`, using the same smoothing as with the `SdfSmoothUnion` node.

### SdfSmoothUnion[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#sdfsmoothunion "Permanent link")

Inputs: `a`, `b` Outputs: `sdf` Parameters: `smoothness`

Returns the smooth union of two signed distance field values `a` and `b`. Smoothness is controlled with the `smoothness` parameter. Higher smoothness will create a larger "weld" between the shapes formed by the two inputs.

### SdfSphere[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#sdfsphere "Permanent link")

Inputs: `x`, `y`, `z` Outputs: `sdf` Parameters: `radius`

Returns the signed distance field of a sphere centered at the origin, of given `radius`, at coordinates `(x, y, z)`.

### SdfSphereHeightmap[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#sdfsphereheightmap "Permanent link")

Inputs: `x`, `y`, `z` Outputs: `sdf` Parameters: `image`, `radius`, `factor`

Returns an approximation of the signed distance field of a spherical heightmap, at coordinates `(x, y, z)`. The heightmap is an `image` using panoramic projection, similar to those used for environment sky in Godot. The radius of the sphere is specified with `radius`. The heights from the heightmap can be scaled using the `factor` parameter. The image must use an uncompressed format.

### SdfTorus[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#sdftorus "Permanent link")

Inputs: `x`, `y`, `z` Outputs: `sdf` Parameters: `radius1`, `radius2`

Returns the signed distance field of a torus centered at the origin, facing the Y axis, at coordinates `(x, y, z)`. The radius of the ring is `radius1`, and its thickness is `radius2`.

## Vector[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#vector "Permanent link")

### Distance2D[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#distance2d "Permanent link")

Inputs: `x0`, `y0`, `x1`, `y1` Outputs: `out`

Returns the distance between two 2D points `(x0, y0)` and `(x1, y1)`.

### Distance3D[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#distance3d "Permanent link")

Inputs: `x0`, `y0`, `z0`, `x1`, `y1`, `z1` Outputs: `out`

Returns the distance between two 3D points `(x0, y0, z0)` and `(x1, y1, z1)`.

### Normalize[¶](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/#normalize "Permanent link")

Inputs: `x`, `y`, `z` Outputs: `nx`, `ny`, `nz`, `len`

Returns the normalized coordinates of the given `(x, y, z)` 3D vector, such that the length of the output vector is 1.
