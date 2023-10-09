# VoxelBoxMover体素箱移器

> ## Excerpt
> 继承：引用计数

---
##  体素箱移

 继承：引用计数

##  说明：

  
实用程序类允许仅使用体素 AABB 重现简单的移动和滑动逻辑，类似于 Minecraft 物理。此类只能与块状体素一起使用。

  
将它的实例存储在脚本的成员变量中，并在Node.\_process或Node.\_physics\_process中使用它（它可以在你喜欢的任何位置工作）。

```
var motion = Vector3(0, 0, -10 * delta) # Move forward
motion = _box_mover.get_motion(get_translation(), motion, aabb, terrain_node)
global_translate(motion)
```

##  方法：

|  返回 |  签名 |
| --- | --- |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html) |   
get\_collision\_mask （ ） 常量 |
|  [浮](https://docs.godotengine.org/en/stable/classes/class_float.html) |   
get\_max\_step\_height （ ） 常量 |
|  [矢量3](https://docs.godotengine.org/en/stable/classes/class_vector3.html) |   
get\_motion （ 矢量3 位， 矢量3 运动， AABB aabb， 节点地形 ） |
|  [布尔](https://docs.godotengine.org/en/stable/classes/class_bool.html) |   
has\_stepped\_up （ ） 常量 |
|  [布尔](https://docs.godotengine.org/en/stable/classes/class_bool.html) |   
is\_step\_climbing\_enabled （ ） 常量 |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBoxMover/#) |   
set\_collision\_mask （ int 掩码 ） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBoxMover/#) |   
set\_max\_step\_height （浮子高度） |
|  [无效](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBoxMover/#) |   
set\_step\_climbing\_enabled （ 启用布尔值 ） |

##  方法说明

-     
    intget\_collision\_mask（ ）

  
获取用于检测可碰撞体素的碰撞掩码。

  
此碰撞掩码特定于此碰撞系统，并在VoxelBlockyModel.collision\_mask中定义。

-     
    floatget\_max\_step\_height（ ）
    
-     
    Vector3get\_motion（矢量3位，矢量3运动，AABB aabb，节点地形）
    

  
给定一个运动向量，返回一个修改后的向量，告诉您角色移动多少。这类似于KinematicBody.move\_and\_slide，只是您必须应用运动。

-    boolhas\_stepped\_up（ ）

  
启用阶梯攀爬后，告知上次对VoxelBoxMover.get\_motion调用何时导致攀爬发生。

  
攀爬会向上修改运动矢量，使身体卡在台阶顶部。这可能会对字符控制器代码产生影响，例如将字符视为在地板上而不是跳跃。

-     
    boolis\_step\_climbing\_enabled（ ）

  
告知是否启用了攀登台阶。

-     
    voidset\_collision\_mask（ 整数掩码 ）

  
设置用于检测可碰撞体素的碰撞遮罩。

  
只会检测到在遮罩之间共享至少一位的体素。

  
此碰撞掩码特定于此碰撞系统，并在VoxelBlockyModel.collision\_mask中定义。

-     
    voidset\_max\_step\_height（浮子高度）

  
设置可以像“楼梯”一样攀爬的最大高度。

-     
    voidset\_step\_climbing\_enabled（启用布尔值）

  
启用后，VoxelBoxMover.get\_motion将尝试爬上小台阶。这允许实现类似Minecraft的楼梯。

_  
生成于 Oct 02， 2023_
