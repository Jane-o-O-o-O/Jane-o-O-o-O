<div align="center">

# 金张政 / Jane-zz

**Agent Engineer · AI Native 全栈开发者**

从 Agent Harness 与 Runtime，到工作流编排、MCP / Skills、Memory / Context 与 Evals，<br>
持续构建真正可运行、可评测、可维护的 Agent 系统。

[![Website](https://img.shields.io/badge/Website-jane--zz.me-111827?style=flat-square&logo=vercel&logoColor=white)](https://jane-zz.me)
[![Resume](https://img.shields.io/badge/Resume-Latest-2563EB?style=flat-square&logo=readthedocs&logoColor=white)](https://jane-zz.me/resume-latest.pdf)
[![GitHub](https://img.shields.io/badge/GitHub-Jane--o--O--o--O-181717?style=flat-square&logo=github)](https://github.com/Jane-o-O-o-O)
[![Email](https://img.shields.io/badge/Email-i%40jane--zz.me-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:i@jane-zz.me)

`ALL IN AGENT`

</div>

---

## 关于我

- 武汉纺织大学人工智能专业本科生、计算机创新创业人才班成员，长期投入 Agent 工程与大模型应用实践。
- 已完成 **4 段研发实践**，覆盖三家企业与中国船舶第七〇一研究所。
- 研发范围覆盖 Agent 定时任务、Memory / Context、Evals、Multi-Agent、GraphRAG 与计算机视觉。
- 参与建设的 SkillHub 已服务 **1000+ 开发者、沉淀 5000+ Skills**；个人 Agent Pulse Skill 已获 **47,519 次安装**（2026-10-09 skills.sh 快照）。
- 独立交付支持 **6 种语言**的桌面 Agent；已完成 **3 项专利交底，申报推进中**。[专利与科研](https://jane-zz.me/#research)
- 既关注 Agent 的推理与任务执行，也关注系统是否可追踪、可评测、可恢复和可维护。

> 您目前看到的所有关于我的信息，都不是我的最终形态。  
> 我一定会走得更远。  
> 任何行业都值得被 Agent 重构一遍。

---

## Agent 工程能力

| 方向 | 工程实践 |
| --- | --- |
| **Orchestration** | 使用 AgentScope、LangGraph 与 PocketFlow 进行主 / 子 Agent 设计、任务拆分、状态流转和工作流编排 |
| **Runtime & Harness** | 基于 Pi SDK 实践持久会话、后台任务、执行循环、工具注册、结构化事件、权限边界和失败恢复 |
| **Memory & Context** | 实践记忆更新、历史对话筛选与排序、上下文拼接、长度控制和后台清理任务 |
| **Tools & Ecosystem** | 开发 Tool Calling、MCP 与 Codex Skills，并参与 SkillHub 生态建设 |
| **Evals & Observability** | 参与 Agent 评测、结果统计与 Badcase 分析，熟悉 Langfuse 链路追踪和运行监控 |
| **Knowledge & Retrieval** | 完成 GraphRAG 实体合并、社区发现、摘要生成、图谱持久化与检索增强全链路实践 |

---

## 代表项目

### [Personal Agent](https://github.com/Jane-o-O-o-O/personal-agent)

基于 Pi SDK、TypeScript、Fastify、React、SQLite 与 Chromium 的自托管个人 AI 助手。支持持久后台任务、定时目标、可编辑记忆、原生浏览器人工接管及 MCP/API 扩展，网页关闭后任务仍在服务端继续执行。

**2026-10-04 冻结版本**通过 **166 项单元与服务集成、27 项网页端到端、31 项公网浏览器与交接检查**，三组分别统计，范围见验证报告。

`Pi SDK` `Persistent Tasks` `Human-in-the-Loop` `Chromium` `MCP`

[工程案例](https://jane-zz.me/projects/personal-agent/) · [该版本验证报告](https://github.com/Jane-o-O-o-O/personal-agent/blob/b08d387cde83fdd23ca4a75f0a74173f810967ec/docs/browser-interaction-recheck.md)

### [grok-build-desktop](https://github.com/Jane-o-O-o-O/grok-build-desktop)

基于 Electron 的 Grok Build 桌面工作台，复用原生 `grok` Runtime、会话与 Memory 机制，集成主任务与并行侧任务、流式工具活动、持久终端、嵌入式浏览器和 Git 工作区，支持 MCP 与第三方模型接入。

已发布 **[v0.1.2](https://github.com/Jane-o-O-o-O/grok-build-desktop/releases/tag/v0.1.2)**，覆盖 **Windows、macOS、Linux**，提供 **59 项原生设置**；支持会话续接、工具状态追踪与敏感密钥安全存储。

`Multi-Agent` `Electron` `Runtime` `Memory` `Structured Events`

### [Agent-Pulse-Skill](https://github.com/Jane-o-O-o-O/agent-pulse-skill)

面向 Agent 使用分析的 Codex Skill，skills.sh 安装量 **47,519 次，约 47.5k**（2026-10-09 快照）。支持 Codex、Claude、Cursor、Aider、Copilot 等平台日志的会话检索、Token 与成本统计、预算预测、健康检查和报表导出。

通过标准化 Skill 描述、命令选择流程与 JSON 快照，让 Agent 能根据用户意图自动调用对应 CLI 能力。

`Codex Skills` `Agent Observability` `CLI` `Token Analytics` `skills.sh`

[skills.sh](https://www.skills.sh/jane-o-o-o-o/agent-pulse-skill/agent-pulse) · [GitHub](https://github.com/Jane-o-O-o-O/agent-pulse-skill)

### [RelationGraph](https://github.com/Jane-o-O-o-O/RelationGraph)

Neo4j + FastAPI + React + TypeScript 的 3D 知识图谱系统。支持实体构建与搜索、社区摘要、关系一跳展开、最短路径查询和 3D 交互浏览，并通过 spaCy 与 60+ 人物别名映射完成实体抽取和消歧。

`GraphRAG` `Neo4j` `React` `FastAPI` `spaCy`

[Live Demo](https://graph.jane-zz.me) · [GitHub](https://github.com/Jane-o-O-o-O/RelationGraph)

### [OpenChat](https://chat.jane-zz.me)

大模型对话与调优实验平台。支持系统提示词、工具调用、流式响应、采样参数、重复惩罚、seed 与 reasoning effort 等配置，用于验证模型设置对稳定性、创造性和推理质量的影响。

`LLM` `Tool Calling` `Streaming` `Prompt` `Model Tuning`

### [SSHFerry](https://github.com/Jane-o-O-o-O/SSHFerry)

多会话 SSH 文件传输工作区，采用 PySide6 桌面客户端与 FastAPI 后端。支持上传、下载、远端互传、`remote_root` 沙箱安全边界和任务可视化管控。

`Python` `PySide6` `FastAPI` `SSH` `SFTP`

[Live Demo](https://sshferry.cloud) · [GitHub](https://github.com/Jane-o-O-o-O/SSHFerry)

---

## 研发经历

**Agent 算法研究员 · 亿道数字中央研究院**<br>
`2026.06 - 2026.09`

- 负责 Agent-One 的 Evaluation Harness、Benchmark Runner 与 Langfuse 可观测链路，以 Case JSON 统一评测规格和判定依据。
- 本项目测试素材覆盖率由 **64.8% 提升至 88.9%**；原 **10 个多轮失败案例全部恢复后续交互，其中 8 个转为通过**。
- 优化定时任务从意图识别到执行触发的链路，修复相对时间计算偏差、单次/循环任务误判与审批循环。
- 作为 Agent-Two 项目 owner，基于 Pi Agent、Electron 与 React 独立完成支持 **6 种语言**的桌面 Agent，覆盖架构、前后端开发、测试与交付。

**AI 应用工程师 · 北京未来式智能科技有限公司**<br>
`2026.02 - 2026.05`

- 完成无向图建模、实体解析合并、Leiden 社区发现、社区摘要生成与检索增强的 GraphRAG 全链路升级。
- 实现边键规范化、无向 PageRank 与 `communityId` 持久化；引入本地 NLP 与社区摘要增量更新，相较原全量大模型处理链路，图谱构建成本降低约 **60%**。
- GraphRAG 交付四川某国企，该部署图谱知识库存储超过 **1000GB**、实体节点超过 **60 万**，检索速度维持在十秒内。
- 参与 SkillHub 技能封装、注册、分发与运行规范建设，服务 **1000+ 开发者、沉淀 5000+ Skills**。

**Agent Flow 研发工程师 · 武汉绘梦心河有限公司**<br>
`2025.09 - 2025.12`

- 从零搭建基于 AgentScope 的论文生成工作流，完成主 Agent、子 Agent 与任务协作设计。
- 实现 Agent 工具调用、MCP 与 Skills，并负责完整工作流的设计和开发。
- 使用 React 与 FastAPI 完成前后端架构和复杂业务逻辑落地。

**研究助理 · 中国船舶集团第七〇一研究所**<br>
`2024.09 - 2025.03`

- 参与双模态水上目标识别方法研发与验证，并基于研究所数据集完成系统实验分析。
- 完成与 YOLOv8、FusionVIRNet 的对比实验。
- 参与目标检测技术与大模型微调优化；团队相关成果发表于 Springer 旗下 SCI 期刊 **The Visual Computer**。

[最新简历与指标来源](https://jane-zz.me/resume-latest.pdf) · [研发经历详情](https://jane-zz.me/#experience)

---

## 技术栈

**Agent 工作流**

`LangGraph` `PocketFlow` `AgentScope` `Multi-Agent` `状态管理`

**Agent Runtime**

`Pi SDK` `Agent Harness` `Execution Loop` `Tool Registry` `Structured Events` `Sandbox`

**上下文与评测**

`Memory` `Context Engineering` `Langfuse` `Evaluation Harness` `Benchmark Runner` `Agent Evals` `Badcase`

**工具与生态**

`Tool Calling` `MCP` `Codex Skills` `SkillHub` `npx`

**RAG / GraphRAG**

`Embedding` `Vector Search` `Re-ranking` `Leiden` `Neo4j` `Elasticsearch`

**全栈工程**

`Python` `C++` `JavaScript` `TypeScript` `FastAPI` `Flask` `Django` `React` `MySQL` `MongoDB` `Redis` `Docker` `Git`

---

## 教育与奖项

**武汉纺织大学 · 人工智能本科**<br>
`2023.09 - 至今`

- 全国大学生测绘程序设计大赛：**全国特等奖**，2024。
- China Robot Competition & RoboCup：**全国三等奖**，2024。
- 全球人工智能算法精英大赛 · 巡航射击赛道：**全国优秀奖**，2025.12。
- 另获计算机设计、计算机能力挑战、创新创业与数学建模等多项省级奖项。

---

## GitHub 数据

<div align="center">

**3,762 次近一年贡献 · 53 个公开仓库**

<sub>2026-10-09 快照，贡献按 GitHub 贡献日历统计；下方图卡动态更新。</sub>

<img src="https://github-readme-stats.vercel.app/api?username=Jane-o-O-o-O&show_icons=true&theme=transparent&hide_border=true" width="48%" alt="GitHub Stats" />
<img src="https://github-readme-streak-stats.herokuapp.com/?user=Jane-o-O-o-O&theme=transparent&hide_border=true" width="48%" alt="GitHub Streak" />

![Profile Views](https://komarev.com/ghpvc/?username=Jane-o-O-o-O&color=2563eb&style=flat-square)

</div>
