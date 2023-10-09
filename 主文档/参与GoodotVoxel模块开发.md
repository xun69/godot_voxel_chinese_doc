# 参与Goodot Voxel模块开发

该模块的源代码可以在Github上找到。

##  贡献


要为模块做出贡献，您需要使用 Git 克隆存储库，并在 Github 上创建分支，以便能够发出拉取请求。

###  C++代码


建议阅读官方 Godot 文档中的引擎开发部分。它解释了如何编译引擎、设置 IDE 以及如何创建自定义模块。


有关与体素工具相关的代码指南，请参阅代码指南

###  主要文档


该文档是使用Markdown编写的，使用Mkdocs格式化，并作为ReadTheDocs上的网站提供。


要为主页做出贡献，请对 `doc/docs` 文件夹下的文件进行更改 `.md` ，并在 Github 上发布 PR。

###  API 文档


为了贡献类引用 （API），您可以改为在 下 `doc/classes` 编辑 XML 文件，类似于对常规 Godot 模块或核心类所做的那样。


更改 XML 文件后，可以使用以下命令使用 中的 `build.py` `doc/tools` 脚本将其转换为其 Markdown 对应项：

```
python build.py -a
```


`build.py` 有其他论据可以做其他事情。如果在没有参数的情况下运行它，将打印帮助。

###   图形节点文档

\[VoxelGeneratorGraph\] 的图形节点目前没有用 Godot 类表示。因此，他们在 XML 文件中使用自己的文档，使用类似于类的工作流。XML 文件是编辑器以及在线文档中显示的节点描述和类别的唯一事实来源。


XML文件可以通过使用以下参数运行Godot来从引擎中存在的节点生成或更新：

`--voxel_doc_tool src dst`


其中 `src` 是原始 XML 的路径， `dst` 是写入更新的 XML 的路径。两条路径可以相同。此 XML 文件应已在 下 `doc/graph_nodes.xml` 进行版本控制。


然后，可以使用 XML 文件生成多个文档：

-     
    Markdown 文档，出现在网站上
-     
    C++文档，显示在编辑器中


两者都是通过从内部 `doc/tools/` 运行脚本 `graph_nodes_doc.py` 生成的。

##  图层

###  主要层


该模块有 3 个主要层：

-     
    体素：体素引擎。包装到命名空间中 `zylann::voxel::` 。
-     
    Util：函数、助手和数据结构库，不依赖于体素。包装到命名空间中 `zylann::` 。
-     
    第三方：第三方库。

###  文件夹


该模块分为多个文件夹，每个文件夹都有不同的依赖项。因此，可以使用 ，或 `VoxelStream` 独立使用 `VoxelMesher` ， `VoxelGenerator` 而无需使用 `VoxelTerrain` 节点。

|  目录 |  描述 |
| --- | --- |
| constants/ |整个引擎中使用的常量和查找表。 |
| doc/ |  包含文档 |
| edition/ |用于访问和修改体素的高级实用程序。可能取决于体素节点。 |
| editor/ |特定于编辑器的代码。也可能取决于体素节点。 |
| meshers/ |包含任务管理。依赖于网格器、流、存储，但不直接依赖于节点。 |
| generators/ |程序生成器。它们仅依赖于体素存储和数学。 |
| meshers/ |仅依赖于体素存储、数学和一些 Godot 图形 API。 |
| misc/ |各种脚本和配置文件，存储在这里以避免主文件夹混乱。 |
| modifiers/ |与修饰符功能相关的文件。 |
| shaders/ |引擎内部使用的着色器，包括文本形式和格式化C++形式。 |
| storage/ |存储和内存数据结构。 |
| streams/ |文件处理代码。仅取决于文件系统和存储。 |
| terrain/ |包含所有节点。取决于模块的其余部分，但仅编辑器部分除外。 |
| tests/ |包含测试。如果在构建脚本中启用，则当 Godot 启动时，它们会运行。 |
| thirdparty/ |第三方库，源代码形式。它们是静态编译的，因此Godot仍然是一个可执行文件。 |
| util/ |通用实用程序函数和结构。他们不依赖于体素的东西。 |

###  代码


