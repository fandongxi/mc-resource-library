# 6. 光影 Shaders

光影通过阴影、水面反射、体积光、大气雾提升画面，对显卡要求较高。

## 6.0 全量入口

| 平台 | 全部光影入口 |
| --- | --- |
| **Modrinth** | https://modrinth.com/shaders |
| **CurseForge** | https://www.curseforge.com/minecraft/shaders |
| **Iris 官网** | https://irisshaders.dev （加载器与安装器） |

## 6.1 加载方案（按加载器选）

| 方案 | 适用 | 说明 |
| --- | --- | --- |
| **OptiFine** | 仅 Forge（低版本经典） | 自带光影入口与性能选项；高版本 Forge 渐被 Embeddium/Oculus 取代 |
| **Iris + Sodium** | Fabric（1.16.5+）/ NeoForge（1.21.1+） | 开源、帧数高、兼容绝大多数 OptiFine 光影，当前主流 |
| **Embeddium + Oculus** | Forge 高版本 | Sodium / Iris 的 Forge 非官方移植 |

- 光影包放置：`.minecraft/shaderpacks/`，游戏内「视频设置 → 光影」选择。

## 6.2 主流光影精选（Modrinth 搜索直达）

| 光影 | 风格/定位 | 搜索 |
| --- | --- | --- |
| **Complementary Reimagined / Unbound** | 现代明亮、兼容性最好，新手首选 | https://modrinth.com/shaders?q=Complementary |
| **BSL Shaders** | 柔和自然，经典大众款，低配可跑 | https://modrinth.com/shaders?q=BSL |
| **Sildur's Vibrant / Enhanced / Default+** | 鲜艳/增强/原版风，多档性能 | https://modrinth.com/shaders?q=Sildurs |
| **SEUS PTGI** | 路径追踪写实，硬件要求高 | https://modrinth.com/shaders?q=SEUS |
| **Kappa** | 电影感，阴影与体积光出色 | https://modrinth.com/shaders?q=Kappa |
| **Nostalgia** | 复古柔和 | https://modrinth.com/shaders?q=Nostalgia |
| **Bliss** | 清新治愈轻量款 | https://modrinth.com/shaders?q=Bliss |
| **Photon** | 鲜艳高对比，近年热门 | https://modrinth.com/shaders?q=Photon |
| **MakeUp Ultra Fast** | 低配高效光影 | https://modrinth.com/shaders?q=MakeUp |
| **Chocapic13 V9** | 经典可调高自由度 | https://modrinth.com/shaders?q=Chocapic13 |
| **Continuum** | 写实电影级 | https://modrinth.com/shaders?q=Continuum |
| **Rethinking Voxels** | 新一代体素光照方向 | https://modrinth.com/shaders?q=Rethinking+Voxels |
| **AstraLex** | 明亮清爽向 | https://modrinth.com/shaders?q=AstraLex |

> Sildur's 官方安装说明：https://sildurs-shaders.github.io/install/

## 6.3 性能建议

1. 先装 Sodium/Embeddium 再开光影，帧数差距巨大。
2. 阴影距离、体积光、反射是三大性能杀手，低配先关阴影。
3. 集显/老显卡用 BSL、Sildur's Default+ 等轻量款，不要硬上 PTGI。
4. 光影与「核心着色器类材质包」可能冲突，二选一。
