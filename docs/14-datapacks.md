# 14. 数据包 Data Packs

数据包是**纯原版机制**的轻量内容包：不改模组、不需客户端安装，放入世界即可生效，服务器/单机通用，适合在原版或轻量服上加内容。

## 14.0 全量入口

| 平台 | 全部数据包入口 |
| --- | --- |
| **Modrinth** | https://modrinth.com/datapacks |
| **CurseForge** | https://www.curseforge.com/minecraft/search?class=data-packs （Data Packs 分类） |
| **Vanilla Tweaks** | https://vanillatweaks.net/picker/datapacks/ （勾选式 QoL 合集） |

## 14.1 安装方法

1. 单机：`.minecraft/saves/<存档>/datapacks/`，把数据包文件夹或 zip 放入。
2. 服务器：`world/datapacks/`。
3. 进游戏执行 `/reload`，或重启世界；用 `/datapack list` 查看是否加载。
4. 数据包需匹配游戏版本；部分含函数的包换版本可能失效。

## 14.2 世界生成类

| 数据包 | 说明 | 搜索 |
| --- | --- | --- |
| **Terralith** | 95+ 新群系、火山/樱花谷，纯维度重做（Modrinth 下载量顶级） | https://modrinth.com/datapacks?q=Terralith |
| **Tectonic** | 更大更起伏的地形塑造 | https://modrinth.com/datapacks?q=Tectonic |
| **Incredible Defaults** | 优化原版地貌生成 | https://modrinth.com/datapacks?q=Incredible+Defaults |
| **Nullscape** | 下界重做 | https://modrinth.com/datapacks?q=Nullscape |
| **Incendium Legacy** | 下界群系改造 + 挑战结构与武器 | https://modrinth.com/datapacks?q=Incendium |

## 14.3 结构 / 探险类

| 数据包 | 说明 | 搜索 |
| --- | --- | --- |
| **Dungeons and Taverns** | 酒馆与地牢结构 | https://modrinth.com/datapacks?q=Dungeons+and+Taverns |
| **Trek** | 替代原版结构生成 | https://modrinth.com/datapacks?q=Trek |
| **Explorify** | 简洁友好的新结构合集 | https://modrinth.com/datapacks?q=Explorify |

## 14.4 QoL / 工具类

| 数据包 | 说明 | 搜索 |
| --- | --- | --- |
| **VeinMiner** | 连锁挖矿（按住指定键挖整矿脉） | https://modrinth.com/datapacks?q=VeinMiner |
| **Graves / Player Graves** | 死亡掉落生成墓碑，可找回物品 | https://modrinth.com/datapacks?q=Graves |
| **More Mob Variants** | 更多生物毛色变种 | https://modrinth.com/datapacks?q=More+Mob+Variants |
| **Custom Nether Portals** | 用不同方块搭下界传送门 | https://modrinth.com/datapacks?q=Custom+Nether+Portals |
| **Stackable Shulker Boxes** | 潜影盒可堆叠 | https://modrinth.com/datapacks?q=Stackable+Shulker |
| **Craftable Bundles** | 可合成收纳袋 | https://modrinth.com/datapacks?q=Craftable+Bundles |
| **Leaf Decay / 树叶快速腐烂** | 清理树林更方便 | https://modrinth.com/datapacks?q=Leaf+Decay |
| **Vanilla Tweaks 合集** | 生物头颅、玩家墓碑、自定义成就等勾选打包 | https://vanillatweaks.net/picker/datapacks/ |

## 14.5 数据包 vs 模组

| 维度 | 数据包 | 模组 |
| --- | --- | --- |
| 是否需加载器 | 否，原生运行 | 需 Forge/Fabric/NeoForge |
| 客户端是否要装 | 否（服务器装即可） | 联机双方版本需一致 |
| 能加新方块/机器 | 基本不能（原版机制内） | 能 |
| 适合 | 原版+/轻量服微调 | 深度玩法改造 |
