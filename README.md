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

- 武汉纺织大学人工智能专业本科生，长期投入 Agent 工程与大模型应用实践。
- 在三家互联网公司与中国船舶第七〇一研究所累计完成 **12+ 个月、4 段研发实践**。
- 研发范围覆盖 Agent 定时任务、Memory / Context、Evals、Multi-Agent、GraphRAG 与计算机视觉。
- 参与建设的 SkillHub 已服务 **1000+ 开发者、沉淀 5000+ Skills**；个人 Agent Pulse Skill 已获 **26.5k+ 安装**。
- 既关注 Agent 的推理与任务执行，也关注系统是否可追踪、可评测、可恢复和可维护。

> 您目前看到的所有关于我的信息，都不是我的最终形态。  
> 我一定会走得更远。  
> 任何行业都值得被 Agent 重构一遍。

---

## Agent 工程能力

| 方向 | 工程实践 |
| --- | --- |
| **Orchestration** | 使用 AgentScope、LangGraph 与 PocketFlow 进行主 / 子 Agent 设计、任务拆分、状态流转和工作流编排 |
| **Runtime & Harness** | 理解模型调用、执行循环、工具注册、会话状态、结构化事件、权限边界和执行结果反馈 |
| **Memory & Context** | 实践记忆更新、历史对话筛选与排序、上下文拼接、长度控制和后台清理任务 |
| **Tools & Ecosystem** | 开发 Tool Calling、MCP 与 Codex Skills，并参与 SkillHub 生态建设 |
| **Evals & Observability** | 参与 Agent 评测、结果统计与 Badcase 分析，熟悉 Langfuse 链路追踪和运行监控 |
| **Knowledge & Retrieval** | 完成 GraphRAG 实体合并、社区发现、摘要生成、图谱持久化与检索增强全链路实践 |

---

## 代表项目

### [grok-build-desktop](https://github.com/Jane-o-O-o-O/grok-build-desktop)

基于 Electron 的多 Agent 协作式 AI 编程工作台。采用“主 Agent + 多个独立任务 Agent”的协作模式，为每个 Agent 建立隔离的 Runtime、上下文和任务状态，并通过共享 Memory 与项目上下文同步保持协作一致。

将回答、思考和工具调用抽象为结构化事件，支持实时执行展示、状态追踪、会话续接、Git 分支管理、Diff 统计、Electron 沙箱与敏感密钥安全存储。

`Multi-Agent` `Electron` `Runtime` `Memory` `Structured Events`

### [Agent-Pulse-Skill](https://github.com/Jane-o-O-o-O/agent-pulse-skill)

面向 Agent 使用分析的 Codex Skill，skills.sh 下载安装量 **26.5k+**。支持 Codex、Claude、Cursor、Aider、Copilot 等平台日志的会话检索、Token 与成本统计、预算预测、健康检查和报表导出。

通过标准化 Skill 描述、命令选择流程与 JSON 快照，让 Agent 能根据用户意图自动调用对应 CLI 能力。

`Codex Skills` `Agent Observability` `CLI` `Token Analytics` `skills.sh`

[skills.sh](https://www.skills.sh/jane-o-o-o-o/agent-pulse-skills/agent-pulse) · [GitHub](https://github.com/Jane-o-O-o-O/agent-pulse-skill)

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

**AI 技术实习生 · 深圳市亿道信息集团 / 亿道研究院**<br>
`2026.06 - 至今`

- 参与 Ailyn 定时任务、记忆与上下文模块开发，维护任务触发规则、执行状态与异常处理。
- 完成历史对话筛选、排序、拼接和上下文长度控制，减少无效输入并提升多轮理解能力。
- 参与 Agent 评测流程建设，执行评测、统计结果并分析 Badcase，辅助优化一致性与任务完成效果。

**全栈工程实习生 · 北京未来式智能科技有限公司**<br>
`2026.02 - 2026.05`

- 完成无向图建模、实体解析合并、Leiden 社区发现、社区摘要生成与检索增强的 GraphRAG 全链路升级。
- 实现边键规范化、无向 PageRank 与 `communityId` 在 Neo4j / Elasticsearch 的全链路持久化。
- 参与 SkillHub 生态建设，将多项内部产品、MCP 与 RAGFlow 能力封装为 Skills，服务 1000+ 开发者。

**Agent 研发实习生 · 武汉绘梦心河有限公司**<br>
`2025.09 - 2025.12`

- 从零搭建基于 AgentScope 的论文生成工作流，完成主 Agent、子 Agent 与任务协作设计。
- 实现 Agent 工具调用、MCP 与 Skills，并负责完整工作流的设计和开发。
- 使用 React 与 FastAPI 完成前后端架构和复杂业务逻辑落地。

**研究助理 · 中国船舶集团第七〇一研究所**<br>
`2024.09 - 2025.03`

- 参与双模态水上目标识别方法研发与验证，并基于研究所数据集完成系统实验分析。
- 完成与 YOLOv8、FusionVIRNet 的对比实验。
- 参与目标检测技术与大模型微调优化。

---

## 技术栈

**Agent 工作流**

`LangGraph` `PocketFlow` `AgentScope` `Multi-Agent` `状态管理`

**Agent Runtime**

`Agent Harness` `Execution Loop` `Tool Registry` `Structured Events` `Sandbox`

**上下文与评测**

`Memory` `Context Engineering` `Langfuse` `Agent Evals` `Badcase`

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

- 全国大学生测绘程序设计大赛：**全国特等奖**，前 5%，2024。
- China Robot Competition & RoboCup：**全国三等奖**，2024。
- 全球算法精英大赛 · 巡航射击：**全国优秀奖**，2025.12。
- 另获计算机设计、计算机能力挑战、创新创业与数学建模等多项省级奖项。

---

## GitHub 数据

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=Jane-o-O-o-O&show_icons=true&theme=transparent&hide_border=true" width="48%" alt="GitHub Stats" />
<img src="https://github-readme-streak-stats.herokuapp.com/?user=Jane-o-O-o-O&theme=transparent&hide_border=true" width="48%" alt="GitHub Streak" />

![Profile Views](https://komarev.com/ghpvc/?username=Jane-o-O-o-O&color=2563eb&style=flat-square)

</div>