除了文件夹结构所反映的层之外，Godot 和这个模块之间还有一个隐含的区别：如果一段代码不需要依赖 Godot，那么它往往不依赖于 Godot。


例如，Transvoxel的实现对Godot的依赖性很小。事实上，它不关心资源是什么，不需要变体，不需要绑定，不需要使用 OOP 等。这就是为什么网格资源不包含逻辑，而是充当算法与其在Godot中的使用之间的“桥梁”。


同样适用于 `VoxelBuffer` ：这个类实际上不是一个成熟的戈多对象。它比这轻得多，因为它可以有数千个实例，甚至支持在堆栈上分配和移动。在脚本编写者必须与之交互的少数情况下，它作为包装器对象公开。

##  测试


测试不是强制性的，但如果有时间进行新的测试，那就太好了。


该模块最近包含一个 `tests/` 文件夹，其中包含单元测试。在撰写本文时，它们很少，我仍然不经常写新的。作为一名游戏开发人员，为所有内容编写单元测试并不是我习惯的一部分，但我认识到，对于像这样的模块，如果可以轻松测试功能，最好有一些。它甚至已经帮助修复了一些错误。


目前没有使用测试框架，相反，它们只是通过在失败或不失败时打印错误来运行。在Godot 4中使用了Doctest框架，因此我们可以看看以后是否可以迁移到该框架。

##  线程


该模块使用多个后台线程来处理体素。线程数可以在项目设置中调整。

