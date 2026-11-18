# 6. 光影 Shaders

光影通过光线追踪式渲染（阴影、水面反射、体积光、大气雾）提升画面，**对显卡要求较高**。

## 6.1 加载方案（按加载器选）

| 方案 | 适用 | 说明 |
| --- | --- | --- |
| **OptiFine** | 仅 Forge（低版本经典） | 自带光影入口与性能选项，老牌方案；高版本 Forge 已逐渐被 Embeddium/Oculus 取代 |
| **Iris + Sodium** | Fabric（1.16.5+）/ NeoForge（1.21.1+） | 开源、帧数高、兼容绝大多数 OptiFine 光影包，当前主流 |
| **Embeddium + Oculus** | Forge 高版本 | Sodium / Iris 的 Forge 非官方移植，Forge 玩家光影方案 |

- Iris 官网：https://irisshaders.dev （安装器自动带上 Sodium）
- 光影包放置：`.minecraft/shaderpacks/`，游戏内「视频设置 → 光影」选择。

## 6.2 主流光影包

| 光影 | 风格 | 特点 |
| --- | --- | --- |
| **Complementary Shaders**（Reimagined / Unbound） | 现代明亮、平衡 | 兼容性最好、可调项丰富，新手首选 |
| **BSL Shaders** | 柔和自然 | 经典大众款，配置低也能跑 |
| **Sildur's Vibrant / Enhanced / Default+** | 鲜艳 / 增强 / 原版风 | 多档性能版本，低配友好 |
| **SEUS PTGI** | 路径追踪写实 | 画面顶级，硬件要求高 |
| **Kappa** | 电影感 | 阴影与体积光出色 |
| **Nostalgia** | 复古柔和 | 怀旧氛围 |
| **Bliss** | 清新治愈 | 近年热门轻量款 |

> 光影包在 Modrinth / CurseForge 与各作者官网分发；Sildur's 安装说明见 https://sildurs-shaders.github.io/install/

## 6.3 性能建议

1. 先开 Sodium/Embeddium 再装光影，帧数差距巨大。
2. 阴影距离、体积光、反射是三大性能杀手，低配先关阴影。
3. 集显/老显卡用 BSL、Sildur's Default+ 等轻量款；不要硬上 PTGI。
4. 光影与「核心着色器类材质包」可能冲突，二选一。
