# Unity 生存工具 3D 资源清单

下载日期：2026-08-04

这些资源均来自 OpenGameArt 的原作者/发布页面，页面标注为 CC0。可用于个人或商业项目，通常无需署名。发布前仍建议保留本清单并再次核对来源页面。

## 已下载并解压

### Kenney Survival Kit

- 文件夹：`kenney_survival-kit/`
- 内容：80 个低多边形生存模型，包括斧、镐、锤、铲、锄，以及建筑、资源和营地道具。
- 格式：FBX、OBJ、GLB，附纹理。
- Unity：优先使用 FBX；把整个模型目录复制进项目的 `Assets/`。
- 许可：CC0；署名 Kenney.nl 非强制。
- 来源：https://opengameart.org/content/survival-kit
- 原始包：`kenney_survival-kit.zip`

### Stylized Low Poly Tools

- 文件夹：`low_poly_tools/`
- 内容：镐、锤、铲、锄、斧，含游戏图标。
- 许可：CC0。
- 来源：https://opengameart.org/content/stylized-low-poly-tools
- 原始包：`low_poly_tools.zip`

### Crowbar

- 文件夹：`crowbar/`
- 内容：低多边形撬棍。
- 格式：Blender `.blend`。Unity 通常需要本机安装 Blender 才能直接导入；更稳妥的做法是在 Blender 中导出 FBX。
- 许可：CC0。
- 来源：https://opengameart.org/content/crowbar
- 原始包：`crowbar.zip`

## 已下载、尚未解压

### Survival Tools PBR

- 原始包：`survivaltools.7z`
- 内容：锤（680 tris）、手斧（860 tris）、镐（2008 tris），共享 2K PBR 纹理；包含通用版本和带碰撞的 UE4 版本。
- 许可：CC0。
- 来源：https://opengameart.org/content/survival-tools
- 当前 Windows 自带 tar 不支持此 7z 的 LZMA 编码。可用 7-Zip 解压；Unity 应选通用版本（General/no collision）。

## Unity 导入建议

1. 先使用 Kenney 包的 FBX，风格统一、体积小，最适合快速 Demo。
2. 在模型 Import Settings 中检查 `Scale Factor`，以 1 Unity Unit = 1 米为准。
3. 手持道具建议建立空父物体作为握持点，再微调位置和旋转。
4. 碰撞体优先用 Box/Capsule 组合，避免给低模工具直接使用复杂 Mesh Collider。
5. Built-in/URP 材质若显示粉色，重新创建对应管线的 Lit 材质并挂载纹理。

