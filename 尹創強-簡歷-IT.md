# 尹創強 — 個人簡歷（詳細版）

**求職意向：運維開發工程師 / IT 基礎設施負責人 | 深圳 | 全職**

📞 18681121363 | 📧 ikeee@qq.com | 🔗 [github.com/ikeee](https://github.com/ikeee)

---

## 個人優勢

- 8 年 IT 運維實戰（3 年政企批量部署 + 5 年學校資訊化獨立操盤），能一人撐起整個 IT 部門
- 2024–2026 年深度使用 AI 編程工具（Claude Code），獨立完成 10+ 個全棧項目，覆蓋 Python / TypeScript / Rust / Docker
- 擅長用開源工具零成本搭建企業級系統——13 個項目中 10 個為自建方案
- 15 年創業經驗（1997–2008），懂成本控制、需求優先級、用戶視角

---

## 工作經歷

### 深圳大學附屬教育集團外國語中學 · 資訊化負責人（2020.09 – 至今）

獨立負責全校 IT 基礎設施的規劃、建設與運維。從零開始，一人完成需求調研 → 選型部署 → 日常運維 → 用戶培訓的全鏈路。

**職責範圍：**
- 全校電腦、網絡、多媒體設備的規劃、採購、部署與維護
- 校園內網架構設計與安全策略（所有系統自建在內網，數據不出校門）
- 教師 IT 培訓與日常技術支援
- 開源方案選型與落地，零商業軟件採購

**主要成果：**

| 類別 | 系統 | 技術方案 | 說明 |
|------|------|---------|------|
| 教學 | Teacher-Folder 課件同步 | Shell + rsync + NAS SMB | 教師端推送→NAS 存儲→班級終端自動拉取。Win/Mac 雙平台，2 年穩定運行 |
| 教學 | PPT-Resource-Hub | 靜態站點 + GitHub 託管 | 課件資源共享平台，教師上傳模板和教案互相借鑒 |
| 教學 | MediaCMS 視頻 Hub | Django + Docker + HLS | 公開課視頻平台，支援上傳、分類、點播，內網頻寬免費 |
| 辦公 | 校園門戶導航 | 純靜態 HTML + Nginx | 全校師生每日第一屏，統一入口、歸類清晰 |
| 辦公 | MkDocs 資訊化手冊 | Python MkDocs + Git | IT 知識文檔化，教師自助查詢，降低運維諮詢量 |
| 辦公 | Wiki.js 設備指南 | Node.js + Wiki.js | 每間教室設備型號、使用步驟、故障排查，圖文 Wiki |
| 通訊 | Jitsi Meet 視頻會議 | Java/JS + WebRTC | 自建視頻會議，內網部署無用戶數限制，隱私保護 |
| 通訊 | Owncast 直播系統 | Go + RTMP/HLS | 運動會、文藝匯演、家長會一鍵推流 |
| 宣傳 | Memos 校園動態 | Go + SQLite | 輕量圖文發布平台，比公眾號更輕便 |
| 宣傳 | 奇安信壁紙推送 | 天擎 V10 原生策略 | 通知/海報直達教室大屏，全校覆蓋零額外開發 |
| 互動 | Photos-Wall-3D 體感牆 | MediaPipe Pose + Three.js | 架空層 LED 大屏互動，33 個骨骼關鍵點實時識別，純前端方案 |

---

### 中科創威 · IT 運維工程師（2017.03 – 2020.07）

負責政企客戶的桌面環境批量部署與伺服器日常運維。

- Windows/Linux 雙平台系統安裝、軟件分發、標準化配置模板
- 伺服器日常巡檢、故障排查、系統更新與補丁管理
- 將運維操作文檔化、流程化，形成可複用的 SOP 體系

**積累的能力：** 工程化思維——標準化、文檔化、可複製。從「管一台機器」到「管一批機器」的認知升級。

---

### 自主創業 · 網吧連鎖（1997 – 2008）

從 1 家起步擴展至 6 家連鎖，全週期獨立操盤。

- **選址**：人流分析、競品調研、租金談判
- **網絡部署**：從百兆到千兆的網絡架構規劃，伺服器搭建，計費系統選型與維護
- **運營**：高峰期排隊管理、機器故障快速回應、會員留存策略
- **退出**：2008 年家用寬頻普及、行業結構下行前，完成資產出售主動離場

**積累的能力：** 系統不是技術問題，是人的問題。選址比機器配置重要，運營比技術架構重要，用戶體驗比功能列表重要。

---

## 項目詳情

### 一、AI 驅動的工作流自動化（2026.03 – 至今）

利用 Claude Code 等 AI 編程工具獨立構建的開發與運維體系。

#### 1. 教案自動生成引擎

**技術棧：** Python · LLM（多 Provider） · Qdrant 向量數據庫 · BGE-large-zh · Prompt Engineering

**功能：**
- 10 模塊結構化教案自動生成：教學目標 → 教材分析 → 學情分析 → 重難點 → 教學方法 → 教學活動 → 教學流程 → 作業設計 → 板書設計 → 教學反思
- 覆蓋語文、數學、英語、物理、化學、生物 6 個學科
- 文理分科策略：理科走「實驗→觀察→歸納→公式→應用」，文科走「情境→研讀→梳理→追問→共鳴→表達」
- Qdrant + BGE-large-zh 向量化教材原文，教案中精準引用課標條目
- 50+ 條自動化質檢規則（結構完整性、術語規範性、字數達標、課標引用準確性）
- A/B/C/D 四級評分體系，A/B 級通過率 90%+

**量化成果：** 備課時間從 2 小時 → 5 分鐘

#### 2. 互動課件系統（open-slide）

**技術棧：** React · TypeScript · Vite · PptxGenJS · Remotion · CSS Animations

**功能：**
- 11 種可複用佈局組件（卡片式、分欄式、步驟式、對比式等），按教案內容選擇佈局直接填入
- 已交付 12 課時：數學（二次函數 6 課時，含 Remotion 投籃軌跡物理模擬視頻）、英語（body-language 3 課時、unknown-world 3 課時）
- 教案編輯器：瀏覽器內 Markdown 編輯（端口 5174），教師無需接觸代碼
- 教案 → 結構化標籤解析 → PptxGenJS 自動渲染 PPT → Nginx 託管交付

**自研工具：**
- slide-review.py：自動掃描 TSX 源碼檢測 5 類問題（過時 API 引用、未閉合標籤、缺失 export、無效 import、樣式語法錯誤）
- 驗收清單：JSX 無報錯 → 所有鏈接 200 OK → 移動端響應式 → 教案-課件內容一一對應

**Remotion 投籃軌跡視頻：**
- 用 Remotion（React 視頻框架）編寫拋物線投籃物理模擬動畫
- 參數可調（初速度 / 角度 / 重力加速度）
- 嵌入 math-ch2 二次函數課件，與知識點一一對應
- 渲染管線可在伺服器端自動化執行

#### 3. Multi-Agent 協作架構

**技術棧：** Python · MQTT (Mosquitto) · SSE · cron · HTTP API

**架構設計：**
- 三通道通信基礎設施：MQTT 群聊（日常溝通）+ Shared Brain 知識中樞（:8080，廣播/私語/SSE 實時推送）+ HTTP API（任務派發）
- LWT（Last Will Testament）遺囑消息實現 Agent 在線/離線自動檢測
- cron 調度：每日打卡、交叉閱讀提醒、知識庫健康檢查全自動化
- Agent 恢復 SOP：離線時一鍵診斷 + 重啟

**設計原則：**
- 三角分工模型：架構與全棧開發 + 前端與課件渲染 + 研究與文檔撰寫，各司其職
- 各角色使用獨立上下文產出，確保真實差異性
- 每日 10:00 自動交叉閱讀隊友筆記，形成知識閉環

#### 4. 微服務集群

**技術棧：** Docker Compose · Nginx · 1Panel · SSH · iptables

**服務矩陣：**

| 服務 | 端口 | 用途 |
|------|------|------|
| OpenClaw (Nova) | :18789 | 課件開發 |
| QwenPaw (Qwen) | :8088 | 研究分析 |
| Shared Brain | :8080 | 知識中樞（廣播/私語/SSE） |
| Mosquitto | :1883 | MQTT 群聊 broker |
| OpenResty | :80 | 靜態資源分發 |
| Memos | :5230 | 筆記發布 |

**運維原則：**
- 單機（192.168.30.97）編排全部 6+ 容器
- 全部服務通過 Nginx 反向代理暴露，零 Docker 端口直接暴露
- SSH + base64 pipe 自建部署管線，不依賴 GitHub Actions 或外部 CI/CD

#### 5. Encyclopedia 知識庫

**技術棧：** 純靜態 HTML/CSS/JavaScript · Design Token 體系

**功能：**
- 19KB / 693 行純前端首頁，無框架依賴
- 雙索引自動同步（index.json + notes-index.json）
- knowledge-lint.py 定時掃描 404 與格式異常
- 暖米白紙色（#f5f2ed） + 赭石單色（#b45309）Design Token，克制即高級
- 純文字筆記列表（無 emoji / tags / star / 摘要），左側豎線標記選中態

#### 6. 電商運營調研

**時間：** 2026.06.05 | **耗時：** 45 分鐘完成從指令到報告交付

**背景：** 調研開源項目後，決策從「開發自動化工具」轉向「用平台現有 AI 工具做運營」，節省至少 2 週開發週期。

**產出：**
- 五階段自動閉環 SOP：AI大數據選詞 → AI人群建模 → AI勝率選款 → 自動化上架+測款 → 流量放大+風控
- 每階段含量化門檻：搜索量>1000/天、毛利>35%、CTR<2%淘汰、投產比<1.5停投
- 三條品類文案模板（家居收納 / 寵物用品 / 廚房小工具）
- 同步 6 路搜索交叉驗證，多源數據融合

#### 7. 備課設計原則方法論

**產出：** 從 Anthropic 設計哲學推導出四大產品設計原則——

1. **克制**：減少認知負荷，每個功能必須有存在理由
2. **調性先於功能**：先定美學基調，再決定做什麼功能
3. **每個組件有存在理由**：可刪性測試，刪不掉才保留
4. **輸出有跡可循**：每份教案可追溯課標依據和設計意圖

**寫作方法：** 「先定調再動筆」——花 30 秒確定一個核心比喻，全文圍繞它展開。實踐成果：定調「備課產品不是工具，是課堂的建築師」。

---

### 二、開源項目貢獻

#### OpenMAIC — 清華大學 AI 互動課堂
- 發表：JCST 2026（Journal of Computer Science and Technology）
- Stars：1.5k+
- 個人貢獻：77 個 commits，3 個 PR 合入（#2 Vercel 部署 / #3 MinerU 文檔解析 / #4 OpenClaw 集成），提交 13+ 個 Issues
- Bug 修復亮點：發現 Qwen ASR 語音識別關鍵 Bug——瀏覽器 MediaRecorder 生成 WebM 音頻，但 API 請求聲明為 WAV，MIME 類型不匹配導致音頻解碼失敗，始終返回「嗯。」。改兩行代碼修復（Fixes #76）
- 測試：搭建 Vitest 測試框架，編寫 139 個單元測試，編寫 Action Parser 完整測試套件
- 其他修復：TTS 長語音拼接異常、Agent 持久化丟失、Tavily 搜索 400 字符截斷、Prompt 洩露教師身份到課件、Turbopack 構建兼容、React Compiler 衝突

**技術棧：** Next.js 16 · TypeScript · LangGraph · Multi-Agent · Vitest

#### 花箋 Floral Notepaper — Tauri 2 + React 19 + Rust 桌面便簽
- DeepSeek API 翻譯引擎升級，替換原有不穩定的免費翻譯 API
- 中英雙向翻譯：粘貼英文自動翻中文，粘貼中文自動翻英文
- 粘貼自動翻譯 + 生詞本功能
- 聚焦 Windows 平台，精簡 ~700 行代碼（移除 macOS/Linux 支援）
- 修復自動儲存期間打字導致內容丟失和光標跳動的併發競態 bug
- 修復視窗主題切換閃白屏問題
- CI/CD 發布流程優化，編寫 Release Note 與環境配置文檔

**技術棧：** Tauri 2 · Rust · React 19 · TypeScript · DeepSeek API

#### 個人開源項目
- **Teacher-Folder**：課件自動同步系統（Shell + rsync + NAS，GitHub 開源）
- **Photos-Wall-3D**：體感互動牆（MediaPipe Pose + Three.js，GitHub 開源）
- **PPT-Resource-Hub**：課件資源共享平台

---

## 技能

| 類別 | 具體技能 |
|------|---------|
| 編程語言 | Python · TypeScript · Rust · Shell（Bash / PowerShell） |
| 前端 | React · Next.js · Vite · HTML5 Canvas · Three.js |
| 後端 / AI | Qdrant (RAG) · LangGraph · MQTT · REST API · Prompt Engineering · LLM 多 Provider 架構 |
| 運維 / 基礎設施 | Docker Compose · Nginx 反向代理 · SSH 部署 · iptables · 群暉 NAS · OpenWrt · 1Panel |
| 工具鏈 | Git · GitHub Actions · Linux (Debian/Ubuntu) · Windows Server |

---

## 教育背景

- 高中學歷（寮步中學高中部）
- 持續自學：通過實際項目驅動學習，近兩年系統實踐了 Rust、TypeScript、Docker、LLM 應用開發等技術棧

---

## 附加資訊

- **語言**：中文（粵語、普通話），英文（可閱讀技術文檔，借助 AI 工具寫作）
- **GitHub**：[github.com/ikeee](https://github.com/ikeee)
- **在線簡歷**：[ikeee.github.io/A1Q2/resume.html](https://ikeee.github.io/A1Q2/resume.html)
- **所在城市**：東莞
