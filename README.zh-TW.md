# Awesome REA + TDK 案例

**[English](README.md)** | [简体中文](README.zh-CN.md) | 繁體中文

一份精選的逆向工程案例合集：用 AI 代理透過 [REA](https://github.com/morluto/rea) 分析應用，再用 [TDK CLI](https://github.com/flisk-sh/flisk) 把分析結果變成可以在本機執行的服務堆疊。

每個案例回答三個問題：

1. **REA 發現了什麼？** 行為、介面、資料格式或二進位細節，並附上證據。
2. **TDK 搭建了什麼？** 重現應用有用行為的本機服務、資料和執行環境。
3. **可以重複使用什麼？** 讓這些工作成功的提示詞和技能。

## 工作流程

```text
REA（代理 + CLI/MCP） → findings.md → tdk project / tdk resource → tdk up → 執行並檢查
```

1. 讓 REA 分析你有權分析的應用或二進位檔。
2. 把發現儲存到 `findings.md`：介面、協定、資料格式和尚未解決的問題。
3. 用 TDK 搭建與發現相符的服務，然後用 `tdk up` 啟動。
4. 把哪些有效、哪些無效記錄到案例檔裡。

從 [prompts/](prompts/) 中的提示詞開始。

## 案例

下表中的狀態說明來源資料支援到什麼程度。這些案例都還沒有 TDK 建置，部分 REA 聲稱尚未驗證。

| 案例 | 對象 | 狀態 |
| :--- | :--- | :--- |
| [Brother 掃描按鈕連接 NAS](cases/brother-scan-to-nas.md) | Brother 掃描器，SMB/FTP/S3 儲存 | 構想 |
| [NJFE 耳鏡攝影機橋接](cases/njfe-ear-camera-bridge.md) | PC 上的 Wi-Fi 耳鏡攝影機 | 構想 |
| [智慧馬桶控制](cases/smart-toilet-desktop-control.md) | 藍牙智慧馬桶 | 構想 |
| [Urban Terror 瀏覽器版](cases/urban-terror-browser.md) | Urban Terror（Quake III 引擎） | 有報導，未使用 REA |
| [LG PlxNative Plex 用戶端](cases/lg-plxnative-plex-client.md) | LG 電視媒體用戶端 | 有報導，未使用 REA |
| [T6 線上恢復](cases/t6-online-restoration.md) | 已停服的多人後端 | 待驗證 |
| [Pre-CU Star Wars Galaxies 模擬器](cases/pre-cu-swg-emulator.md) | MMO 伺服器模擬器 | 待驗證 |
| [The Incredible Machine 瀏覽器版](cases/incredible-machine-browser.md) | 瀏覽器益智遊戲 | 待驗證 |
| [H1Z1：從逆向到 MMO 後端](cases/h1z1-mmo-backend.md) | 線上生存射擊遊戲 | 進行中（有報導） |
| [Red Alert 2 強化學習環境](cases/red-alert-2-rl-environment.md) | 即時戰略遊戲引擎 | 待驗證 |
| [Animal Jam / Burrow 用戶端與伺服器](cases/animal-jam-burrow-client-server.md) | 線上遊戲用戶端與伺服器 | 待驗證（未確認） |
| [瀏覽器版 Counter-Strike](cases/browser-counter-strike-multiplayer.md) | 瀏覽器多人射擊遊戲 | 待驗證 |
| [Three Kingdoms XIV: trainer functions as an MCP server](cases/three-kingdoms-mcp-tools.md) | Romance of the Three Kingdoms XIV | Needs verification |
| [Hearthstone on macOS: game-control agent, deck optimizer and replay review](cases/hearthstone-macos-agent.md) | Hearthstone | Needs verification |
| [Mobile game interactions: an evidence pipeline with Codex and REA](cases/mobile-game-evidence-pipeline.md) | Mobile game | In progress |
| [Dragon Ball Budokai: browser port with a local game server](cases/dragon-ball-budokai-browser-port.md) | Dragon Ball Budokai | Needs verification |

透過 [CONTRIBUTING.md](CONTRIBUTING.md) 新增案例。

## 範圍與授權

- 只分析你擁有或取得許可分析的軟體。不要在案例中包含專有資源、金鑰、憑證或私人資料。
- 只提供摘要和連結。描述證據，不要貼上整個二進位檔或受著作權保護的程式碼。
- 案例記錄的是作者的觀察。除非案例中註明，否則都未經獨立驗證。

## 授權

本儲存庫的整理內容和程式碼：[MIT](LICENSE)。連結的專案保留各自的授權。
