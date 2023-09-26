---
created: 2023-09-27T00:01:21 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelBoxMover/
author: 
---

# VoxelBoxMover体素箱移器

> ## Excerpt
> Inherits: RefCounted 继承：引用计数

---
Inherits: [RefCounted](https://docs.godotengine.org/en/stable/classes/class_refcounted.html) 继承：引用计数

## Description: 说明：

Utility class allowing to reproduce simple move-and-slide logic using only voxel AABBs, similar to Minecraft physics. This class may only be used with blocky voxels.  
实用程序类允许仅使用体素 AABB 重现简单的移动和滑动逻辑，类似于 Minecraft 物理。此类只能与块状体素一起使用。

Store an instance of it within a member variable of your script, and use it within [Node.\_process](https://docs.godotengine.org/en/stable/classes/class_node.html#class-node-method-process) or [Node.\_physics\_process](https://docs.godotengine.org/en/stable/classes/class_node.html#class-node-method-physics-process) (it works wherever you like).  
将它的实例存储在脚本的成员变量中，并在Node.\_process或Node.\_physics\_process中使用它（它可以在你喜欢的任何位置工作）。

```
var motion = Vector3(0, 0, -10 * delta) # Move forward
motion = _box_mover.get_motion(get_translation(), motion, aabb, terrain_node)
global_translate(motion)

```

## Methods: 方法：

## Method Descriptions 方法说明

-   [int](https://docs.godotengine.org/en/stable/classes/class_int.html) **get\_collision\_mask**( )  
    intget\_collision\_mask（ ）

Gets the collision mask used to detect collidable voxels.  
获取用于检测可碰撞体素的碰撞掩码。

This collision mask is specific to this collision system, and is defined in [VoxelBlockyModel.collision\_mask](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModel/#i_collision_mask).  
此碰撞掩码特定于此碰撞系统，并在VoxelBlockyModel.collision\_mask中定义。

-   [float](https://docs.godotengine.org/en/stable/classes/class_float.html) **get\_max\_step\_height**( )  
    floatget\_max\_step\_height（ ）
    
-   [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) **get\_motion**( [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) pos, [Vector3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) motion, [AABB](https://docs.godotengine.org/en/stable/classes/class_aabb.html) aabb, [Node](https://docs.godotengine.org/en/stable/classes/class_node.html) terrain )  
    Vector3get\_motion（矢量3位，矢量3运动，AABB aabb，节点地形）
    

Given a motion vector, returns a modified vector telling you by how much to move your character. This is similar to [KinematicBody.move\_and\_slide](https://docs.godotengine.org/en/stable/classes/class_kinematicbody.html#class-kinematicbody-method-move-and-slide), except you have to apply the movement.  
给定一个运动向量，返回一个修改后的向量，告诉您角色移动多少。这类似于KinematicBody.move\_and\_slide，只是您必须应用运动。

-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **has\_stepped\_up**( )  boolhas\_stepped\_up（ ）

When step climbing is enabled, tells when the last call to [VoxelBoxMover.get\_motion](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBoxMover/#i_get_motion) caused climbing to occur.  
启用阶梯攀爬后，告知上次对VoxelBoxMover.get\_motion调用何时导致攀爬发生。

Climbing modifies the motion vector upwards so that the body is snapped on top of the step. This can have implications in character controller code, such as considering the character to be on the floor instead of having jumped.  
攀爬会向上修改运动矢量，使身体卡在台阶顶部。这可能会对字符控制器代码产生影响，例如将字符视为在地板上而不是跳跃。

-   [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) **is\_step\_climbing\_enabled**( )  
    boolis\_step\_climbing\_enabled（ ）

Tells if step climbing is enabled.  
告知是否启用了攀登台阶。

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBoxMover/#) **set\_collision\_mask**( [int](https://docs.godotengine.org/en/stable/classes/class_int.html) mask )  
    voidset\_collision\_mask（ 整数掩码 ）

Sets the collision mask used to detect collidable voxels.  
设置用于检测可碰撞体素的碰撞遮罩。

Only voxels sharing at least one bit between the masks will be detected.  
只会检测到在遮罩之间共享至少一位的体素。

This collision mask is specific to this collision system, and is defined in [VoxelBlockyModel.collision\_mask](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModel/#i_collision_mask).  
此碰撞掩码特定于此碰撞系统，并在VoxelBlockyModel.collision\_mask中定义。

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBoxMover/#) **set\_max\_step\_height**( [float](https://docs.godotengine.org/en/stable/classes/class_float.html) height )  
    voidset\_max\_step\_height（浮子高度）

Sets the maximum height that can be climbed like "stairs".  
设置可以像“楼梯”一样攀爬的最大高度。

-   [void](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBoxMover/#) **set\_step\_climbing\_enabled**( [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html) enabled )  
    voidset\_step\_climbing\_enabled（启用布尔值）

When enabled, [VoxelBoxMover.get\_motion](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBoxMover/#i_get_motion) will attempt to climb up small steps. This allows to implement Minecraft-like stairs.  
启用后，VoxelBoxMover.get\_motion将尝试爬上小台阶。这允许实现类似Minecraft的楼梯。

_Generated on Sep 12, 2023  
生成于 Sep 12， 2023_
