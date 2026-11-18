# 9. 指令与命令方块 Commands

> 指令在聊天框输入，`/` 开头；命令方块需开启作弊（创建世界时允许作弊，或 OP 权限）。
> 坐标格式 `x y z`；`~` 代表相对当前位置，`~10` 即向前 10 格。

## 9.1 高频基础指令

| 指令 | 作用 |
| --- | --- |
| `/gamemode survival|creative|adventure|spectator` | 切换游戏模式 |
| `/give <玩家> <物品> [数量]` | 给予物品，如 `/give Steve minecraft:diamond 64` |
| `/tp <玩家> <目标或坐标>` | 传送，`/tp @s ~ ~ ~` 原地 |
| `/teleport` | 同 tp，支持跨维度参数 |
| `/summon <实体> [坐标]` | 召唤实体，如 `/summon minecraft:cow` |
| `/locate structure|biome <名称>` | 定位结构/群系（新版为 `/locate structure village_plains`） |
| `/fill <起点> <终点> <方块> [替换方式]` | 批量填充方块，如 `/fill ~ ~ ~ ~10 ~5 ~10 glass hollow` |
| `/setblock <坐标> <方块>` | 放置单个方块 |
| `/clone <起> <终> <目标>` | 复制区域 |
| `/kill <目标>` | 清除实体（`/kill @e` 清全部，慎用） |
| `/experience add <玩家> <数量> points|levels` | 给经验 |
| `/effect give <玩家> <效果> [秒] [等级]` | 施加药水效果 |
| `/enchant <玩家> <附魔> [等级]` | 手持物品附魔 |
| `/weather clear|rain|thunder` | 天气 |
| `/time set day|night|1000` | 时间 |
| `/difficulty peaceful|easy|normal|hard` | 难度 |
| `/spawnpoint [玩家] [坐标]` | 设置重生点 |
| `/spreadplayers <x> <z> <间距> 1 <目标>` | 随机散布玩家 |

## 9.2 选择器（@a / @e / @p / @s）

| 选择器 | 含义 | 常用参数 |
| --- | --- | --- |
| `@p` | 最近玩家 | `[distance=..10]` 10 格内 |
| `@a` | 所有玩家 | `[type=player]`、`[team=red]` |
| `@e` | 所有实体 | `[type=zombie,limit=5]`、`[tag=foo]` |
| `@s` | 执行者自身 | — |

## 9.3 gamerule 常用规则

| 规则 | 作用（true/false） |
| --- | --- |
| `keepInventory` | 死亡不掉落 |
| `mobGriefing` | 怪物是否破坏方块（苦力怕爆炸、末影人搬砖） |
| `doDaylightCycle` | 昼夜循环 |
| `doWeatherCycle` | 天气循环 |
| `doMobSpawning` | 自然刷怪 |
| `naturalRegeneration` | 自然回血 |
| `fallDamage` | 跌落伤害 |
| `mobDamage` | 生物造成伤害 |
| `commandBlockOutput` | 命令方块输出是否刷屏 |
| `randomTickSpeed` | 随机刻速度（作物生长、火焰蔓延，数字越大越快） |

示例：`/gamerule keepInventory true`

## 9.4 execute 链入门（高级）

`execute` 是条件执行框架，骨架：

```
execute as @p at @s if block ~ ~-1 ~ minecraft:stone run say 你站在石头上
```

- `as`：改变执行者，`at`：改变执行位置。
- `if block / if entity / if score`：条件判断。
- `run`：满足后执行的指令。
- 可链式嵌套，做检测+触发机关。

## 9.5 命令方块

1. `/give @s minecraft:command_block` 获取。
2. 右键放置，三种模式：**脉冲**（红石触发一次）、**循环**（每刻执行）、**连锁**（前一个成功后执行）。
3. 勾选「始终激活」可免红石；「条件制约」为条件执行。
4. 红石比较器可读取命令方块成功输出强度，用于计分板逻辑。
5. 大型装置配合 `/scoreboard`（计分板）与 `/tellraw`（发送格式化文字）做剧情/UI。

## 9.6 学习资源

- 中文官方 Wiki 指令页：https://zh.minecraft.wiki （搜索对应指令）
- B 站 / YouTube 搜「命令方块教程」，从脉冲灯、抽奖机、打怪刷塔逐级练。
