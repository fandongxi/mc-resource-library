# 8. 服务端与联机 Servers & Multiplayer

## 8.1 服务端软件选型

| 服务端 | 用途 | 获取 |
| --- | --- | --- |
| **Vanilla 官方服务端** | 原版纯净，无插件 | https://www.minecraft.net/download/server |
| **Paper** | 插件服主流（Bukkit/Spigot 插件兼容），性能优于 Spigot | https://papermc.io |
| **Purpur** | Paper 增强版，额外玩法开关，配置自由度高 | https://purpurmc.org |
| **Spigot** | 经典插件服务端，Paper 的上游 | https://www.spigotmc.org |
| **Folia** | PaperMC 多线程分区服务端，适合大型多人生存（实验性） | https://papermc.io |
| **Fabric / Forge / NeoForge 服务端** | 模组服，与客户端加载器一致 | 各加载器官网提供服务端 jar |
| **GeyserMC + Floodgate** | 让基岩版玩家加入 Java 版服务器 | https://geysermc.org |

## 8.2 本地开服最简流程（Paper 为例）

1. 安装对应版本 Java（见 [第 2 章](02-versions.md)）。
2. 下载 Paper jar，新建文件夹，命令行运行：`java -jar paper.jar --nogui`。
3. 首次启动生成 `eula.txt`，把 `eula=false` 改为 `eula=true`。
4. 再次启动生成 `server.properties`、世界与插件文件夹。
5. 同局域网：客户端直连本机/内网 IP；外网：见 8.3。
6. 端口默认 25565，需在路由器/防火墙放行。

> 模组服：服务端加载器必须与客户端**同版本同加载器**，mods 文件夹双方一致。

## 8.3 外网联机方案

| 方案 | 适用 | 说明 |
| --- | --- | --- |
| **内网穿透 / ZeroTier / Tailscale** | 朋友小范围联机 | 虚拟局域网，免公网 IP，配置简单 |
| **Hamachi** | 小圈子怀旧 | 经典虚拟局域网，性能一般 |
| **端口转发（公网 IP）** | 长期稳定服 | 路由器做 25565 端口映射，注意安全配置 |
| **租用 VPS / 面板服** | 长期公开服 | 云厂商或专业 MC 服务商提供，省心但付费 |
| **官方 Realms** | 原版小服 | Mojang 官方托管，仅原版/官方附加包 |

## 8.4 服务器管理要点

- `server.properties`：难度、白名单 `white-list=true`、最大玩家数、正版校验 `online-mode`。
- 插件放 `plugins/`（Paper/Purpur），模组放 `mods/`（模组服）。
- 定期备份世界文件夹（`world/`），崩溃前可回滚。
- 公网服务必开白名单、限制命令权限，装好反作弊/领地类插件。
- 服主常用：LuckPerms（权限）、EssentialsX（基础指令）、WorldEdit（建筑）、CoreProtect（查区块日志）。
