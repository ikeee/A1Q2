# Yin Chuangqiang — Resume (Detailed Version)

**Job Target: DevOps Engineer / IT Infrastructure Lead | Shenzhen | Full-time**

📞 18681121363 | 📧 ikeee@qq.com | 🔗 [github.com/ikeee](https://github.com/ikeee)

---

## Personal Strengths

- 8 years of hands-on IT operations (3 years of government/enterprise batch deployment + 5 years of independent K-12 school IT management), capable of single-handedly running an entire IT department
- 2024–2026: Deep use of AI programming tools (Claude Code), independently completed 10+ full-stack projects covering Python / TypeScript / Rust / Docker
- Skilled at building enterprise-grade systems with open-source tools at zero cost — 10 out of 13 projects are self-built solutions
- 15 years of entrepreneurial experience (1997–2008), with a solid grasp of cost control, requirement prioritization, and user perspective

---

## Work Experience

### Shenzhen University Affiliated Education Group Foreign Language Junior High School · IT Director (2020.09 – Present)

Independently responsible for the planning, construction, and operation of the entire school's IT infrastructure. Starting from scratch, single-handedly completed the full chain of requirements research → vendor selection & deployment → daily operations → user training.

**Scope of Responsibilities:**
- Planning, procurement, deployment, and maintenance of all school computers, networks, and multimedia equipment
- Campus intranet architecture design and security policy (all systems are self-hosted on the intranet; data never leaves the campus)
- Teacher IT training and daily technical support
- Open-source solution evaluation and implementation, with zero commercial software procurement

**Key Achievements:**

| Category | System | Tech Stack | Description |
|------|------|---------|------|
| Teaching | Teacher-Folder Courseware Sync | Shell + rsync + NAS SMB | Teacher-side push → NAS storage → classroom terminal auto-pull. Dual-platform Win/Mac, stable operation for 2 years |
| Teaching | PPT-Resource-Hub | Static site + GitHub hosting | Courseware resource sharing platform; teachers upload templates and lesson plans for mutual reference |
| Teaching | MediaCMS Video Hub | Django + Docker + HLS | Open class video platform supporting upload, categorization, and on-demand streaming; intranet bandwidth at zero cost |
| Administration | Campus Portal Navigation | Pure static HTML + Nginx | The daily first screen for all faculty and students; unified entry point with clear categorization |
| Administration | MkDocs IT Handbook | Python MkDocs + Git | IT knowledge documented for teacher self-service lookup, reducing operational support volume |
| Administration | Wiki.js Equipment Guide | Node.js + Wiki.js | Per-classroom equipment model, usage steps, and troubleshooting, in an illustrated Wiki |
| Communication | Jitsi Meet Video Conferencing | Java/JS + WebRTC | Self-hosted video conferencing, intranet deployment with no user limit, privacy protected |
| Communication | Owncast Live Streaming | Go + RTMP/HLS | One-click push streaming for sports meets, art performances, and parent meetings |
| Publicity | Memos Campus Updates | Go + SQLite | Lightweight text-and-image publishing platform, more agile than an official WeChat account |
| Publicity | Qi-An-Xin Wallpaper Push | TianQing V10 native policy | Notices/posters delivered directly to classroom large screens, full campus coverage with zero extra development |
| Interactive | Photos-Wall-3D Motion-Sensing Wall | MediaPipe Pose + Three.js | Elevated-floor LED large-screen interaction, 33 skeletal keypoints real-time recognition, pure frontend solution |

---

### Zhongke Chuangwei · IT Operations Engineer (2017.03 – 2020.07)

Responsible for batch desktop environment deployment and routine server operations for government and enterprise clients.

- Windows/Linux dual-platform system installation, software distribution, standardized configuration templates
- Routine server inspection, fault diagnosis, system updates, and patch management
- Documented and proceduralized operational tasks, forming a reusable SOP system

**Capability Gained:** Engineering mindset — standardization, documentation, replicability. A cognitive upgrade from "managing one machine" to "managing a fleet of machines."

---

### Self-Employed · Internet Cafe Chain (1997 – 2008)

Started from a single location and expanded to a chain of 6, independently managing the full lifecycle.

- **Site Selection:** Foot traffic analysis, competitive research, lease negotiation
- **Network Deployment:** Network architecture planning from 100 Mbps to Gigabit, server setup, billing system selection and maintenance
- **Operations:** Peak-hour queue management, rapid machine failure response, member retention strategy
- **Exit:** In 2008, before widespread home broadband adoption and industry structural decline, completed asset sale and proactively exited the market

**Capability Gained:** Systems are not a technology problem — they are a people problem. Site selection matters more than machine specs, operations matter more than technical architecture, and user experience matters more than feature lists.

---

## Project Details

### I. AI-Driven Workflow Automation (2026.03 – Present)

A development and operations system independently built using AI programming tools such as Claude Code.

#### 1. Automated Lesson Plan Generation Engine

**Tech Stack:** Python · LLM (Multi-Provider) · Qdrant Vector Database · BGE-large-zh · Prompt Engineering

**Features:**
- 10-module structured lesson plan auto-generation: Teaching Objectives → Textbook Analysis → Student Analysis → Key & Difficult Points → Teaching Methods → Teaching Activities → Teaching Flow → Homework Design → Board Writing Design → Teaching Reflection
- Covers 6 subjects: Chinese, Math, English, Physics, Chemistry, Biology
- Discipline-specific strategies: Sciences follow "Experiment → Observation → Induction → Formula → Application"; Humanities follow "Context → Close Reading → Sorting → Questioning → Resonance → Expression"
- Qdrant + BGE-large-zh vectorization of textbook source texts, with precise curriculum standard citations in lesson plans
- 50+ automated quality-check rules (structural completeness, terminology standards, word count compliance, curriculum standard citation accuracy)
- A/B/C/D four-tier scoring system, with A/B pass rate at 90%+

**Quantified Result:** Lesson preparation time reduced from 2 hours → 5 minutes

#### 2. Interactive Courseware System (open-slide)

**Tech Stack:** React · TypeScript · Vite · PptxGenJS · Remotion · CSS Animations

**Features:**
- 11 reusable layout components (Card, Column, Step-by-Step, Comparison, etc.), select layout by lesson plan content and populate directly
- 12 class sessions delivered: Math (Quadratic Functions, 6 sessions, including Remotion basketball shot trajectory physics simulation video), English (Body Language, 3 sessions; Unknown World, 3 sessions)
- Lesson Plan Editor: In-browser Markdown editing (port 5174), teachers never touch code
- Lesson Plan → Structured tag parsing → PptxGenJS auto-rendering PPT → Nginx hosted delivery

**Self-Built Tools:**
- slide-review.py: Auto-scans TSX source code to detect 5 types of issues (deprecated API references, unclosed tags, missing exports, invalid imports, style syntax errors)
- Acceptance Checklist: No JSX errors → All links 200 OK → Mobile responsive → Lesson plan and courseware content one-to-one correspondence

**Remotion Basketball Shot Trajectory Video:**
- Built a parabolic basketball shot physics simulation animation using Remotion (React video framework)
- Adjustable parameters (initial velocity / angle / gravitational acceleration)
- Embedded in the Math CH2 Quadratic Functions courseware, one-to-one correspondence with knowledge points
- Rendering pipeline can be executed automatically on the server side

#### 3. Multi-Agent Collaboration Architecture

**Tech Stack:** Python · MQTT (Mosquitto) · SSE · cron · HTTP API

**Architecture Design:**
- Three-channel communication infrastructure: MQTT group chat (daily communication) + Shared Brain knowledge hub (:8080, broadcast/whisper/SSE real-time push) + HTTP API (task dispatch)
- LWT (Last Will Testament) messages for automatic Agent online/offline detection
- cron scheduling: Daily check-in, cross-reading reminders, knowledge base health checks — fully automated
- Agent Recovery SOP: One-click diagnosis + restart when offline

**Design Principles:**
- Triangular division of labor model: Architecture & Full-Stack Development + Frontend & Courseware Rendering + Research & Documentation Writing, each with clear responsibilities
- Each role produces output using independent context, ensuring genuine differentiation
- Daily 10:00 AM automatic cross-reading of teammates' notes, forming a knowledge closed loop

#### 4. Microservice Cluster

**Tech Stack:** Docker Compose · Nginx · 1Panel · SSH · iptables

**Service Matrix:**

| Service | Port | Purpose |
|------|------|------|
| OpenClaw (Nova) | :18789 | Courseware development |
| QwenPaw (Qwen) | :8088 | Research & analysis |
| Shared Brain | :8080 | Knowledge hub (broadcast/whisper/SSE) |
| Mosquitto | :1883 | MQTT group chat broker |
| OpenResty | :80 | Static asset distribution |
| Memos | :5230 | Note publishing |

**Operations Principles:**
- Single machine (192.168.30.97) orchestrating all 6+ containers
- All services exposed via Nginx reverse proxy, zero direct Docker port exposure
- SSH + base64 pipe self-built deployment pipeline, no dependency on GitHub Actions or external CI/CD

#### 5. Encyclopedia Knowledge Base

**Tech Stack:** Pure static HTML/CSS/JavaScript · Design Token System

**Features:**
- 19 KB / 693 lines pure frontend homepage, zero framework dependencies
- Dual-index auto-sync (index.json + notes-index.json)
- knowledge-lint.py scheduled scanning for 404 errors and format anomalies
- Warm cream paper tone (#f5f2ed) + Ochre monochrome (#b45309) Design Token — restraint as sophistication
- Plain-text note list (no emoji / tags / stars / summaries), left-side vertical bar marking selected state

#### 6. E-Commerce Operations Research

**Date:** 2026.06.05 | **Time Spent:** 45 minutes from prompt to report delivery

**Background:** After researching open-source projects, pivoted from "developing automation tools" to "using the platform's existing AI tools for operations," saving at least 2 weeks of development time.

**Deliverables:**
- Five-stage automated closed-loop SOP: AI Big Data Keyword Selection → AI Audience Modeling → AI Win-Rate Product Selection → Automated Listing + Testing → Traffic Amplification + Risk Control
- Each stage includes quantified thresholds: Search Volume > 1,000/day, Gross Margin > 35%, CTR < 2% eliminated, ROI < 1.5 paused
- Three category copywriting templates (Home Storage / Pet Supplies / Kitchen Gadgets)
- Simultaneous 6-channel search cross-validation, multi-source data fusion

#### 7. Lesson Plan Design Principles Methodology

**Deliverable:** Derived four major product design principles from Anthropic's design philosophy —

1. **Restraint:** Reduce cognitive load; every feature must have a reason to exist
2. **Tone Before Function:** Define the aesthetic tone first, then decide what features to build
3. **Every Component Has a Reason to Exist:** Deletability test — keep only what cannot be deleted
4. **Traceable Output:** Every lesson plan can be traced back to curriculum standard basis and design intent

**Writing Method:** "Set the tone before you write" — spend 30 seconds determining a core metaphor and build the entire text around it. Practical result: Set the tone as "A lesson planning product is not a tool — it is the architect of the classroom."

---

### II. Open Source Project Contributions

#### OpenMAIC — Tsinghua University AI Interactive Classroom
- Published: JCST 2026 (Journal of Computer Science and Technology)
- Stars: 1.5k+
- Personal Contributions: 77 commits, 3 PRs merged (#2 Vercel Deployment / #3 MinerU Document Parsing / #4 OpenClaw Integration), submitted 13+ Issues
- Bug Fix Highlight: Discovered a critical Qwen ASR voice recognition bug — browser MediaRecorder generated WebM audio, but the API request declared WAV format; MIME type mismatch caused audio decoding failure, consistently returning only "Hmm." Fixed with a two-line code change (Fixes #76)
- Testing: Set up Vitest testing framework, wrote 139 unit tests, authored a complete Action Parser test suite
- Other Fixes: TTS long-speech concatenation anomaly, Agent persistence loss, Tavily search 400-character truncation, Prompt leaking teacher identity into courseware, Turbopack build compatibility, React Compiler conflict

**Tech Stack:** Next.js 16 · TypeScript · LangGraph · Multi-Agent · Vitest

#### Floral Notepaper (花笺) — Tauri 2 + React 19 + Rust Desktop Sticky Notes
- Upgraded the translation engine to DeepSeek API, replacing the previously unstable free translation API
- Chinese-English bidirectional translation: paste English auto-translates to Chinese, paste Chinese auto-translates to English
- Paste-to-auto-translate + vocabulary notebook feature
- Focused on Windows platform, trimmed ~700 lines of code (removed macOS/Linux support)
- Fixed a concurrency race-condition bug where typing during auto-save caused content loss and cursor jumping
- Fixed window theme switching white flash issue
- Optimized CI/CD release workflow, authored Release Notes and environment setup documentation

**Tech Stack:** Tauri 2 · Rust · React 19 · TypeScript · DeepSeek API

#### Personal Open Source Projects
- **Teacher-Folder**: Courseware auto-sync system (Shell + rsync + NAS, open-sourced on GitHub)
- **Photos-Wall-3D**: Motion-sensing interactive wall (MediaPipe Pose + Three.js, open-sourced on GitHub)
- **PPT-Resource-Hub**: Courseware resource sharing platform

---

## Skills

| Category | Specific Skills |
|------|---------|
| Programming Languages | Python · TypeScript · Rust · Shell (Bash / PowerShell) |
| Frontend | React · Next.js · Vite · HTML5 Canvas · Three.js |
| Backend / AI | Qdrant (RAG) · LangGraph · MQTT · REST API · Prompt Engineering · LLM Multi-Provider Architecture |
| Operations / Infrastructure | Docker Compose · Nginx Reverse Proxy · SSH Deployment · iptables · Synology NAS · OpenWrt · 1Panel |
| Toolchain | Git · GitHub Actions · Linux (Debian/Ubuntu) · Windows Server |

---

## Education

- High school diploma (Liaobu Middle School, Senior High Division)
- Continuous self-study: Project-driven learning; in the past two years, systematically practiced Rust, TypeScript, Docker, LLM application development, and other tech stacks

---

## Additional Information

- **Languages**: Chinese (Cantonese, Mandarin), English (able to read technical documentation; writing with AI tool assistance)
- **GitHub**: [github.com/ikeee](https://github.com/ikeee)
- **Online Resume**: [ikeee.github.io/A1Q2/resume.html](https://ikeee.github.io/A1Q2/resume.html)
- **Current City**: Dongguan
