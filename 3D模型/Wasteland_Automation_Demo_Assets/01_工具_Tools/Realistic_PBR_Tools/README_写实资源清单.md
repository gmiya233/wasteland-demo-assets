# Unity 写实 / PBR 生存工具资源

下载日期：2026-08-04

## 已下载并解压

### Survival Tools PBR

- 路径：`SurvivalTools_PBR/`
- 内容：写实锤、手斧、镐；通用版和 UE4 版各一套，共 6 个 FBX。
- 规格：锤 680 tris、手斧 860 tris、镐 2008 tris，共享 2K PBR 纹理。
- Unity 推荐：使用 General/通用版本；UE4 版本附带的碰撞设置不适合直接照搬。
- 许可：CC0。
- 来源：https://opengameart.org/content/survival-tools

### Fire Axe

- 路径：`Fireaxe_CC0/`
- 内容：消防斧，386 tris；Diffuse、Normal、Specular 纹理（512×512）。
- 许可：CC0。
- 来源：https://opengameart.org/content/fire-axe
- 原包：`Fireaxe_CC0.zip`

### Stone Axe & Pickaxe

- 路径：`Stone_Axe_Pickaxe_CC0/`
- 内容：石斧与石镐，约 700–900 tris，1024 纹理。
- 许可：CC0。
- 来源：https://opengameart.org/content/stone-axe-pickaxe
- 原包：`Stone_Axe_Pickaxe_CC0.zip`

### Crowbar PBR

- 路径：`Crowbar_PBR_CC-BY-4.0/`
- 内容：写实旧化撬棍 FBX，含 Albedo、AO、Metallic、Normal、Roughness PBR 纹理，高模烘焙法线。
- 来源：https://www.fab.com/listings/4419aba1-109f-4aad-b773-94b0687483ae
- 许可注意：作者描述写 CC0，但 Fab 当前 `License terms` 字段显示 CC BY 4.0。存在冲突，应按更严格的 CC BY 4.0 使用并署名作者 `plaggy`，除非取得作者进一步确认。
- 建议署名：`Crowbar 3D model by plaggy, licensed under CC BY 4.0.`
- 原包：`cc0-crowbar_CC-BY-4.0.zip`

## Unity 材质设置

- Built-in Standard：Albedo → Albedo，Normal → Normal Map，Specular 工作流使用 Standard (Specular setup)。
- URP Lit：Diffuse/Albedo → Base Map，Normal → Normal Map；Metallic 与 Smoothness 需要按纹理类型设置。
- Roughness 转 Smoothness：`Smoothness = 1 - Roughness`。如果只有 Roughness 图，需反相后放入 Metallic/Mask Map 的 Alpha。
- 导入法线贴图后，将 Texture Type 改为 `Normal map`。
- 推荐为手持工具建立单独的 Grip 空物体，避免直接修改模型原点。
