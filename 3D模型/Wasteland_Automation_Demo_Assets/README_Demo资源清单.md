# 废土自动化生存 Demo 3D 资源库

整理日期：2026-08-04

## 文件夹说明

| 文件夹 | 内容 | 模型概况 |
|---|---|---:|
| `01_工具_Tools` | 镐、手斧、锤、消防斧、撬棍、石制工具 | 10 FBX |
| `02_资源废料_Resources` | 木材、石料、金属板、原木、岩石 | 12 FBX |
| `03_自动化设备_Automation` | 传送带、弯道、分流、机械臂、机器、管道、阀门、厂房组件 | 143 FBX + OBJ + GLB |
| `04_能源系统_Energy` | 太阳能板 | 1 GLB |
| `05_储存容器_Storage` | 箱子、木桶、桶、瓶子、宝箱 | 10 FBX |
| `06_基地建造_BaseBuilding` | 墙、门、窗、屋顶和模块化建筑组件 | 79 FBX + OBJ + GLB |
| `07_废土废墟_Ruins` | 7 类高楼废墟、广告牌、残骸 | 10 FBX + Blend |
| `08_防御设施_Defense` | 模块化炮塔、武器、防御塔、地形组件 | 160 FBX + OBJ + GLB |
| `09_敌人与角色_Characters` | 50+ 动画角色，包含僵尸及人形角色 | 52 FBX + OBJ + Blend |
| `10_运输载具_Vehicles` | 轿车、货车、救护车、消防车、车轮和车辆碎片 | 50 FBX + OBJ + GLB |

## 第一版场景推荐

不要一次把所有模型放进项目。先从每类挑选以下内容：

1. 工具：镐、斧、撬棍、锤。
2. 资源：木材、石料、金属板、废料箱。
3. 自动化：直线传送带、转弯、T 型分流、机械臂、基础机器、管道与阀门。
4. 能源：太阳能板；发电机和电池暂时用 Factory Kit 的机器/箱体占位。
5. 储存：大箱、桶、料斗；Factory Kit 中也包含适合输入/输出端的结构件。
6. 建造：地板、墙、门、屋顶各 2–3 个模块。
7. 环境：2 个完整废墟、3 个残骸/广告牌作为背景变化。
8. 防御：一种炮塔底座、一种枪械上层、围墙或路障。
9. 敌人：一个僵尸、一个掠夺者占位角色。
10. 运输：一辆 Van 或 Pickup 风格车辆，加独立车轮。

这样可以控制在约 45–60 个实际导入模型内，同时覆盖“搜刮 → 储存 → 加工 → 自动生产 → 防守 → 扩张”的闭环。

## 许可与来源

- Factory Kit 3.0 — Kenney — CC0  
  https://opengameart.org/content/conveyor-kit
- Building Kit — Kenney — CC0  
  https://opengameart.org/content/building-kit
- Tower Defense Kit — Kenney — CC0  
  https://opengameart.org/content/tower-defense-kit
- Car Kit 3.1 — Kenney — CC0  
  https://opengameart.org/content/car-kit
- Animated Characters Pack — Quaternius — CC0  
  https://opengameart.org/content/animated-characters-pack
- 3D Apocalyptic Building / City — Majadroid — CC0  
  https://opengameart.org/content/3d-apocalyptic-building-city-cc0
- Survival Kit — Kenney — CC0  
  https://opengameart.org/content/survival-kit
- Survival Tools PBR、Fire Axe、Stone Axe & Pickaxe — CC0，详见 `01_工具_Tools/Realistic_PBR_Tools/README_写实资源清单.md`。
- Crowbar PBR — Fab 页面许可字段显示 CC BY 4.0；署名 `plaggy`。不要当作 CC0 发布。
- Solar Panel — Jummit — CC BY 4.0 / GPL 3.0；本库按 CC BY 4.0 使用并署名。  
  https://opengameart.org/content/solar-panel

原始下载包保存在各分类的 `_原始包` 文件夹中。发布游戏前不要删除许可证和本清单。

## Unity 导入建议

- Kenney 资源优先导入 FBX；GLB 可作为跨引擎备份。
- 每个大型资源包只复制 Demo 真正使用的模型到 Unity `Assets/`，不要整包全部导入。
- 建筑与传送带统一使用网格吸附。
- 传送带、机器、容器设置明确的输入/输出空物体。
- 角色 FBX 在 Rig 面板中设置为 Humanoid 后再测试动画。
- 写实工具和废墟与 Kenney 低模风格不同，正式美术阶段需要统一材质、色调和细节密度。

