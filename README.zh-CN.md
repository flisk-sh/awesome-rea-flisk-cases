# Awesome REA + TDK 案例

**[English](README.md)** | 简体中文 | [繁體中文](README.zh-TW.md)

一份精选的逆向工程案例合集：用 AI 代理通过 [REA](https://github.com/morluto/rea) 分析应用，再用 [TDK CLI](https://github.com/flisk-sh/flisk) 把分析结果变成可以在本地运行的服务栈。

每个案例回答三个问题：

1. **REA 发现了什么？** 行为、接口、数据格式或二进制细节，并附上证据。
2. **TDK 搭建了什么？** 复现应用有用行为的本地服务、数据和运行环境。
3. **可以复用什么？** 让这些工作成功的提示词和技能。

## 工作流程

```text
REA（代理 + CLI/MCP） → findings.md → tdk project / tdk resource → tdk up → 运行并检查
```

1. 让 REA 分析你有权分析的应用或二进制文件。
2. 把发现保存到 `findings.md`：接口、协议、数据格式和未解决的问题。
3. 用 TDK 搭建与发现相符的服务，然后用 `tdk up` 启动。
4. 把哪些有效、哪些无效记录到案例文件里。

从 [prompts/](prompts/) 中的提示词开始。

## 案例

下表中的状态说明来源资料支持到什么程度。这些案例都还没有 TDK 构建，部分 REA 声称尚未验证。

| 案例 | 对象 | 状态 |
| :--- | :--- | :--- |
| [Brother 扫描按钮连接 NAS](cases/brother-scan-to-nas.md) | Brother 扫描仪，SMB/FTP/S3 存储 | 构想 |
| [NJFE 耳镜摄像头桥接](cases/njfe-ear-camera-bridge.md) | PC 上的 Wi-Fi 耳镜摄像头 | 构想 |
| [智能马桶控制](cases/smart-toilet-desktop-control.md) | 蓝牙智能马桶 | 构想 |
| [Urban Terror 浏览器版](cases/urban-terror-browser.md) | Urban Terror（Quake III 引擎） | 有报道，未使用 REA |
| [LG PlxNative Plex 客户端](cases/lg-plxnative-plex-client.md) | LG 电视媒体客户端 | 有报道，未使用 REA |
| [T6 在线恢复](cases/t6-online-restoration.md) | 已停服的多人后端 | 待验证 |
| [Pre-CU Star Wars Galaxies 模拟器](cases/pre-cu-swg-emulator.md) | MMO 服务器模拟器 | 待验证 |
| [The Incredible Machine 浏览器版](cases/incredible-machine-browser.md) | 浏览器益智游戏 | 待验证 |
| [H1Z1：从逆向到 MMO 后端](cases/h1z1-mmo-backend.md) | 在线生存射击游戏 | 进行中（有报道） |
| [Red Alert 2 强化学习环境](cases/red-alert-2-rl-environment.md) | 即时战略游戏引擎 | 待验证 |
| [Animal Jam / Burrow 客户端与服务器](cases/animal-jam-burrow-client-server.md) | 在线游戏客户端与服务器 | 待验证（未确认） |
| [浏览器版 Counter-Strike](cases/browser-counter-strike-multiplayer.md) | 浏览器多人射击游戏 | 待验证 |
| [Three Kingdoms XIV: trainer functions as an MCP server](cases/three-kingdoms-mcp-tools.md) | Romance of the Three Kingdoms XIV | Needs verification |
| [Hearthstone on macOS: game-control agent, deck optimizer and replay review](cases/hearthstone-macos-agent.md) | Hearthstone | Needs verification |
| [Mobile game interactions: an evidence pipeline with Codex and REA](cases/mobile-game-evidence-pipeline.md) | Mobile game | In progress |
| [Dragon Ball Budokai: browser port with a local game server](cases/dragon-ball-budokai-browser-port.md) | Dragon Ball Budokai | Needs verification |

通过 [CONTRIBUTING.md](CONTRIBUTING.md) 添加案例。

## 范围与许可

- 只分析你拥有或获得许可分析的软件。不要在案例中包含专有资源、密钥、凭据或私人数据。
- 只提供摘要和链接。描述证据，不要粘贴整个二进制文件或受版权保护的代码。
- 案例记录的是作者的观察。除非案例中注明，否则都未经独立验证。

## 许可证

本仓库的整理内容和代码：[MIT](LICENSE)。链接的项目保留各自的许可证。
