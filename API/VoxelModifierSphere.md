---
created: 2023-10-09T22:38:26 (UTC +08:00)
tags: []
source: https://voxel-tools.readthedocs.io/en/latest/api/VoxelModifierSphere/
author: 
---

# VoxelModifierSphere体素修饰器球体

> ## Excerpt
> Scripting API

---
-   [Voxel Tools documentation](https://voxel-tools.readthedocs.io/en/latest/)

-   [Getting Voxel Tools](https://voxel-tools.readthedocs.io/en/latest/getting_the_module/)

-   [Quick start](https://voxel-tools.readthedocs.io/en/latest/quick_start/)

-   [Overview](https://voxel-tools.readthedocs.io/en/latest/overview/)

-   [Terrain types](https://voxel-tools.readthedocs.io/en/latest/terrain_types/)

-   [Blocky terrains](https://voxel-tools.readthedocs.io/en/latest/blocky_terrain/)

-   [Smooth terrains](https://voxel-tools.readthedocs.io/en/latest/smooth_terrain/)

-   [Generators](https://voxel-tools.readthedocs.io/en/latest/generators/)

-   [VoxelGeneratorGraph nodes](https://voxel-tools.readthedocs.io/en/latest/graph_nodes/)

-   [Streams](https://voxel-tools.readthedocs.io/en/latest/streams/)

-   [Instancing](https://voxel-tools.readthedocs.io/en/latest/instancing/)

-   [Editor](https://voxel-tools.readthedocs.io/en/latest/editor/)

-   [Multiplayer](https://voxel-tools.readthedocs.io/en/latest/multiplayer/)

-   [Scripting](https://voxel-tools.readthedocs.io/en/latest/scripting/)

-   [Procedural generation](https://voxel-tools.readthedocs.io/en/latest/procedural_generation/)

-   [Performance](https://voxel-tools.readthedocs.io/en/latest/performance/)

-   [Module development](https://voxel-tools.readthedocs.io/en/latest/module_development/)

-   [Changelog](https://voxel-tools.readthedocs.io/en/latest/changelog/)

-   [](https://voxel-tools.readthedocs.io/en/latest/___/)

Scripting API

-   [FastNoise2](https://voxel-tools.readthedocs.io/en/latest/api/FastNoise2/)
-   [VoxelBlockSerializer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockSerializer/)
-   [VoxelBlockyAttribute](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyAttribute/)
-   [VoxelBlockyAttributeAxis](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyAttributeAxis/)
-   [VoxelBlockyAttributeCustom](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyAttributeCustom/)
-   [VoxelBlockyAttributeDirection](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyAttributeDirection/)
-   [VoxelBlockyAttributeRotation](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyAttributeRotation/)
-   [VoxelBlockyLibrary](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyLibrary/)
-   [VoxelBlockyLibraryBase](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyLibraryBase/)
-   [VoxelBlockyModel](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModel/)
-   [VoxelBlockyModelCube](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModelCube/)
-   [VoxelBlockyModelEmpty](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModelEmpty/)
-   [VoxelBlockyModelMesh](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyModelMesh/)
-   [VoxelBlockyType](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyType/)
-   [VoxelBlockyTypeLibrary](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBlockyTypeLibrary/)
-   [VoxelBoxMover](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBoxMover/)
-   [VoxelBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelBuffer/)
-   [VoxelColorPalette](https://voxel-tools.readthedocs.io/en/latest/api/VoxelColorPalette/)
-   [VoxelDataBlockEnterInfo](https://voxel-tools.readthedocs.io/en/latest/api/VoxelDataBlockEnterInfo/)
-   [VoxelEngine](https://voxel-tools.readthedocs.io/en/latest/api/VoxelEngine/)
-   [VoxelGenerator](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGenerator/)
-   [VoxelGeneratorFlat](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorFlat/)
-   [VoxelGeneratorGraph](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorGraph/)
-   [VoxelGeneratorHeightmap](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorHeightmap/)
-   [VoxelGeneratorImage](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorImage/)
-   [VoxelGeneratorNoise](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorNoise/)
-   [VoxelGeneratorNoise2D](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorNoise2D/)
-   [VoxelGeneratorScript](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorScript/)
-   [VoxelGeneratorWaves](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGeneratorWaves/)
-   [VoxelGraphFunction](https://voxel-tools.readthedocs.io/en/latest/api/VoxelGraphFunction/)
-   [VoxelInstanceComponent](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceComponent/)
-   [VoxelInstanceGenerator](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceGenerator/)
-   [VoxelInstanceLibrary](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceLibrary/)
-   [VoxelInstanceLibraryItem](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceLibraryItem/)
-   [VoxelInstanceLibraryMultiMeshItem](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceLibraryMultiMeshItem/)
-   [VoxelInstanceLibrarySceneItem](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstanceLibrarySceneItem/)
-   [VoxelInstancer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelInstancer/)
-   [VoxelLodTerrain](https://voxel-tools.readthedocs.io/en/latest/api/VoxelLodTerrain/)
-   [VoxelMeshSDF](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMeshSDF/)
-   [VoxelMesher](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesher/)
-   [VoxelMesherBlocky](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherBlocky/)
-   [VoxelMesherCubes](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherCubes/)
-   [VoxelMesherDMC](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherDMC/)
-   [VoxelMesherTransvoxel](https://voxel-tools.readthedocs.io/en/latest/api/VoxelMesherTransvoxel/)
-   [VoxelModifier](https://voxel-tools.readthedocs.io/en/latest/api/VoxelModifier/)
-   [VoxelModifierMesh](https://voxel-tools.readthedocs.io/en/latest/api/VoxelModifierMesh/)
-   [VoxelModifierSphere](https://voxel-tools.readthedocs.io/en/latest/api/VoxelModifierSphere/)
    -   [Properties:](https://voxel-tools.readthedocs.io/en/latest/api/VoxelModifierSphere/#properties)
    -   [Property Descriptions](https://voxel-tools.readthedocs.io/en/latest/api/VoxelModifierSphere/#property-descriptions)
-   [VoxelNode](https://voxel-tools.readthedocs.io/en/latest/api/VoxelNode/)
-   [VoxelRaycastResult](https://voxel-tools.readthedocs.io/en/latest/api/VoxelRaycastResult/)
-   [VoxelStream](https://voxel-tools.readthedocs.io/en/latest/api/VoxelStream/)
-   [VoxelStreamRegionFiles](https://voxel-tools.readthedocs.io/en/latest/api/VoxelStreamRegionFiles/)
-   [VoxelStreamSQLite](https://voxel-tools.readthedocs.io/en/latest/api/VoxelStreamSQLite/)
-   [VoxelStreamScript](https://voxel-tools.readthedocs.io/en/latest/api/VoxelStreamScript/)
-   [VoxelTerrain](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTerrain/)
-   [VoxelTool](https://voxel-tools.readthedocs.io/en/latest/api/VoxelTool/)
-   [VoxelToolBuffer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelToolBuffer/)
-   [VoxelToolLodTerrain](https://voxel-tools.readthedocs.io/en/latest/api/VoxelToolLodTerrain/)
-   [VoxelToolTerrain](https://voxel-tools.readthedocs.io/en/latest/api/VoxelToolTerrain/)
-   [VoxelViewer](https://voxel-tools.readthedocs.io/en/latest/api/VoxelViewer/)
-   [VoxelVoxLoader](https://voxel-tools.readthedocs.io/en/latest/api/VoxelVoxLoader/)
-   [ZN\_FastNoiseLite](https://voxel-tools.readthedocs.io/en/latest/api/ZN_FastNoiseLite/)
-   [ZN\_FastNoiseLiteGradient](https://voxel-tools.readthedocs.io/en/latest/api/ZN_FastNoiseLiteGradient/)
-   [ZN\_ThreadedTask](https://voxel-tools.readthedocs.io/en/latest/api/ZN_ThreadedTask/)

Serialization formats

-   [Voxel block format v1](https://voxel-tools.readthedocs.io/en/latest/specs/block_format_v1/)
-   [Voxel block format v2](https://voxel-tools.readthedocs.io/en/latest/specs/block_format_v2/)
-   [Voxel block format v3](https://voxel-tools.readthedocs.io/en/latest/specs/block_format_v3/)
-   [Voxel block format v4](https://voxel-tools.readthedocs.io/en/latest/specs/block_format_v4/)
-   [Compressed data format](https://voxel-tools.readthedocs.io/en/latest/specs/compressed_container/)
-   [Instance block format v0](https://voxel-tools.readthedocs.io/en/latest/specs/instances_format_v0/)
-   [Instance block format v1](https://voxel-tools.readthedocs.io/en/latest/specs/instances_format_v1/)
-   [Region format v2](https://voxel-tools.readthedocs.io/en/latest/specs/region_format_v2/)
-   [Region format v3](https://voxel-tools.readthedocs.io/en/latest/specs/region_format_v3/)
-   [SQLite format](https://voxel-tools.readthedocs.io/en/latest/specs/sqlite_format/)
-   [2](https://voxel-tools.readthedocs.io/en/latest/___2/)

[Voxel Tools documentation](https://voxel-tools.readthedocs.io/en/latest/)

-   [](https://voxel-tools.readthedocs.io/en/latest/)
  
脚本 API VoxelModifierSphere

___

##  体素修饰球

 继承：体素修饰符

##  属性：

##  属性描述

-    浮动半径 = 10.0

_  
生成于 Oct 02， 2023_
