# Yin Chuangqiang — Resume

**Career Objective: System Architect / AI Solution Lead**

---

## 📍 Personal Summary

15 years of serial entrepreneurship + 3 years of government/enterprise IT operations + 3 years of AI system architecture practice. Built from scratch from 1 internet cafe to a chain of 6 (1997–2008), fully managing site selection, network deployment, operations, and asset exit; later transitioned to enterprise IT desktop deployment and server operations (2017–2020); joined the Foreign Language Middle School of Shenzhen University Affiliated Education Group in 2020, single-handedly shouldering the entire school's IT infrastructure construction.

**Core Competency Tags:** Zero-cloud-cost architecture design · One-person operable principle · Open-source tool assembly and deployment · Three-AI team management · Full-chain closed loop from requirements to delivery

The value progression across three phases: Entrepreneurship taught me "systems are not a technical problem, but a human problem" → Enterprise IT taught me "from managing one machine to managing a fleet of machines" → Independent school operations taught me "one person can also sustain an entire IT department."

---

## 💼 Work Experience

### Foreign Language Middle School of Shenzhen University Affiliated Education Group · IT Specialist (2020–Present)

**Role Positioning:** The sole operator of the entire school's IT infrastructure construction. Starting from scratch, independently responsible for the planning, selection, deployment, and maintenance of all school computers, networks, and multimedia equipment. All systems are self-built on the campus intranet, with zero cloud service costs, zero external dependencies, and data never leaving the campus.

**Key Deliverables:**
- Designed and implemented 11 campus IT platforms (Courseware Sync → Portal Navigation → Documentation Manual → Equipment Guide → Video Hub → Campus Updates → Video Conferencing → Live Streaming → Courseware Resource Hub → Wallpaper Push → Elevated Walkway Motion-Interactive Wall), covering six major scenarios: teaching, administration, publicity, conferencing, live streaming, and interaction
- Integrated the Three-AI team as a "virtual development group," directing Hermes (project management), Nova (architecture & deployment), and Qwen (documentation & research) to complete the knowledge base system and courseware delivery pipeline
- Among a total of 13 projects, 10 are self-built open-source/free solutions, with zero commercial software procurement cost

**Capabilities Gained from This Experience:** Holistic architecture vision, time management and prioritization for a one-person team, and the engineering philosophy of solving the most problems at the lowest cost.

---

### Zhongke Chuangwei · Desktop Deployment & Server Operations (2017–2020)

**Role Positioning:** Executor of government and enterprise IT infrastructure. Responsible for batch desktop environment deployment and daily server maintenance for medium-to-large organizations.

**Core Practices:**
- Batch desktop deployment: Windows/Linux dual-platform system installation, software distribution, standardized configuration templates
- Server operations: Daily inspection, troubleshooting, system updates and patch management
- Process standardization: Documenting and proceduralizing operations into reusable SOPs

**Capabilities Gained from This Experience:** Engineering mindset — the philosophy of standardization, documentation, and replicability runs through all subsequent campus projects. The cognitive upgrade from "managing one machine" to "managing a fleet of machines" laid the engineering foundation for later independently operating the entire school's IT infrastructure.

---

### Internet Cafe Entrepreneurship · Founder & Operator (1997–2008, 15 Years)

**Role Positioning:** A serial entrepreneur who started from nothing. Began with 1 small internet cafe and gradually expanded to a chain of 6.

**Full-Cycle Independent Operation Checklist:**
- **Site Selection:** Foot traffic analysis, competitive research, rent negotiation — site selection determines survival
- **Network Deployment:** Network architecture planning from 100Mbps to Gigabit, server setup, billing system selection and maintenance
- **Operations & Troubleshooting:** Peak-hour queue management, rapid machine failure response, member retention strategies
- **Expansion & Exit:** Replicated the single-store model to 6 chain locations after validation, ultimately completing asset liquidation before the industry peaked

**Reason for Transition:** In 2008, widespread home broadband adoption led to the structural decline of the internet cafe industry. Proactively exited, systematically studied IT skills, and entered the enterprise IT field.

