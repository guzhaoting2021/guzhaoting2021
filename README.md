<div align="center">

## Hi, I'm ZT Gu 👋

**AI Application Engineer · Manufacturing Digitalization**<br/>
AI 应用工程师 · 制造业数字化

*I turn LLMs into production tools for the factory floor, the quality lab and the sales office.*<br/>
*把大模型做成工厂、品质、销售每天真正在用的生产力工具。*

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Vue](https://img.shields.io/badge/Vue_3-4FC08D?style=flat-square&logo=vuedotjs&logoColor=white)
![React](https://img.shields.io/badge/React_19-61DAFB?style=flat-square&logo=react&logoColor=black)
![Electron](https://img.shields.io/badge/Electron-47848F?style=flat-square&logo=electron&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-5FA04E?style=flat-square&logo=nodedotjs&logoColor=white)
![Claude](https://img.shields.io/badge/Claude-D97757?style=flat-square&logo=anthropic&logoColor=white)
![vLLM](https://img.shields.io/badge/vLLM-on--prem-30A2FF?style=flat-square)

</div>

### ⚡ About · 关于我

- 🏭 **AI × Manufacturing** — drawing review, quality inspection, order-to-cash. Real users, real production data.<br/>
  AI × 制造：图纸审核、品质检验、订单到回款，面向真实用户和生产数据。
- 🧠 **Full stack, end to end** — on-prem LLM serving, rule engines, agent runtimes, web and desktop apps.<br/>
  从私有化大模型部署、规则引擎、Agent 运行时，到 Web 与桌面应用，全链路自己做。
- 🌏 **Across US & China teams** — building the systems that connect sales, factory and finance.<br/>
  跨中美团队，打通销售、工厂与财务之间的系统。
- 🎯 **From interview to production** — requirement research → design → code → deployment → iteration.<br/>
  从需求调研到上线迭代，一个人跑完整个闭环。

### 🚀 Featured Projects · 代表项目

#### 📐 Drawing Review AI · 图纸智能审核 &nbsp;`In production`
Rule engine + multimodal LLM that checks customer drawings against internal drawings line by line, returning **Same / Different / Needs review** for every requirement.<br/>
规则引擎 + 多模态大模型，逐条比对客户原图与内部转化图，每一项给出「一致 / 不一致 / 需复核」。
- **30+ declarative rules** in YAML with pluggable strategies — exact / synonym / regex / visual pattern / LLM semantic judge<br/>
  30+ 条 YAML 声明式规则、可插拔策略，确定性规则与大模型语义判决各司其职
- **5 business modules**, incl. BOM Excel × multi-PDF batch auto-matching and old-vs-new revision diff with revision-block verification<br/>
  5 大业务模块，含 BOM 与多份图纸批量自动配对审核、新旧版图纸差异对比与版本栏声明核对
- **Fully on-prem** — self-hosted Qwen on vLLM (one model for text + vision); drawings never leave the plant network<br/>
  全私有化：vLLM 自托管 Qwen(文本 + 视觉一体)，图纸数据不出厂区网络
- Rebuilt UI in Vue 3 + TypeScript + Tailwind, with side-by-side / overlay / slider PDF comparison<br/>
  Vue 3 + TS 重写前端，支持并排 / 叠加 / 滑块三种图纸对比视图

`Flask` `Vue 3` `TypeScript` `vLLM` `Qwen` `MySQL` `pdf.js`

#### 🔎 Drawing Review Copilot · AI 图纸评审助手 &nbsp;`Prototype v0.5`
Upload a customer drawing, get an engineering-grade review in minutes: FAI dimension & tolerance table, manufacturability and push-back points, measurement difficulty, inspection equipment, and what's missing.<br/>
上传客户图纸，几分钟内拿到工程级评审：FAI 尺寸公差表、可制造性与可推回的要求、测量难点、检测设备建议、图纸缺失项。
- Every cell editable, findings accept / dismiss, one-click **Excel + Word** export<br/>
  结果可逐格编辑、逐条确认，一键导出 Excel / Word
- Multi-revision compare — every changed requirement, its impact, and whether the revision block records it<br/>
  多版本比对：列出每处变更、影响，以及版本栏是否如实记录
- Ask-AI chat drafts customer emails and factory requirements in Chinese<br/>
  内置 AI 对话，一键起草客户邮件、给工厂的中文要求
- **EN / 中文 one switch** — numbers, tolerances and part numbers are verified unchanged after translation<br/>
  中英一键切换，翻译后自动校验数字、公差、料号零改动

`Node.js` `Claude API` `Excel / Word export`

#### 🔗 Order Hub × QuickBooks Online · 跨境订单中枢 &nbsp;`In progress`
One source of truth from US sales order → China production & shipment → customs → delivery → invoice → payment.<br/>
打通「美国销售单 → 中国生产发货 → 清关入库 → 发货 → 开票 → 回款」全链路。
- Phase 1: a bridge that syncs existing Excel workflows into **QuickBooks Online** via API and writes payment status back — zero disruption to how people work<br/>
  第一步：桥接程序把现有 Excel 流程同步进 QuickBooks Online，并回写收款状态，不改变大家的工作习惯
- Roadmap: quoting → receiving / inventory / shipping → landed cost, dashboards and AI<br/>
  路线：报价协同 → 到货 / 库存 / 发货 → 到岸成本、经营看板与 AI

`QuickBooks Online API` `Node.js`

#### 🖥 Desktop AI Workspace · 桌面 AI 工作台
A self-hosted, local-first desktop workbench for AI agents — **Claude Agent SDK** runtime routed to DeepSeek through an Anthropic-compatible API.<br/>
自托管、本地优先的桌面 AI 工作台，内核为 Claude Agent SDK，通过 Anthropic 兼容协议接入 DeepSeek。
- Agents, Skill marketplace, knowledge base, MCP connectors, project-folder authorization<br/>
  Agent、Skill 市场、知识库、MCP 连接器、项目目录授权
- Human-in-the-loop **approval bus**, permission policies, SSE streaming, full run history<br/>
  人在回路的审批总线、权限策略、流式输出、完整执行记录
- Zero-dependency Node backend + SQLite, React 19 front end, packaged for macOS & Windows<br/>
  零依赖 Node 后端 + SQLite，React 19 前端，Mac / Windows 双平台打包

`Electron` `React 19` `Claude Agent SDK` `DeepSeek` `MCP` `SQLite`

#### 📰 AI Weekly Digest · AI 周报
Collects AI news every Monday and delivers a formatted HTML email digest — fully on GitHub Actions, zero servers.<br/>
每周一自动汇总 AI 应用与基建资讯，生成 HTML 邮件推送，全程 GitHub Actions，零服务器。

`GitHub Actions` `Python`

### 🧭 How I Build · 我的做法

- **Rules where they're reliable, LLMs where judgment is needed** — every AI verdict stays traceable.<br/>
  规则能判的不交给模型，交给模型的要可追溯。
- **On-prem first** when the data is sensitive. · 敏感数据优先私有化。
- **Fit the workflow, don't fight it** — integrate with the tools people already trust.<br/>
  顺着现有流程做，接入大家已经信任的工具，而不是逼人换。

### 🛠 Tech Stack · 技术栈

- **AI** — Claude API · Claude Agent SDK · MCP · vLLM · Qwen · DeepSeek · multimodal document understanding
- **Backend** — Python · Flask · Node.js · Express · MySQL · SQLite
- **Frontend** — Vue 3 · React 19 · TypeScript · Tailwind CSS · Electron · Vite
- **Integration & Ops** — QuickBooks Online API · GitHub Actions · Nginx · Linux · Playwright

---

<sub>Most of my work lives in private repositories — happy to walk through it. · 项目多为内部私有仓库，欢迎交流。</sub>
