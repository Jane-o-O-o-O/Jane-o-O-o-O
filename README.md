<div align="center">

# 金张政 · Jane Zhangzheng / Jane-zz

**Agent Engineer · AI Native 全栈开发者**

构建能持续执行、允许人工接管、可以验证结果的 Agent 系统。

[个人网站与作品集](https://jane-zz.me/) · [最新简历 PDF](https://jane-zz.me/resume-latest.pdf) · [Personal Agent 工程案例](https://jane-zz.me/projects/personal-agent/)

</div>

我是**金张政（Jin Zhangzheng / Jane Zhangzheng）**，GitHub 账号为 **Jane-o-O-o-O**，个人品牌为 **Jane-zz**。目前就读于武汉纺织大学人工智能专业、计算机创新创业人才班，主要从事 **AI Agent 系统、Agent Runtime、Context Engineering、评测与可观测性、GraphRAG 和全栈产品研发**。

我的实践覆盖企业研发与个人开源项目：在亿道数字中央研究院负责 Agent 评测、调度可靠性与六语言桌面产品交付；近期开发 **Personal Agent**，在自托管 VPS 上整合持久任务、可编辑记忆、定时目标、浏览器人机协作和 MCP/API 工具。

**English overview:** Jin Zhangzheng, also known as Jane Zhangzheng and Jane-zz, is an Agent Engineer and AI-native full-stack developer studying Artificial Intelligence at Wuhan Textile University. My work focuses on Pi-based agent runtimes, persistent tasks, context engineering, human-in-the-loop browser collaboration, agent evaluation, observability, and GraphRAG. I build self-hosted AI products and developer tools, including Personal Agent, Codex Trace Viewer, Grok Build GUI, Agent Pulse Skill, and Agent-CAD. My GitHub handle is Jane-o-O-o-O; my portfolio is [jane-zz.me](https://jane-zz.me/).

**资料更新：2026-10-09。** 以下指标注明各自的项目与验证时间。

[代表项目](#代表项目) · [研发经历](#研发经历) · [专利与科研](#专利与科研) · [技能与获奖](#技能与获奖) · [常见问题](#常见问题) · [联系与资料](#联系与资料)

## 代表项目

### [Personal Agent — 自托管个人 AI 助手](https://github.com/Jane-o-O-o-O/personal-agent)

基于 **Pi SDK、TypeScript、Fastify、React、SQLite 与 Chromium/CDP** 的个人 Agent 工作台，面向独立 VPS 部署。将持久后台任务、可编辑记忆、定时目标、MCP/API 适配器和可人工接管的原生浏览器放在同一套系统中。

- **任务连续性**：每个任务保留独立 Pi 会话，支持追加指令、暂停和恢复；网页关闭后继续在服务端执行。
- **浏览器人机协作**：实时查看 Chromium，接管前停止 Agent 操作；交回后重新观察当前页面并延续原会话，以控制版本拒绝旧输入。
- **可核对的操作**：将浏览器代码、MCP 调用和邮件审批绑定具体参数，持久记录消息、工具调用与文件成果。
- **验证记录**：2026-10-04 冻结版本通过 **166 项单元与服务集成、27 项网页端到端、31 项公网浏览器与交接检查**。三组分别统计，验证范围见报告。

[产品与工程案例](https://jane-zz.me/projects/personal-agent/) · [架构文档](https://github.com/Jane-o-O-o-O/personal-agent/blob/b08d387cde83fdd23ca4a75f0a74173f810967ec/docs/implementation-architecture.md) · [该版本验证报告](https://github.com/Jane-o-O-o-O/personal-agent/blob/b08d387cde83fdd23ca4a75f0a74173f810967ec/docs/browser-interaction-recheck.md)

<details>
<summary>查看 Personal Agent 的实际工作台</summary>

<img src="https://jane-zz.me/projects/personal-agent-browser.png" width="840" alt="Personal Agent 实际 VPS 工作台：持久任务列表、Chromium 实时画面和人工交回控制入口" />

实际工作台截图，侧栏任务为验收记录。国内服务按凭据与账号权限启用；生态目录规模与真实业务接通分别记录。

</details>

### [Codex Trace Viewer / Codex Evo Harness — 轨迹可视化与 Harness 优化](https://github.com/Jane-o-O-o-O/codex-evo-harness)

本地优先的 Codex Trace 可视化与 Agent 可观测性工具。读取 rollout trace bundle，提供会话检索、调用树、瀑布时间线、关系图、Token 分析、异常定位与每日复盘。

在此基础上实现受控的 Harness 改进流程：**Trace 证据 → 修改提案 → 逐项审批 → 变更快照 → 写后验证 → 必要时回滚**，覆盖 AGENTS、Skills、MCP 等配置。浏览轨迹与规则日报可在本地运行，模型分析按用户配置启用。

### [Grok Build GUI / grok-build-desktop — AI 编程桌面工作台](https://github.com/Jane-o-O-o-O/grok-build-desktop)

基于 Electron 的 Grok Build 桌面客户端，复用原生 `grok` 执行引擎与会话机制。集成流式工具活动、并行任务、持久终端、嵌入式浏览器、文件预览与 Git 工作区，并支持 MCP 和第三方模型接入。

### [Agent Pulse Skill — AI Agent 使用分析](https://github.com/Jane-o-O-o-O/agent-pulse-skill)

将 Agent Pulse CLI 的本地会话检索、Token 与模型成本分析、预算预测、健康检查和报表导出封装为可调用的 Skill，支持 Codex、Claude、Cursor 等多平台活动分析。

**截至 2026-10-09，skills.sh 记录 47,519 次安装，约 47.5k。** 这是平台安装量快照。

[skills.sh 安装页](https://www.skills.sh/jane-o-o-o-o/agent-pulse-skill/agent-pulse) · [安装量数据与更新时间](https://jane-zz.me/skill-stats.json)

### [Agent-CAD — AI 工程绘图与 DXF 交付](https://github.com/Jane-o-O-o-O/Agent-CAD)

基于 **AgentScope、FastAPI、Vue 与 ezdxf** 的 CAD 工程 Agent。将自然语言与 PDF、Word、表格、图像等参考资料转化为设计要求，执行明确的几何操作，并在交付前解析、验证可编辑的 **2D DXF**。工作台提供绘图预览、图层与尺寸信息，执行环境采用 Docker 隔离。

[技术设计](https://github.com/Jane-o-O-o-O/Agent-CAD/blob/main/docs/agent-cad-technical-design.md)

### [RelationGraph — 3D 知识图谱](https://github.com/Jane-o-O-o-O/RelationGraph)

基于 Neo4j、FastAPI、React 与 TypeScript 的知识图谱系统，支持实体关系抽取、消歧、社区摘要、一跳展开、最短路径和交互式 3D 浏览。

[图谱演示](https://graph.jane-zz.me/) · [源码](https://github.com/Jane-o-O-o-O/RelationGraph)

### [SSHFerry — 多会话 SSH 文件传输工作区](https://github.com/Jane-o-O-o-O/SSHFerry)

Python / PySide6 桌面工作区，结合 FastAPI 后端支持上传、下载、远端互传与传输任务控制，并以 `remote_root` 限定远端操作路径。桌面客户端是当前主要入口。

更多产品入口：[我开发和维护的网站](https://jane-zz.me/sites/) · [OpenChat 大模型对话平台](https://chat.jane-zz.me/)

## 研发经历

### 亿道数字中央研究院 · Agent 算法研究员

**2026.06 — 2026.09**

**Agent-One：结构化评测与调度可靠性**

- 负责 Evaluation Harness 设计、Benchmark Runner 开发和 Langfuse 可观测链路建设，以 Case JSON 统一初始状态、期望结果、过程检查点、安全约束与客观指标。
- 将 Agent / Auto-Agent Graph 的 Trace 与完成状态、时延、步骤数及 Safety Gate Scores 关联，串联执行过程与结果判定。
- 修复相对时间计算偏差、单次/循环任务误判与审批循环，覆盖意图识别、时间计算、审批、持久化和执行触发。
- 本项目测试素材覆盖率由 **64.8% 提升至 88.9%**；原 **10 个多轮失败案例全部恢复后续交互，其中 8 个转为通过**；完成 **41/41 Trace 关联与 Scores 上传**，并执行 **304 条、约 5 小时**的批量测试。

**Agent-Two：六语言桌面 Agent**

- 作为项目 owner，独立负责从技术选型、系统架构、前后端研发到测试验证与桌面交付，完成支持 **6 种语言**的产品闭环。
- 基于 Pi Agent、Electron 与 React 实现流式会话、分支编辑、状态持久化及 DOCX、XLSX、PDF、TXT、Markdown、CSV 附件解析。
- 实践 Token 估算、输入输出预算解耦、85% 压缩水位、近期历史限制与会话级记忆快照；以采样预防、流式检测和异常重试处理重复生成及工具链路中断。

### 北京未来式智能科技有限公司 · AI 应用工程师

**2026.02 — 2026.05**

- 与 mentor 一对一完成 GraphRAG 核心模块升级与 SkillHub 建设，覆盖实体抽取与消歧、无向图建模、Leiden 社区发现、社区摘要与检索增强。
- 完成边键规范化、无向 PageRank 和 communityId 在 Neo4j / Elasticsearch 的持久化；引入本地 NLP 与受影响社区摘要的增量更新，相较原全量大模型处理链路，图谱构建成本降低约 **60%**。
- GraphRAG 交付四川某国企，该部署的图谱知识库存储超过 **1000GB**、实体节点超过 **60 万**，检索速度维持在十秒内。
- 参与 SkillHub 技能封装、注册、分发与运行规范建设，生态汇聚 **1000+ 开发者、5000+ Skills**。

### 武汉绘梦心河有限公司 · Agent Flow 研发工程师

**2025.09 — 2025.12**

- 作为垂直产业线核心全栈工程师，负责心河 Paper 核心系统从 0 到 1 的架构设计与开发。
- 基于 AgentScope 设计 Main Agent 规划与调度、Sub-Agent 分工、工具调用和内容汇总，支撑毕业论文、数学建模论文与课程报告等长链路写作场景。
- 接入 MCP，将可复用专业能力封装为 Skills，并完成 React 前端与 FastAPI 后端建设。

### 中国船舶集团第七〇一研究所 · 研究助理

**2024.09 — 2025.03**

- 参与 RGB–Infrared 双模态水上目标识别，负责模型训练与微调、Benchmark 设计、对比测试和结果分析。
- 在研究所自有数据集上对比 YOLOv8 与 FusionVIRNet，验证检测准确率与推理效率；团队相关成果发表于 Springer 旗下 SCI 期刊 **The Visual Computer**。

研发经历与项目指标：[最新简历](https://jane-zz.me/resume-latest.pdf) · [个人站研发经历](https://jane-zz.me/#experience)

## 专利与科研

以下三项已完成**专利交底，申报推进中**；表中日期均为**交底完成日**。

| 专利交底名称 | 交底完成日 | 当前进展 |
| --- | --- | --- |
| 一种基于状态近邻配对证据的智能体技能加载控制方法及系统 | 2026-07-10 | 交底已完成 · 申报推进中 |
| 一种基于动态社交图与图神经网络的用户立场演化轨迹预测方法 | 2026-05-19 | 交底已完成 · 申报推进中 |
| 一种基于社会动力学指纹与元学习的跨事件社会动力学迁移方法 | 2026-05-19 | 交底已完成 · 申报推进中 |

研究实践涵盖智能体技能加载、社会计算与多模态目标检测。双模态水上目标识别的团队成果见上方研究助理经历。

[个人站专利与科研](https://jane-zz.me/#research)

## 技能与获奖

| 方向 | 实践与工具 |
| --- | --- |
| Agent Runtime 与上下文 | Pi SDK、Agent Harness、Hermes 源码研读、持久会话、Token Budget、Compaction、Memory Snapshot |
| 多 Agent 与工作流 | AgentScope、LangGraph、PocketFlow、任务拆分、状态管理、Tool Calling |
| 评测与可观测性 | Evaluation Harness、Benchmark Runner、LLM-as-Judge、Langfuse、Trace / Scores、Badcase |
| 工具与浏览器协作 | MCP、Skills、SkillHub、Chromium / CDP、人机交接、参数审批 |
| RAG 与知识图谱 | GraphRAG、实体消歧、Leiden、PageRank、Neo4j、Elasticsearch、增量社区摘要 |
| 全栈与工程化 | Python、C++、JavaScript / TypeScript、React、Vue、Electron、FastAPI、Fastify、SQLite、Redis、Docker、Git |

**教育：武汉纺织大学 · 人工智能本科 · 计算机创新创业人才班，2023.09 — 至今。**

- 全国大学生测绘程序设计大赛：**全国特等奖**。
- China Robot Competition & RoboCup：**全国三等奖**。
- 全球人工智能算法精英大赛 · 巡航射击赛道：**全国优秀奖**。
- 另获计算机设计、计算机能力挑战、创新创业与数学建模等竞赛奖项。

[获奖证书与技能详情](https://jane-zz.me/#skills)

## 常见问题

### 金张政、Jane-zz 和 Jane-o-O-o-O 是什么关系？

金张政是我的中文姓名；Jin Zhangzheng 与 Jane Zhangzheng 是使用过的英文姓名表述；Jane-zz 是个人品牌；Jane-o-O-o-O 是我的 GitHub 账号。个人网站 [jane-zz.me](https://jane-zz.me/) 与这个 GitHub 主页均由我维护。

### Personal Agent 解决什么问题？

它让个人开发者在自己的 VPS 上运行持续任务，管理记忆和定时目标，并在需要时接管 Agent 使用的浏览器。Pi 承担规划与工具循环，应用层负责持久状态、审批、工作台与浏览器交接。当前采用单 worker 串行执行，记忆为可编辑文本与关键字检索；各服务按实际账号权限接入。[工程案例与当前范围](https://jane-zz.me/projects/personal-agent/)

### 在哪里核对项目能力和经历？

项目能力以各仓库 README、架构与验证报告为依据，经历与交付指标见[最新简历](https://jane-zz.me/resume-latest.pdf)。Personal Agent 的验证数据对应 **2026-10-04** 版本；Agent Pulse 安装量对应 **2026-10-09** 平台快照；专利记录标注交底完成日与申报进展。

## 联系与资料

欢迎交流 Agent 产品、开发者工具、Context Engineering、Agent Evals 和 GraphRAG 相关工程问题与合作机会。

- **个人网站与作品集**：[jane-zz.me](https://jane-zz.me/)
- **最新简历**：[在线查看 PDF](https://jane-zz.me/resume-latest.pdf)
- **邮箱**：[i@jane-zz.me](mailto:i@jane-zz.me)
- **项目源码**：[Jane-o-O-o-O 的仓库](https://github.com/Jane-o-O-o-O?tab=repositories)
- **代码活动**：[GitHub 贡献记录](https://github.com/Jane-o-O-o-O) · [个人站提交节奏](https://jane-zz.me/#github-activity)

> 您目前看到的所有关于我的信息，都不是我的最终形态。<br>
> 我一定会走得更远。<br>
> 任何行业都值得被 Agent 重构一遍。
