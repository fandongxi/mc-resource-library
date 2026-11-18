# 3. 模组加载器 Mod Loaders

加载器是模组运行的底座。**同一模组只支持特定加载器与特定游戏版本**，三者必须同时匹配。

## 3.1 四大加载器对比

| 加载器 | 起源 | 生态特点 | 适用 |
| --- | --- | --- | --- |
| **Forge** | 社区老牌（2012–） | 内容模组（科技/魔法）最丰富；1.20.1 为其末期主线版本，官方后续转向 NeoForge | 1.20.1 及更早内容模组包 |
| **NeoForge** | Forge 核心开发者分叉（1.20.1 起） | 1.21+ 的 Forge 系正统，API 更干净、更新更快 | 1.20.1 兼容起步，1.21+ 主流 |
| **Fabric** | 轻量独立工具链 | 更新极快、体积小；性能优化模组（Sodium 系）与新特性模组集中在此 | 追求帧数、新版本、轻量模组 |
| **Quilt** | Fabric 的社区分叉 | 兼容绝大多数 Fabric 模组，额外提供部分 API | 想尝试 Fabric 生态的进阶玩家 |

> LiteLoader 已基本淘汰，不再推荐。

## 3.2 选型建议

- 玩**大型科技/魔法整合包**（格雷科技、AE2、匠魂、暮色森林等）：看整合包用什么加载器，1.20.1 多为 Forge/NeoForge。
- 玩**轻量化、高帧数、现代优化**：Fabric（Sodium + Lithium 优化全家桶）。
- **光影**：Fabric 用 Iris+Sodium；Forge 低版本用 OptiFine，高版本用 Embeddium+Oculus；详见 [第 6 章](06-shaders.md)。
- Forge 与 NeoForge 模组**绝大多数不互通**；Fabric 模组一般可在 Quilt 上运行。

## 3.3 安装方式

1. **启动器内一键安装**（PCL2 / HMCL / Prism）：选好游戏版本 → 安装对应加载器，最省心。
2. 官方安装器：
   - Forge：https://files.minecraftforge.net
   - NeoForge：https://neoforged.net
   - Fabric：https://fabricmc.net （中文文档：https://docs.fabricmc.net/zh_cn/）
3. 安装后在版本列表确认出现加载器标识，再向 `mods` 文件夹放入对应模组。

## 3.4 常见依赖

许多模组需要前置库（Library / API）单独安装，否则崩溃或不加载，常见：

- **JEI**（查看配方，几乎所有内容包必备）
- **Architectury API**（跨加载器模组的公共前置）
- **Kotlin for Forge / Fabric**（Kotlin 编写模组的前置）
- **CUP / Cloth Config / owo-lib**（配置界面前置）

> 启动器和模组页面会标注所需前置，下载时按提示补齐。
