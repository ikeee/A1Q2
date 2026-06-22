# 尹创强 — 个人简历（详细版）

**求职意向：运维开发工程师 / IT 基础设施负责人 | 深圳 | 全职**

📞 18681121363 | 📧 ikeee@qq.com | 🔗 [github.com/ikeee](https://github.com/ikeee)

---

## 个人优势

- 8 年 IT 运维实战（3 年政企批量部署 + 5 年学校信息化独立操盘），能一人撑起整个 IT 部门
- 2024–2026 年深度使用 AI 编程工具（Claude Code），独立完成 10+ 个全栈项目，覆盖 Python / TypeScript / Rust / Docker
- 擅长用开源工具零成本搭建企业级系统——13 个项目中 10 个为自建方案
- 15 年创业经验（1997–2008），懂成本控制、需求优先级、用户视角

---

## 工作经历

### 深圳大学附属教育集团外国语中学 · 信息化负责人（2020.09 – 至今）

独立负责全校 IT 基础设施的规划、建设与运维。从零开始，一人完成需求调研 → 选型部署 → 日常运维 → 用户培训的全链路。

**职责范围：**
- 全校计算机、网络、多媒体设备的规划、采购、部署与维护
- 校园内网架构设计与安全策略（所有系统自建在内网，数据不出校门）
- 教师 IT 培训与日常技术支持
- 开源方案选型与落地，零商业软件采购

**主要成果：**

| 类别 | 系统 | 技术方案 | 说明 |
|------|------|---------|------|
| 教学 | Teacher-Folder 课件同步 | Shell + rsync + NAS SMB | 教师端推送→NAS 存储→班级终端自动拉取。Win/Mac 双平台，2 年稳定运行 |
| 教学 | PPT-Resource-Hub | 静态站点 + GitHub 托管 | 课件资源共享平台，教师上传模板和教案互相借鉴 |
| 教学 | MediaCMS 视频 Hub | Django + Docker + HLS | 公开课视频平台，支持上传、分类、点播，内网带宽免费 |
| 办公 | 校园门户导航 | 纯静态 HTML + Nginx | 全校师生每日第一屏，统一入口、归类清晰 |
| 办公 | MkDocs 信息化手册 | Python MkDocs + Git | IT 知识文档化，教师自助查询，降低运维咨询量 |
| 办公 | Wiki.js 设备指南 | Node.js + Wiki.js | 每间教室设备型号、使用步骤、故障排查，图文 Wiki |
| 通讯 | Jitsi Meet 视频会议 | Java/JS + WebRTC | 自建视频会议，内网部署无用户数限制，隐私保护 |
| 通讯 | Owncast 直播系统 | Go + RTMP/HLS | 运动会、文艺汇演、家长会一键推流 |
| 宣传 | Memos 校园动态 | Go + SQLite | 轻量图文发布平台，比公众号更轻便 |
| 宣传 | 奇安信壁纸推送 | 天擎 V10 原生策略 | 通知/海报直达教室大屏，全校覆盖零额外开发 |
| 互动 | Photos-Wall-3D 体感墙 | MediaPipe Pose + Three.js | 架空层 LED 大屏互动，33 个骨骼关键点实时识别，纯前端方案 |

---

### 中科创威 · IT 运维工程师（2017.03 – 2020.07）

负责政企客户的桌面环境批量部署与服务器日常运维。

- Windows/Linux 双平台系统安装、软件分发、标准化配置模板
- 服务器日常巡检、故障排查、系统更新与补丁管理
- 将运维操作文档化、流程化，形成可复用的 SOP 体系

**积累的能力：** 工程化思维——标准化、文档化、可复制。从"管一台机器"到"管一批机器"的认知升级。

---

### 自主创业 · 网吧连锁（1997 – 2008）

从 1 家起步扩展至 6 家连锁，全周期独立操盘。

- **选址**：人流分析、竞品调研、租金谈判
- **网络部署**：从百兆到千兆的网络架构规划，服务器搭建，计费系统选型与维护
- **运营**：高峰期排队管理、机器故障快速响应、会员留存策略
- **退出**：2008 年家用宽带普及、行业结构下行前，完成资产出售主动离场

**积累的能力：** 系统不是技术问题，是人的问题。选址比机器配置重要，运营比技术架构重要，用户体验比功能列表重要。

---

## 项目详情

### 一、AI 驱动的工作流自动化（2026.03 – 至今）

利用 Claude Code 等 AI 编程工具独立构建的开发与运维体系。

#### 1. 教案自动生成引擎

**技术栈：** Python · LLM（多 Provider） · Qdrant 向量数据库 · BGE-large-zh · Prompt Engineering

**功能：**
- 10 模块结构化教案自动生成：教学目标 → 教材分析 → 学情分析 → 重难点 → 教学方法 → 教学活动 → 教学流程 → 作业设计 → 板书设计 → 教学反思
- 覆盖语文、数学、英语、物理、化学、生物 6 个学科
- 文理分科策略：理科走"实验→观察→归纳→公式→应用"，文科走"情境→研读→梳理→追问→共鸣→表达"
- Qdrant + BGE-large-zh 向量化教材原文，教案中精准引用课标条目
- 50+ 条自动化质检规则（结构完整性、术语规范性、字数达标、课标引用准确性）
- A/B/C/D 四级评分体系，A/B 级通过率 90%+

**量化成果：** 备课时间从 2 小时 → 5 分钟

#### 2. 互动课件系统（open-slide）

**技术栈：** React · TypeScript · Vite · PptxGenJS · Remotion · CSS Animations

**功能：**
- 11 种可复用布局组件（卡片式、分栏式、步骤式、对比式等），按教案内容选择布局直接填入
- 已交付 12 课时：数学（二次函数 6 课时，含 Remotion 投篮轨迹物理模拟视频）、英语（body-language 3 课时、unknown-world 3 课时）
- 教案编辑器：浏览器内 Markdown 编辑（端口 5174），教师无需接触代码
- 教案 → 结构化标签解析 → PptxGenJS 自动渲染 PPT → Nginx 托管交付

**自研工具：**
- slide-review.py：自动扫描 TSX 源码检测 5 类问题（过时 API 引用、未闭合标签、缺失 export、无效 import、样式语法错误）
- 验收清单：JSX 无报错 → 所有链接 200 OK → 移动端响应式 → 教案-课件内容一一对应

**Remotion 投篮轨迹视频：**
- 用 Remotion（React 视频框架）编写抛物线投篮物理模拟动画
- 参数可调（初速度 / 角度 / 重力加速度）
- 嵌入 math-ch2 二次函数课件，与知识点一一对应
- 渲染管线可在服务器端自动化执行

#### 3. Multi-Agent 协作架构

**技术栈：** Python · MQTT (Mosquitto) · SSE · cron · HTTP API

**架构设计：**
- 三通道通信基础设施：MQTT 群聊（日常沟通）+ Shared Brain 知识中枢（:8080，广播/私语/SSE 实时推送）+ HTTP API（任务派发）
- LWT（Last Will Testament）遗嘱消息实现 Agent 在线/离线自动检测
- cron 调度：每日打卡、交叉阅读提醒、知识库健康检查全自动化
- Agent 恢复 SOP：离线时一键诊断 + 重启

**设计原则：**
- 三角分工模型：架构与全栈开发 + 前端与课件渲染 + 研究与文档撰写，各司其职
- 各角色使用独立上下文产出，确保真实差异性
- 每日 10:00 自动交叉阅读队友笔记，形成知识闭环

#### 4. 微服务集群

**技术栈：** Docker Compose · Nginx · 1Panel · SSH · iptables

**服务矩阵：**

| 服务 | 端口 | 用途 |
|------|------|------|
| OpenClaw (Nova) | :18789 | 课件开发 |
| QwenPaw (Qwen) | :8088 | 研究分析 |
| Shared Brain | :8080 | 知识中枢（广播/私语/SSE） |
| Mosquitto | :1883 | MQTT 群聊 broker |
| OpenResty | :80 | 静态资源分发 |
| Memos | :5230 | 笔记发布 |

**运维原则：**
- 单机（192.168.30.97）编排全部 6+ 容器
- 全部服务通过 Nginx 反向代理暴露，零 Docker 端口直接暴露
- SSH + base64 pipe 自建部署管线，不依赖 GitHub Actions 或外部 CI/CD

#### 5. Encyclopedia 知识库

**技术栈：** 纯静态 HTML/CSS/JavaScript · Design Token 体系

**功能：**
- 19KB / 693 行纯前端首页，无框架依赖
- 双索引自动同步（index.json + notes-index.json）
- knowledge-lint.py 定时扫描 404 与格式异常
- 暖米白纸色（#f5f2ed） + 赭石单色（#b45309）Design Token，克制即高级
- 纯文字笔记列表（无 emoji / tags / star / 摘要），左侧竖线标记选中态

#### 6. 电商运营调研

**时间：** 2026.06.05 | **耗时：** 45 分钟完成从指令到报告交付

**背景：** 调研开源项目后，决策从"开发自动化工具"转向"用平台现有 AI 工具做运营"，节省至少 2 周开发周期。

**产出：**
- 五阶段自动闭环 SOP：AI大数据选词 → AI人群建模 → AI胜率选款 → 自动化上架+测款 → 流量放大+风控
- 每阶段含量化门槛：搜索量>1000/天、毛利>35%、CTR<2%淘汰、投产比<1.5停投
- 三条品类文案模板（家居收纳 / 宠物用品 / 厨房小工具）
- 同步 6 路搜索交叉验证，多源数据融合

#### 7. 备课设计原则方法论

**产出：** 从 Anthropic 设计哲学推导出四大产品设计原则——

1. **克制**：减少认知负荷，每个功能必须有存在理由
2. **调性先于功能**：先定美学基调，再决定做什么功能
3. **每个组件有存在理由**：可删性测试，删不掉才保留
4. **输出有迹可循**：每份教案可追溯课标依据和设计意图

**写作方法：** "先定调再动笔"——花 30 秒确定一个核心比喻，全文围绕它展开。实践成果：定调"备课产品不是工具，是课堂的建筑师"。

---

### 二、开源项目贡献

#### OpenMAIC — 清华大学 AI 互动课堂
- 发表：JCST 2026（Journal of Computer Science and Technology）
- Stars：1.5k+
- 个人贡献：77 个 commits，3 个 PR 合入（#2 Vercel 部署 / #3 MinerU 文档解析 / #4 OpenClaw 集成），提交 13+ 个 Issues
- Bug 修复亮点：发现 Qwen ASR 语音识别关键 Bug——浏览器 MediaRecorder 生成 WebM 音频，但 API 请求声明为 WAV，MIME 类型不匹配导致音频解码失败，始终返回"嗯。"。改两行代码修复（Fixes #76）
- 测试：搭建 Vitest 测试框架，编写 139 个单元测试，编写 Action Parser 完整测试套件
- 其他修复：TTS 长语音拼接异常、Agent 持久化丢失、Tavily 搜索 400 字符截断、Prompt 泄露教师身份到课件、Turbopack 构建兼容、React Compiler 冲突

**技术栈：** Next.js 16 · TypeScript · LangGraph · Multi-Agent · Vitest

#### 花笺 Floral Notepaper — Tauri 2 + React 19 + Rust 桌面便签
- DeepSeek API 翻译引擎升级，替换原有不稳定的免费翻译 API
- 中英双向翻译：粘贴英文自动翻中文，粘贴中文自动翻英文
- 粘贴自动翻译 + 生词本功能
- 聚焦 Windows 平台，精简 ~700 行代码（移除 macOS/Linux 支持）
- 修复自动保存期间打字导致内容丢失和光标跳动的并发竞态 bug
- 修复窗口主题切换闪白屏问题
- CI/CD 发布流程优化，编写 Release Note 与环境配置文档

**技术栈：** Tauri 2 · Rust · React 19 · TypeScript · DeepSeek API

#### 个人开源项目
- **Teacher-Folder**：课件自动同步系统（Shell + rsync + NAS，GitHub 开源）
- **Photos-Wall-3D**：体感互动墙（MediaPipe Pose + Three.js，GitHub 开源）
- **PPT-Resource-Hub**：课件资源共享平台

---

## 技能

| 类别 | 具体技能 |
|------|---------|
| 编程语言 | Python · TypeScript · Rust · Shell（Bash / PowerShell） |
| 前端 | React · Next.js · Vite · HTML5 Canvas · Three.js |
| 后端 / AI | Qdrant (RAG) · LangGraph · MQTT · REST API · Prompt Engineering · LLM 多 Provider 架构 |
| 运维 / 基础设施 | Docker Compose · Nginx 反向代理 · SSH 部署 · iptables · 群晖 NAS · OpenWrt · 1Panel |
| 工具链 | Git · GitHub Actions · Linux (Debian/Ubuntu) · Windows Server |

---

## 教育背景

- 高中学历（寮步中学高中部）
- 持续自学：通过实际项目驱动学习，近两年系统实践了 Rust、TypeScript、Docker、LLM 应用开发等技术栈

---

## 附加信息

- **语言**：中文（粤语、普通话），英文（可阅读技术文档，借助 AI 工具写作）
- **GitHub**：[github.com/ikeee](https://github.com/ikeee)
- **在线简历**：[ikeee.github.io/A1Q2/resume.html](https://ikeee.github.io/A1Q2/resume.html)
- **所在城市**：东莞
