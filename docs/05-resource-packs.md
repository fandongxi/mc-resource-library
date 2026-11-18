# 5. 资源包（材质包）Resource Packs

资源包只改外观（方块/物品 UI/音效），**不改玩法**，与模组独立安装，可叠加多个。

## 5.1 安装位置

- Java 版：`.minecraft/resourcepacks/` 文件夹，游戏内「选项 → 资源包」启用并调整优先级。
- 基岩版：`.mcpack` 文件双击导入。
- 光影包与材质包互不冲突，可同时开。

## 5.2 风格分类与获取

| 风格 | 代表方向 | 获取渠道 |
| --- | --- | --- |
| 原版延续 / 轻微优化 | Faithful 系列（原版 32x 放大、更清晰）、Vanilla Tweaks（微改补丁式） | Modrinth / CurseForge / planetminecraft.com |
| 高清写实 | 128x–512x 超清材质，吃显存，需高性能显卡 | CurseForge 材质分类 |
| 卡通/低多边形 | 像素可爱、扁平化，低配流畅 | Modrinth |
| PvP / 竞技 | 低分辨率、突出物品轮廓、透明 UI，适合对战 | 社区分发 |
| 中文 UI / 字体 | 界面汉化字体、竖排古风 | 中文社区（见 [第 13 章](13-chinese-localization.md)） |

## 5.3 获取站点

- Modrinth 材质区：https://modrinth.com/resourcepacks
- CurseForge 材质区：https://www.curseforge.com/minecraft/texture-packs
- Planet Minecraft（皮肤/材质/建筑图库）：https://www.planetminecraft.com
- Vanilla Tweaks（原版微调合集）：https://vanillatweaks.net

## 5.4 注意事项

1. 分辨率越高越吃性能；低配从 16x/32x 起步。
2. 材质包需匹配游戏版本，高版本材质在低版本可能缺方块贴图（显示为紫黑）。
3. 多个材质包时，**列表上方优先级更高**，冲突时以上方为准。
4. 不要把光影包（.zip 里是 shaders 配置）放进 resourcepacks，光影放 `shaderpacks` 文件夹。