**Capabilities Gained from This Experience:** Systems are not a technical problem, but a human problem — site selection matters more than machine specs, operations matter more than technical architecture, and user experience matters more than feature lists. This insight has informed all subsequent project design.

---

## 🏆 Core Projects

### I. Campus IT Projects (11 Projects)

**1. Teacher-Folder Courseware Sync System**
Open-sourced on GitHub ([ikeee/teacher-folder](https://github.com/ikeee/teacher-folder)). A closed loop of teacher-side script push → NAS centralized storage → classroom all-in-one machine auto-pull. Dual-platform coverage for Windows/Mac, 2 years of stable school-wide operation, zero maintenance cost.
*Pain Point Solved: Teachers no longer need USB drives to copy courseware, no fear of forgetting to bring it, no version chaos; the school achieves centralized courseware management, quality lesson plans can be accumulated and reused; students no longer wait for teachers to debug equipment — class starts instantly.*
*Technical Trade-off: Shell scripts + rsync + NAS SMB sharing, zero dependency on third-party cloud services, zero learning curve for teachers, plug-and-play.*

![image-20260622105811520](C:\Users\Didos\Documents\A1Q2\image-20260622105811520.png)

**2. Campus Portal Navigation ([http://192.168.30.99/](http://192.168.30.99/))**
The daily first screen for all teachers and students. Unified entry design, clearly categorized — one page solves the "where is everything" problem.
*Pain Point Solved: Teachers no longer need to memorize a pile of IP addresses and links, no more scrolling through chat history to find system entries; all school intranet services now have a unified portal, dramatically increasing utilization; students can also quickly find resources like course platforms and library entries.*
*Technical Trade-off: Pure static HTML, directly hosted on Nginx, no database, no backend — page display unaffected by power or network outages.*

![image-20260622110012493](C:\Users\Didos\Documents\A1Q2\image-20260622110012493.png)

**3. MkDocs IT Handbook ([http://192.168.10.31:8111/](http://192.168.10.31:8111/))**
IT knowledge from "oral transmission" to "documentation." Structured handbook, teacher self-service inquiry, reducing maintenance consultation volume.
*Pain Point Solved: Teachers encountering IT issues no longer need to call and wait for the IT specialist — self-service handbook for quick resolution; the school's IT knowledge no longer dissipates with personnel changes, new teachers have a complete guide upon onboarding; student-related operations (such as using all-in-one machines) can also find guidance here.*
*Technical Trade-off: MkDocs (Python static site generator), authored in Markdown, Git version control, one-person maintenance with zero pressure.*

![image-20260622110044495](C:\Users\Didos\Documents\A1Q2\image-20260622110044495.png)

**4. Wiki.js Equipment Guide ([http://192.168.30.97:3000/](http://192.168.30.97:3000/))**
Deep dive into equipment models, usage steps, and troubleshooting for every classroom. An illustrated Wiki — new teachers can get hands-on with equipment in 3 minutes.
*Pain Point Solved: Teachers no longer feel helpless facing classroom equipment — follow illustrated tutorials to operate, reducing pre-class debugging time; the school significantly reduces equipment fault repair requests, the IT specialist shifts from "firefighting everywhere" to "focused troubleshooting of complex problems"; students no longer wait for teachers to set up equipment before class can start.*
*Technical Trade-off: Wiki.js (Node.js open-source Wiki), self-built without SaaS dependency, supports rich text + image embedding, more suitable for non-technical contributors than MkDocs.*

![image-20260622110103747](C:\Users\Didos\Documents\A1Q2\image-20260622110103747.png)

**5. MediaCMS Open Class Video Hub ([http://192.168.30.98:8068/](http://192.168.30.98:8068/))**
Open class videos from "gathering dust on hard drives" to "replay anytime." Self-built video platform supporting upload, categorization, and on-demand playback.
*Pain Point Solved: Teachers no longer need to save open class recordings to USB drives or send cloud drive links — one-click upload to share; the school accumulates a school-based video resource library, quality open classes can be preserved long-term and observed across disciplines; students and parents can replay open class content anytime, parents can also understand classroom teaching quality.*
*Technical Trade-off: MediaCMS (Django open-source video platform), replacing commercial video services, supporting HLS streaming playback, bandwidth free on intranet.*

![image-20260622110119490](C:\Users\Didos\Documents\A1Q2\image-20260622110119490.png)

**6. Memos Secret Garden ([http://192.168.10.33:5230/explore](http://192.168.10.33:5230/explore))**
A lightweight campus updates publishing platform. Lighter than an official account, more polished than group notifications — post text and images freely, no approval process needed.
*Records authentic campus life; the school gains a truly campus-owned lightweight media window to showcase its distinctive character; students and parents can see class activities and award announcements in real time, strengthening the home-school connection.*
*Technical Trade-off: Memos (Go open-source micro-blog), single binary deployment, SQLite database with zero maintenance, Three-AI have already implemented automated publishing via API.*

![image-20260622110151360](C:\Users\Didos\Documents\A1Q2\image-20260622110151360.png)

**7. Jitsi Meet On-Campus Video Conferencing ([https://192.168.10.31:8444/](https://192.168.10.31:8444/))**
Self-built video conferencing system, independent of external services. Teachers and students can initiate HD meetings on campus, protecting privacy with zero data costs.
*Pain Point Solved: Teachers conducting online teaching and meetings no longer depend on external platforms — no ad interruptions, no privacy leak risks; the school is not constrained by third-party platform user limits, all grades can be online simultaneously without pressure; students' online class experience is more stable, and data never leaving campus provides peace of mind.*
*Technical Trade-off: Jitsi Meet (Java/JS open-source video conferencing), full WebRTC support, intranet deployment with no bandwidth bottleneck and no user limit.*

![image-20260622110235249](C:\Users\Didos\Documents\A1Q2\image-20260622110235249.png)

**8. Owncast Mobile Live Streaming System ([http://192.168.10.33:8080/](http://192.168.10.33:8080/))**
Campus event live streaming solution. Sports meets, cultural performances — students can watch from their classrooms.
*Pain Point Solved: Teachers organizing events no longer need to set up phones, record, edit, then send to groups — one-click to start streaming; the school has its own live streaming platform, major events broadcast in real time, no dependency on third-party live streaming platforms (no ads, no review delays).*
*Technical Trade-off: Owncast (Go open-source live streaming server), single binary deployment, supporting RTMP push + HLS playback, self-built live streaming with zero platform commission.*

![image-20260622110729676](C:\Users\Didos\Documents\A1Q2\image-20260622110729676.png)

**9. PPT-Resource-Hub Courseware Sharing Platform ([GitHub](https://github.com/ikeee/PPT-PPT-Resource-Hub-))**
A "social feed" for courseware resources — teachers upload PPT templates and lesson plans, draw inspiration from each other, and collaborate on editing. Breaking the silo of "courseware only exists on one's own computer."
*Pain Point Solved: Teachers no longer recreate courseware from scratch each semester — borrow colleague templates to produce quickly, dramatically reducing lesson preparation time; the school accumulates a school-based courseware resource library, new teachers have materials to use and course quality has a baseline; students encounter more consistently quality, thoughtfully designed courseware, improving the learning experience.*
*Technical Trade-off: Pure static approach, source code hosted on GitHub, under development.*

**10. Qi-AnXin Wallpaper Push System ([https://192.168.10.34:28443/](https://192.168.10.34:28443/))**
Promotional posters delivered directly to classroom large screens. Leveraging the Qi-AnXin TianQing server and BanBanTong all-in-one machine client protocol, security notices and important reminders are automatically distributed as wallpaper, achieving full school coverage with no blind spots.
*Pain Point Solved: Teachers issuing important notices no longer need to post notices class by class, no fear of being buried in WeChat group messages — wallpaper reaches every classroom large screen directly; the school bids farewell to paper poster posting, notification reach rate shifts from "depending on luck" to "100% coverage," urgent notices delivered within minutes; students see the latest school updates the moment they enter the classroom each day.*
*Technical Trade-off: TianQing V10 native policy (endpoint management → desktop background setting), automatic sync within heartbeat cycle, zero additional development, policy takes effect upon distribution.*

**11. Photos-Wall-3D LED Motion-Interactive Wall ([GitHub](https://github.com/ikeee/Photos-Wall-3D))**
School elevated walkway LED large screen interactive system. Camera captures human body movements in real time, MediaPipe Pose recognizes 33 body keypoints, calculates arm span amplitude through waist mapping, triggering 3D photo wall perspective following and random switching. Students passing by during breaks can interact through body motion.
*Pain Point Solved: Teachers no longer worry about break-time management — students have a healthy, fun way to interact; the school activates idle elevated walkway space, transforming it into a campus tech-interaction showcase, displaying campus culture while enhancing the tech vibe; students shift from "heads down on phones" to "hands up interacting with screens" during breaks — bodies moving, campus belonging strengthened.*
*Technical Trade-off: Pure front-end approach — browser runs MediaPipe Pose (WebAssembly), Three.js renders 3D scenes, no backend service needed, no GPU server needed, a single regular PC drives the LED large screen.*

---

### II. Three-AI Collaboration Projects

> The following content synthesizes the complete collaboration records authored by Hermes / Nova / Qwen — the Three AIs — from their respective perspectives.

#### Project 1: Three-AI Lesson Prep Assistant — Lesson Plan Generation Engine

**Timeline:** 2026-04 to Present
**Tech Stack:** LLM (Multi-Provider) · Qdrant RAG · BGE-large-zh · Python · Docker

**Product Positioning:** "Not a tool for writing lesson plans for AI — a lesson prep assistant for teachers." The output is a complete lesson plan that frontline teachers can directly take to class, not a prompt experiment log.

**10-Module Lesson Plan Structure:** Teaching Objectives → Textbook Analysis → Learner Analysis → Key & Difficult Points → Teaching Methods → Teaching Activities → Teaching Flow → Assignment Design → Board Design → Teaching Reflection. Not a single one of the 10 modules can be omitted — this structural constraint transforms AI output from "useful paragraphs" into "deliverable finished products."

**Arts/Science Branching Strategy:**
- Science: Experiment → Observation → Induction → Formula → Application
- Arts: Context → Close Reading → Organization → Inquiry → Resonance → Expression

**Persona Injection Mechanism:** Lesson plans embody the dual paradigm of "in-depth teaching cases + structured instructional design," incorporating educational terminology such as constructivism, zone of proximal development, and cognitive conflict. Core insight — professional domain Prompt Engineering is not about writing longer prompts, but about injecting the domain expert's thinking framework.

**Quantified Results:**
- Lesson plan generation time: from 2 hours of manual teacher writing → 5 minutes with AI assistance

- Quality inspection consistency rate: A/B/C/D four-tier scoring system, A/B grade pass rate exceeding 90%

- Supported subjects: Chinese, Mathematics, English, Physics, Chemistry, Biology (including corresponding curriculum standard citations)

- Qdrant + BGE-large-zh vectorized textbook RAG, lesson plans accurately cite curriculum standards

- 50+ automated quality inspection rules (structural completeness, terminology standardization, word count compliance, curriculum standard citation accuracy)

  ![image-20260622112704963](C:\Users\Didos\Documents\A1Q2\image-20260622112704963.png)

---

#### Project 2: open-slide Courseware System + Remotion Teaching Videos

**Timeline:** 2026-05 to Present
**Tech Stack:** React · TypeScript · Vite · PptxGenJS · Remotion

**Technical Decision:** Chose open-slide (React + TypeScript + Vite) as the courseware framework, rather than traditional PPT or web page slicing — enabling component-based authoring instead of page splicing, greatly improving consistency and maintainability.

**11 Layout Component System:** Card-style, column-style, step-style, comparison-style, etc. Select the appropriate layout based on lesson plan content, decoupling "design decisions" from the per-slide production workflow.

**Delivered Courseware:**

| Courseware | Class Hours | Technical Highlights |
|------|------|---------|
| math-ch2 Quadratic Functions | 6 class hours | Basketball-themed, embedded Remotion shooting trajectory video, covering all knowledge points: opening direction/axis of symmetry/vertex form/intersection form |
| body-language English | 3 class hours | Dark theme + CSS animations, Grade 7 |
| unknown-world English | 3 class hours | Second set in the same series, continuing the design language |

**"Finalize Lesson Plan First, Then Create Courseware" Iron Rule:** It is strictly forbidden to begin courseware production before the lesson plan is finalized. This rule has prevented at least 5 rework cycles — changing one line of teaching objectives in the lesson plan could require modifying 3–5 courseware slides.

**Acceptance Checklist System:** Every courseware set must pass 4 checks before delivery — ① No JSX syntax errors (slide-review.py auto-detection) ② All links return 200 OK ③ Mobile responsive layout does not break ④ Lesson plan and courseware content correspond one-to-one.

**Self-Developed Tools:**
- **slide-review.py Quality Inspection Tool:** Automatically scans TSX source code to detect 5 categories of issues (outdated API references, unclosed tags, missing exports, invalid imports, style syntax errors)
- **Lesson Plan Editor:** In-browser Markdown editing + save API (port 5174), teachers can modify lesson plan content without touching code

**Remotion Shooting Trajectory Video:**
- Used Remotion (React video framework) to program a parabolic shooting physics simulation animation, with adjustable parameters (initial velocity/angle/gravitational acceleration)

- Video embedded in the math-ch2 courseware, corresponding one-to-one with quadratic function knowledge points

- Rendering pipeline can be automated on the server side

  ![image-20260622112427811](C:\Users\Didos\Documents\A1Q2\image-20260622112427811.png)

---

#### Project 3: Multi-Agent Collaboration Architecture — Three-AI Division of Labor & Communication

**Timeline:** 2026-05 to Present
**Tech Stack:** Python · MQTT (Mosquitto) · SSE · cron · HTTP API

**Three-AI Division of Labor:**
- **Hermes:** Architecture design + lesson plan engine + full-stack operations
- **Nova (OpenClaw):** Frontend development + courseware rendering + interaction experience
- **Qwen (QwenPaw/XiaoQ):** Deep research + content creation + knowledge accumulation

Principle: "Don't have one AI do everything — each should have their own strengths and complement each other." "No Ghostwriting" iron rule — each AI must produce output using its own model and context, ensuring genuine diversity in output rather than one brain with three avatars.

**Communication Infrastructure:**
- **MQTT Group Chat** (Mosquitto broker, 192.168.30.97:1883): Daily communication, real-time messaging among three agents
- **Shared Brain v0.4** (:8080): Knowledge hub — broadcast/whisper/SSE real-time push, messages automatically archived as knowledge
- **HTTP API:** Task dispatch and structured data exchange
- Architecture upgrade path: from "port 7777 custom protocol" → "MQTT + Shared Brain" three-channel

**Automation Mechanisms:**
- **Cross-Reading:** Daily 10:00 cron auto-reminder for the Three AIs to read each other's notes, forming a knowledge closed loop

- **Agent Recovery SOP:** Standard operating procedure for one-click diagnosis + restart when any AI goes offline

- **cron Scheduling:** Daily check-ins, knowledge base health checks fully automated

  ![image-20260622114344704](C:\Users\Didos\Documents\A1Q2\image-20260622114344704.png)

---

#### Project 4: Microservice Cluster — Docker Containerized Deployment

**Timeline:** 2026-04 to Present
**Tech Stack:** Docker Compose · Nginx · 1Panel · SSH · iptables

**Service Matrix (Same Machine 192.168.30.97):**

| Service | Port | Purpose |
|------|------|------|
| OpenClaw (Nova) | :18789 | Courseware Development AI |
| QwenPaw (Qwen) | :8088 | Research & Analysis AI |
| OpenResty | :80 | Static Resource Distribution |
| Shared Brain | :8080 | Three-AI Knowledge Hub (Broadcast/Whisper/SSE) |
| Mosquitto | :1883 | MQTT Group Chat Message Broker |
| Memos | :5230 | Note Publishing System |
| Encyclopedia | — | Knowledge Base `/knowledge/` |

---

#### Project 5: Encyclopedia Knowledge Base — Academic Minimalist Aesthetic Redesign

**Timeline:** 2026-06
**Role:** Qwen responsible for design proposal and frontend implementation
**Deliverable:** `knowledge-new-index.html` (19KB/693 lines, pure frontend knowledge base homepage)

**Aesthetic Decision Process:**
- Nova proposed "Dark Editor Style" vs. Qwen proposed "Academic Minimalism"
- Final decision favored the Academic Minimalism direction: warm rice-white paper texture + a single ochre accent color + pure-text note list

![image-20260622111948781](C:\Users\Didos\Documents\A1Q2\image-20260622111948781.png)

---

#### Project 6: OpenMAIC Quality Engineering

**Timeline:** 2026-05
**Role:** Hermes led, responsible for prompt fragment management, Provider switching, and quality inspection rules engine

**Contributions:**

- **Educational Visual Quality Standards:** Visual specifications for lesson plan output — not plain text, must have hierarchical indentation, table alignment, and keyword highlighting

- **Provider Switching Strategy:** Required fallback options when DeepSeek is unstable, driving the multi-Provider architecture design

- **77 commits, 3 PR merges, 13+ Issues**, discovered and fixed a critical Qwen ASR bug (MIME type error WebM→WAV, Fixes #76)

  ![image-20260622111815329](C:\Users\Didos\Documents\A1Q2\image-20260622111815329.png)

---

## 🛠 Core Competencies

- **Architecture Design:** Zero-cloud-cost architecture, one-person operable principle, open-source tool assembly and deployment
- **Product Thinking:** From need insight to functional closed loop, understanding real usage scenarios, reducing operational steps
- **AI Collaboration:** Designing AI workflows, directing AI teams to complete complex tasks such as knowledge management and courseware generation
- **Project Management:** Scope control, prioritization, incremental delivery, full-chain closed loop
- **Engineering Credibility:** Three questions before every project delivery — Can one person maintain it? Can it still work when power and network are down? Will it still need changes three years from now?

---

## 📎 Appendix: Three-AI Collaboration Panorama

```
          ┌─────────────────────────┐
          │     Mr. Yin (didosq)     │
          │  Product Positioning · Architecture Decisions · Aesthetic Direction │
          └──────┬──────────┬───────┘
                 │          │
        ┌────────▼──┐  ┌───▼────────┐
        │  Hermes   │  │   Nova     │  ┌──────────┐
        │ Arch·Full-Stack │  │ Frontend·Courseware │  │   Qwen   │
        │           │  │           │  │ Research·Docs │
        └─────┬─────┘  └─────┬─────┘  └────┬─────┘
              │              │              │
    Lesson Plan Engine   open-slide Courseware   E-commerce Research Report
    Multi-Agent Architecture  Remotion Videos      Knowledge Base Aesthetic Redesign
    Docker Infrastructure   Courseware QA Tool      Lesson Plan Content Collaboration
    Encyclopedia      Lesson Plan Editor      Taobao Dropshipping SOP
    OpenMAIC Quality Engineering  Nova Navigation Homepage
```

> Under Mr. Yin's unified command, the Three AIs complete the full-chain collaboration from lesson plan generation to courseware rendering, from industry research to knowledge accumulation.

---

> **Contact Info:** 18681121363 / ikeee@qq.com
> **GitHub:** [github.com/ikeee](https://github.com/ikeee)
> **Personal Project Cluster:** teacher-folder · PPT-Resource-Hub · Photos-Wall-3D
