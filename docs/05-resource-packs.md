# 5. 资源包（材质包）Resource Packs

资源包只改外观（方块/物品/UI/音效），不改玩法，可叠加多个，与模组、光影独立。

## 5.0 全量入口

| 平台 | 全部材质入口 |
| --- | --- |
| **Modrinth** | https://modrinth.com/resourcepacks |
| **CurseForge** | https://www.curseforge.com/minecraft/texture-packs |
| **Planet Minecraft** | https://www.planetminecraft.com/resources/texture_packs （社区作品库） |
| **Vanilla Tweaks** | https://vanillatweaks.net （原版微调补丁合集） |

## 5.1 安装位置

- Java 版：`.minecraft/resourcepacks/`，游戏内「选项 → 资源包」启用并调优先级。
- 基岩版：`.mcpack` 双击导入。
- 材质包与光影包互不冲突，可同时开。

## 5.2 知名材质精选（Modrinth 搜索直达）

| 材质 | 风格 | 搜索 |
| --- | --- | --- |
| **Faithful 32x / 64x** | 原版放大、更清晰，最流行 | https://modrinth.com/resourcepacks?q=Faithful |
| **Vanilla Tweaks** | 原版微调（UI/像素/连接纹理） | https://modrinth.com/resourcepacks?q=Vanilla+Tweaks |
| **Pixel Perfection** | 复古 16x 像素 | https://modrinth.com/resourcepacks?q=Pixel+Perfection |
| **Dokucraft** | 暗黑/高童话分支经典老包 | https://modrinth.com/resourcepacks?q=Dokucraft |
| **Sphax PureBDcraft** | 卡通方块漫画风 | https://modrinth.com/resourcepacks?q=PureBDcraft |
| **John Smith Legacy** | 中世纪写实 32x | https://modrinth.com/resourcepacks?q=John+Smith |
| **Jicklus** | 柔和手绘田园风 | https://modrinth.com/resourcepacks?q=Jicklus |
| **Soartex Fanver** | 干净明亮 32x | https://modrinth.com/resourcepacks?q=Soartex |
| **Retro 16x / 32x** | 早期版本怀旧像素 | https://modrinth.com/resourcepacks?q=Retro |
| **PvP 低火/小图腾类** | 竞技对战优化 | https://modrinth.com/resourcepacks?q=PvP |

## 5.3 风格分类（在平台按标签筛选）

- **原版延续/轻微优化**：Faithful、Vanilla Tweaks，低配友好。
- **高清写实**：128x–512x，吃显存，需高性能显卡。
- **卡通/低多边形**：像素可爱、扁平化，低配流畅。
- **PvP/竞技**：低分辨率、突出物品轮廓、透明 UI。
- **中文 UI/字体**：界面汉化字体、古风竖排（见 [第 13 章](13-chinese-localization.md)）。

## 5.4 注意事项

1. 分辨率越高越吃性能，低配从 16x/32x 起步。
2. 材质需匹配游戏版本，高版本材质在低版本可能缺贴图（紫黑方块）。
3. 多材质包时列表上方优先级更高。
4. 光影包（shaders 配置）放 `shaderpacks/`，不要放进 resourcepacks。
