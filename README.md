# Godot Voxel中文文档【翻译项目】

![image](https://github.com/xun69/godot_voxel_chinese_doc/assets/23306801/a4ecc367-0618-409c-bab4-0578cd2a1582)

## 概述

Godot Voxel是一个基于Godot编辑器构建的体素游戏开发工具，它以C++模块的形式开发，并以单独的Godot版本编译和构建，所以本质上它并不是一个Godot插件，而是一个独立的Godot版本。

通过它你可以快速的上手开发类**我的世界**的体素游戏，也可以创建平滑的随机地形用于非体素游戏。

官方虽然提供了文档，但是没有提供中文版本，所以译者([Bilibili@巽星石](https://space.bilibili.com/98273681))想着完整翻译一遍。但是由于原文档内容组织还是有些问题，所以我还是决定对部分内容以自己的方式重新组织语言和排版，让其更适合中国Godoter们的体质。

### Godot Voxel原项目

- GitHub仓库：https://github.com/Zylann/godot_voxel

### 视频教程

- [【Godot教程】用 Godot制作《我的世界》风格的游戏！_哔哩哔哩_bilibili](https://www.bilibili.com/video/BV1mN411J7yv/?spm_id_from=333.337.search-card.all.click)
- 使用平滑透体素方法的戈多体素工具模块的体素地形教程（由 Aknakos 提供）（2021 年 6 月 17 日）
- 如何在戈多制作体素地形（Tokisan Games）（2019年11月4日）
- 戈多体素工具（由游戏从零开始）（2020年7月25日）

## 文档目录

- [下载安装](./主文档/下载安装.md) 
- [快速上手](./主文档/快速上手.md) 
- [体素相关概念](./主文档/体素相关概念.md) 
- [地形类型](./主文档/地形类型.md) 
- [块状地形](./主文档/块状地形.md) 
- [平滑地形](./主文档/平滑地形.md) 

###  演示项目

本地下载安装Godot Voxel后，就可以下载以下三个演示项目进行辅助学习，三个项目都是由Godot Voxel的主要作者[Zylann](https://github.com/Zylann)创建的。所以也算是第一手的学习资料了。

| 截图                                                         | 概述                                                         | 链接                                                         |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| <img src="https://github.com/Zylann/voxelgame/raw/master/screenshots/2020_05_05_1953_small.png" alt="Screenshot" style="zoom: 50%;" /> | 基于Godot Voxel程序生成的体素地形和其他模型网格，基本上实现了《我的世界》的很多功能。 | [体素游戏演示（戈多引擎 4.0）](https://github.com/Zylann/voxelgame#voxel-game-demos-godot-engine-40) |
| <img src="./README.assets/xk.jpeg"  style="zoom: 80%;" />    | 基于Godot Voxel程序生成星球。Youtube[演示视频](https://www.youtube.com/watch?v=8OrZX347MoE)，整体感觉有点像《无人深空》低配版。 | 3D太空游戏演示                                               |
| <img src="./README.assets/3d-noise-1696779223718-12.jpg" alt="img" style="zoom:50%;" /> | 包含基于Godot Voxel的多个演示。                              | [Godot体素工具的演示集合](https://github.com/tinmanjuggernaut/voxelgame) |