![Schema of threads](https://voxel-tools.readthedocs.io/en/latest/images/threads_schema.webp)


有一个线程池。可以给这个池分配许多任务，并将它们分发到它的所有线程。因此，可用的线程越多，大量任务的完成速度就越快。任务也按优先级排序，因此例如，在生成 300 米外的体素块之前，将运行更新玩家附近的网格。


某些任务计划在“串行”组中，这意味着一次只能运行其中一个任务（尽管任何线程都可以运行它们）。这是为了避免在等待任务都锁定共享资源时阻塞所有线程。这用于 I/O，例如加载和保存到磁盘。


线程在体素引擎中进行管理。


注意：此任务系统不考虑“框架”。任务可以随时运行少于或多个主线程的帧。

##  代码规范

###  语法


在大多数情况下，使用 `clang-format` 并遵循戈多惯例。

-     
    类和结构名称 `PascalCase`
-     
    常量、枚举和宏 `CAPSLOCK_CASE`
-    其他名称 `snake_case`
-     
    前缀为 `g_`
-     
    前缀为 的 `s_` 静态
-     
    以 `tls_`
-     
    以 为 `p_` 前缀的参数，但到目前为止尚未真正强制执行。大功能很重要。
-     
    前缀为 的 `_` 私有和受保护字段
-     
    一些私有函数以 开头 `_` ，要么是为了模仿 Godot API，要么是不执行检查的重用函数
-     
    信号处理程序函数以 为 `_on_` 前缀，绝不应手动调用
-     
    以名称为前缀的枚举。例： `enum Type { TYPE_ONE, TYPE_TWO }`
-     
    行尾左大括号，下行闭合
-    从不省略大括号
-     
    二进制运算符和控制流之间的空间： `if (a + b == 42)`
-    使用制表符缩进
-     
    私有包装器函数可用于适应脚本 API，并以 `_b_` .
-     
    使用 Clang-format 来自动化大多数这些规则（C++项目的根目录应该包含一个文件）
-     
    首选仅包含评论的评论 `//`
-     
    包装类中的某些虚拟函数带有前缀 `_zn_` ，以便在编译为模块或 GDExtension时封装签名差异。

###  文件结构

-     
    用于 `.h` 标头和 `.cpp` 实现文件。
-     
    文件名使用 `snake_case` .
-     
    构造函数和析构函数位于顶部
-     
    公共 API 在上面，私有的东西在下面
-     
    绑定位于底部。
-     
    避免排长队。首选的最大行长度为 120 个字符。不要在同一条线上安装太多操作，请使用局部变量。
-     
    如果 `.cpp` 类型或函数是内部的，则在编译时间中定义类型或函数可能比在标头中定义类型或函数更好。

###  C++功能

-     
    除非类型无法表达或模板较长（如 STL 模板），否则不要使用 `auto` 。未授予 IDE（Github 审查和差异）
-     
    适度使用 lambda 和函子是可以的。不是 `std::function` .
-     
    应明确定义 Lambda 捕获（尝试减少 或 `[&]` 的使用 `[=]` ）
-     
    如果STL的表现明显优于Godot替代品，那么它就可以了。
-     
    初始化声明旁边的变量
-     
    避免使用宏来定义逻辑或常量。首选 `static const` 和 `constexpr` `inline` 函数。
-     
    更喜欢添加到 `const` 初始化后不会更改的变量（暂时保留函数参数，因为它会使签名很长）
-     
    当存在显式替代项时，不要利用布尔化。示例：使用 `if (a == nullptr)` 代替 `if (!a)`
-     
    如果可能，请避免使用纯数组，例如 `int a[42]` 。调试器不会捕获它们的溢出。更喜欢使用包装器，例如 `FixedArray` 和 `Span` （或 `std::array` 一旦 `std::span` 修复）
-     
    使用 `uint32_t` ， ， `uint16_t` `uint8_t` 以防整数大小很重要。
-     
    如果可能，请在标头中使用前向声明，而不是包含文件
-     
    不要在标头中做 `using namespace` （除了 ，但这只是为了帮助支持使用相同的代码库的 GDExtension `godot::` ，因为 Godot 核心没有这个命名空间）。
-     
    `mutable` 只能用于线程同步原语。不要将它与“缓存数据”一起使用来制作getter `const` ，因为它在多线程上下文中可能会产生误导。
-     
    不使用例外

###  错误处理

-     
    不使用例外。
-     
    检查不变量，尽早失败。使用 `CRASH_COND` 或 `ZN_ASSERT` 在调试模式下确保状态符合预期，即使它们不会立即造成伤害。
-     
    崩溃对用户来说并不好，因此在面向用户的代码（脚本）中使用宏 `ZN_ASSERT_RETURN` 来获取 `ERR_FAIL_COND` 可以从错误中恢复的代码，或防止命中内部断言
-     
    前缀为 Godot 的宏与 Godot 无关，可用于不太依赖 Godot `ZN_` 的区域的可移植性。

###  性能


在运行频繁的性能关键领域：

-     
    避免分配。通过内存池、 `ObjectPool` 固定大小的阵列或使用 `std::vector` 容量重复使用内存。
-     
    避免 `virtual` 、 `Ref<T>`  、`String`
-     
    不要调整大小 `PoolVectors` 或 `Vector<T>` ，或者如果需要，一次性完成
-     
    注意什么是线程安全的，什么是不是。此模块的一些主要区域在线程中工作。
-     
    将互斥锁减少到最低限度，避免长时间锁定。
-     
    使用适合随时间推移最频繁使用的数据结构（通常是数组、向量或哈希映射）。
-     
    如果统计数据的影响可以忽略不计，请考虑统计数据。它可以帮助用户监控模块的性能，即使在发布版本中也是如此。
-     
    在发布模式下分析代码。此模块对 Tracy 友好，请参阅 `util/profiling.hpp` 。
-     
    在制作数据结构时要注意对齐。例如，打包小于 4 个字节的字段，以便更好地利用空间

###  Godot API

-     
    在性能很重要的领域，使用最直接的 API 来完成作业。特别是，不要使用节点。请参阅 `RenderingServer` 和 `PhysicsServer` 。
-     
    仅当函数可以安全使用并保证存在一段时间时，才向脚本 API 公开函数
-     
    如果可能，请使用 `memnew` 、 `memdelete` 等 `memalloc` `memfree` ，以便在 Godot 监视器中计算内存使用量
-     
    不要留下随机打印。对于详细模式，您也可以使用 `ZN_PRINT_VERBOSE()` `print_verbose()` 代替 。
-     
    如果脚本不需要超过 2^31，则用作 `int` 脚本公开的函数的参数，即使它们从不为负数，因此如果用户犯了错误，错误会更清晰
-     
    如果可能的话，将Godot的使用保持在最低限度，以使代码更具可移植性，有时在将来的GDExtension中更快。某些区域使用 中 `util/` 定义的自定义等效项。


编译为模块或扩展都受支持，因此涉及一些限制：

-     
    不要直接包含戈多标头。使用来自 的 `util/godot` 标头。
-     
    仅使用可用于 GDExtension（或脚本 API）的 API。如果它们存在于两者中但不同，请使用 中 `util/godot` 定义的包装器。

###  命名空间


有意的命名空间是 `zylann::` 主要的，并且 `zylann::voxel::` 用于与体素相关的东西。模块的不同部分可能还有其他部分。


注册的类也具有命名空间以防止冲突。这些没有出现在Godot的ClassDB中，因此与体素相关的类也带有前缀 `Voxel` 。其他更泛型的类带有前缀 `ZN_` 。


如果已注册的类需要与内部类相同的名称，则可以将其放入 `::gd` 子命名空间中。另一方面，内部类也可以加后缀 `Internal` 。

###  版本控制

-     
    首选使用逻辑更改分隔提交，并使用代码格式分隔提交
-     
    执行 PR 时，更喜欢压缩 WIP 提交

##  调试

###  命令行参数


当你启动Godot时，默认情况下它会启动项目经理。当您从那里选择一个项目时，它将重新启动自身，但这会断开调试器的连接。所以建议使用命令行参数，在你想要的项目和模式下直接启动Godot。


首先，确保Godot在项目的工作目录中启动。

-     
    要调试游戏，请毫无争议地启动Godot，它将从主场景开始。
-     
    要调试项目的特定场景，请使用场景的相对路径作为命令行参数启动 Godot
-     
    若要调试编辑器，请添加 `-e` 参数。


在 Windows 上的 VSCode `launch.json` 中设置的选项示例：

```json
{
    "version": "0.2.0",
    "configurations": [
        {
            "name": "(Windows) Launch",
            "type": "cppvsdbg", // For MSVC
            //"type": "cppdbg", // For GDB
            "request": "launch",
            "program": "${workspaceFolder}/bin/godot.windows.editor.dev.x86_64.exe", // Dev build (old target=debug)
            //"program": "${workspaceFolder}/bin/godot.windows.editor.x86_64.exe", // Non-dev build (old target=release_debug)
            "args": [
                "-v", // Verbose output

                //"-e", // Editor mode

                //"--debug-collisions",

                // Run a specific scene
                //"local_tests/sqlite/test_sqlite.tscn",
                //"local_tests/texturing/test_textured_terrain.tscn"
                //"local_tests/texturing/test_texturing.tscn"
            ],
            "stopAtEntry": false,
            "cwd": "D:/PROJETS/INFO/GODOT/Games/SolarSystem/Project",
            "environment": [],
            "visualizerFile": "${workspaceFolder}/modules/voxel/misc/voxel.natvis"
        }
    ]
}
```

###  出错时的断点


建议使用调试器在发生错误或崩溃时获得更好的信息。打开 `core/error/error_macros.cpp` （在Godot 4.x中）并在 中 `_err_print_error` 保留一个断点可能很有用，这样每次发生错误时，调试器都会中断其中，为您提供实时调用堆栈和要检查的变量状态。


如果您调试编辑器，Godot 往往会为不重要的事情打印更多错误，例如在脚本编辑器中犯临时错误，或者尝试在资源管理器停靠中索引资源文件并因任何原因失败。在这种情况下，您可能需要干净的专用测试项目，或者在启动后放置断点。

###  调试打印

 Godot：

```c++
#include <core/string/print_string.h>

print_line(String("Hello {0}, my age is {1}").format(varray(name, age)));
```

 非 Godot：

```c++
#include "util/log.h"
#include "util/string_funcs.h"

println(format("Hello {}, my age is {}", name, age));
```

###  漂亮的打印


除了STL的容器类型之外，Godot和体素模块都使用自己的容器类型。调试器通常无法检查它们。例如，Godot 的 `Vector<T>` 类类似于 但 `std::vector<T>` 调试器无法让你检查其中的内容。


若要解决此问题，通常可以向调试器提供一个文件，其中列出了特殊模式，以更用户友好的方式检查这些类型。


在VSCode中，cpp-tools扩展支持natvis文件。戈多在. `platform/windows/godot.natvis` 要获得 Godot 类型的漂亮打印，请在您的 `launch.json` 文件中添加以下行：

```json
"visualizerFile": "${workspaceFolder}/platform/windows/godot.natvis"
```


不幸的是，目前只能提供一个文件。一个问题开放，请求支持多个文件。这意味着，如果您还想对体素模块的结构进行漂亮的打印，则必须将natvis路径替换为以下内容：

```json
"visualizerFile": "${workspaceFolder}/modules/voxel/misc/voxel.natvis"
```

##  Tracy简介


此模块包含用于分析特定代码段的宏。默认情况下，这些宏将扩展到 Tracy 探查器区域。它允许检查代码运行需要多长时间，并将其显示在时间线中。


它用Tracy 0.7.8进行了测试。

![Tracy screenshot](https://voxel-tools.readthedocs.io/en/latest/images/tracy.webp)


Godot 文档中也提到了替代分析器。它们分析所有内容，似乎基于 CPU 采样，而 Tracy 是一个检测分析器，在时间轴上提供特定的实时结果。

###   如何使用探查器作用域

分析范围限定一段代码。它获取之前、之后的时间，并将其记录到时间轴中。C++我们可以使用 RAII 在退出函数或块时自动关闭一个部分，因此通常在分析区域的开头需要一个宏。


宏与探查器无关，因此如果要使用其他探查器，可以更改它们。


您需要包含 `util/profiling.h` 才能访问宏。


要分析整个函数，请执行以下操作：

```c++
void some_function() {
    ZN_PROFILE_SCOPE();
    //...
}
```


要分析函数的一部分：

```c++
void some_function() {
    // 一些代码...

    // 可以是“if”、“for”、“while”，也可以是这里的简单块
    {
        ZN_PROFILE_SCOPE();
        // 分析的代码...
    }

    //...
}
```


默认情况下，作用域采用函数的名称或文件和行号，但您可以使用 显式 `ZN_PROFILE_SCOPE_NAMED("Hello")` 指定名称。仅支持编译时字符串，请勿使用 `String` 或 `std::string` .


也可以绘制数值，以便它们也显示在时间轴中：

```c++
void process_every_frame() {
    // Some code...

    ZN_PROFILE_PLOT("Bunnies", bunnies.size());
}
```

###   将Tracy添加到Godot

要添加 Tracy 支持，请将其克隆到（Godot 的 `thirdparty` 文件夹，而不是体素模块）下 `thirdparty/tracy` 。然后在 中添加 `modules/voxel/SCsub` 以下行：

```
# tracy library
env.Append(CPPDEFINES="TRACY_ENABLE")
env_voxel.Append(CPPDEFINES="TRACY_ENABLE")
voxel_files += ["#thirdparty/tracy/TracyClient.cpp"]
```


这些行可能已经存在，如果是这样，只需取消注释它们。

完成分析后，不要忘记删除这些行，否则分析数据将累积在内存中而不被检索。

---

**注意**

Tracy 有一个帧标记的概念，通常由应用程序提供，用于告诉探查器每个帧何时开始。Godot 本身不提供性能分析宏，因此帧标记被黑客入侵到进程函数中 `VoxelEngine` 。这允许在时间轴中看到主线程的帧，但它们将从其实际开始偏移。

---


这种整合Tracy的方式是基于vblanco的这个提交

##  预处理器宏


该模块具有一些预处理器宏，可以定义这些宏以关闭正在编译的部分代码。有些可以通过 SCons 命令行参数指定。

-     
    `MESHOPTIMIZER_ZYLANN_NEVER_COLLAPSE_BORDERS` ：必须定义此值才能解决 的问题 `MeshOptimizer` 。见 https://github.com/zeux/meshoptimizer/issues/311
-     
    `MESHOPTIMIZER_ZYLANN_WRAP_LIBRARY_IN_NAMESPACE` ：必须定义这个以防止与Godot自己的MeshOptimizer版本发生冲突。见 https://github.com/zeux/meshoptimizer/issues/311#issuecomment-955750624
-     
    `VOXEL_ENABLE_FAST_NOISE_2` ：如果已定义，该模块将使用 FastNoise2 进行编译，并集成了对 SIMD 噪声的支持。它是可选的，以防它在某些编译器或平台上引起问题。SCons 参数： `voxel_fast_noise_2=yes`
-     
    `VOXEL_RUN_TESTS` ：如果 ，则将 `True` 编译测试并在启动时运行，以验证引擎的某些功能是否仍然正常工作。默认情况下，它在生产版本中处于关闭状态。这主要用于在模块上进行C++开发时的调试版本。SCons 参数： `voxel_tests=yes`
-     
    `ZN_GODOT` ：在将此项目编译为模块时必须定义。
-     
    `ZN_GODOT_EXTENSION` ：在将此项目编译为 GDExtension时必须定义。

##  着色器


该模块包含其某些功能的着色器，主要是计算着色器。它们位于 `shaders/dev/` 文件夹下。


`shaders/dev` 包含一个戈多项目。这个项目的目的主要是快速测试着色器是否编译正确，并最终使用简单的场景和GDScript代码对其进行测试。


有几种编写着色器的方法：

-     
    普通：常规着色器，将按原样使用。
-     
    模板：这些包含 `<PLACEHOLDER>` 部分，引擎将用生成的代码替换这些部分。这些部分中的代码将被替换，并且仅用于使着色器在测试项目中编译。
-     
    代码段：这些 `<SNIPPET>` 包含部分，这些部分将插入到模板或其他生成的代码中。这些部分之外的代码将不会使用，并且仅用于使着色器在测试项目中编译。


在编译为模块时传送外部文件很不方便，因此它们直接嵌入C++中，类似于Godot的做法。可以执行脚本来更新这些生成的文件。您必须在 `shaders/` 文件夹中打开命令行并运行 `python text2cpp.py` 。


目前，生成着色器的C++代码与这些着色器的内容交织在一起。例如，代码生成中的C++字符串可以包含在 GLSL 文件中找到的变量名称，因此您应该打开两者以了解上下文。

##  使用另一个模块中的模块

直接在 Godot 中编写自定义C++模块是更直接地访问 Godot 和体素引擎功能的一种方法，这比 GDExtension的性能更好且更稳定。如果要创建自定义生成器、网格器、流或仅使用模块的组件，而无需直接修改模块，也可以执行此操作。


您可以通过在包含 `modules/voxel/` 中使用以下内容来包含体素模块中的文件：

```c++
#include <modules/voxel/storage/voxel_buffer_internal.h>
```


您还需要在 `SCsub` 文件中定义预处理器宏：

```c++
env_yourmodule.Append(CPPDEFINES = [
    'ZN_GODOT'
])
```

##  GDExtension

---

**警告**

此功能正在开发中，尚未准备好投入生产。它有错误，可能会使引擎崩溃。检查问题跟踪器以了解正在进行的工作。

---


此模块可以编译为 GDExtension库。这允许将其作为库文件（ `.dll` ， `.so` ...）分发，而无需重新编译Godot引擎。TODO：Godot的文档似乎还没有包含有关GDExtension的信息。现在，您可以查看此旧新闻和GodotCpp存储库。


要编译库： - 下载 GodotCpp 的副本 - 在体素模块的根目录中，在 `SConstruct` 脚本开头写入 GodotCpp 的路径，或从命令行设置环境变量。- 打开与编译Godot相同的控制台，将目录更改为体素模块的根文件夹，并在那里运行SCons。它将使用 `SConstruct` 该文件而不是 `SCsub` .库将保存在一个 `bin/` 文件夹下。


Windows上的构建命令示例（用于编辑器的未优化调试版本）：

```bash
scons platform=windows target=debug -j4
```


构建的库将放置在 `project/` 包含 Godot 4 项目的文件夹中。然后可以打开它来测试扩展。请注意，它可能尚未针对所有平台进行设置（到目前为止，Windows 64 位已设置）。


在实现此目标之前，有许多问题需要解决。扩展能够运行，但存在已知问题。检查问题跟踪器以了解正在进行的工作。
