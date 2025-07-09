---
layout: post
title: Microsoft Build 2025 大会：开源 GitHub Copilot Chat、发布新的Copilot Coding Agent、全面支持MCP...
date: 2025-06-18
category: Frontier Trends
thumbnail: /style/image/microsoft-build-2025-github-copilot-chat-copilot-coding-agent-mcp_1.jpg
icon: game
---
* content
{:toc}

微软在2025年Build大会上全面展示了其迈向“AI代理时代”与“开放代理网络（Open Agentic Web）”的战略蓝图。
微软称：AI代理得益于推理与记忆方面的突破，正成为推动开发、协作和科学探索的核心力量。我们设想一个智能体能够跨个人、组织、团队以及端到端业务环境运作的世界。这一新兴的互联网愿景**是一个开放的智能体网络 **，其中的人工智能智能体能够代表用户或组织做出决策并执行任务。”
**主要发布亮点：**

- 发布企业级 AI 代理构建平台（多代理协作、定制化、低代码）。

- Copilot 支持企业自定义训练（Copilot Tuning）和多代理编排。

- GitHub Copilot 升级为异步编码代理；Copilot Chat 开源。

- 推出 Windows AI Foundry 和 Azure AI Foundry 模型集市。

- 全面支持 **Model Context Protocol（MCP）**：建立AI代理之间共享上下文的协议标准。

- 发布 **NLWeb 项目**：让网站像HTML一样开放给AI代理语义访问和交互。

![](https://assets-v2.circle.so/h8dp8ggrnwr9h3wico5fipw4gh5k)
## 微软的战略愿景：
![](https://assets-v2.circle.so/923txpuv0mq998faq217tqk7sgpe)
### 1️⃣ 重塑软件开发流程：AI 不再只是“辅助”，而是“参与者”

- **GitHub Copilot 升级为“编码代理”**不再只是智能补全，而是具备上下文记忆、任务规划、异步执行能力的开发伙伴。例如：你可以在GitHub中设定目标，它会帮你分析问题、生成代码、部署、做代码审查。

- **Copilot Chat 开源整合进 VS Code**GitHub Copilot 的聊天功能现在作为开源项目集成进 VS Code，开发者社区可参与定制、扩展，体现了微软对“开放开发”的承诺。

- **Windows AI Foundry 发布**提供统一平台支持AI模型的本地训练、微调、部署，兼容开源和私有大模型。开发者可以轻松运行视觉、语言模型，无需复杂配置。
![](https://assets-v2.circle.so/cg3yciz2gyx4yvfax13rhm60id1g)

### 2️⃣ 构建强大、可控的 AI 代理生态

- **Azure AI Foundry Agent Service 上线**面向开发者的AI代理构建平台，支持多个代理之间的协作（Multi-Agent）、上下文共享（Model Context Protocol）、语义工作流（Semantic Kernel）集成。

- **可观测性工具：性能、成本、质量一目了然**Azure提供了一整套代理监控工具，可以查看代理运行状况，包括响应速度、推理质量、资源消耗、安全问题等，提升企业可控性与合规性。

- **Entra Agent ID：为每个AI代理分配唯一身份**避免企业出现“代理泛滥”，确保每个AI系统的身份、权限、数据访问都受到严格管控。

### 3️⃣ 让企业拥有自己的“内部AI员工”

- **Copilot Tuning：企业自定义 AI 代理**企业可以用内部数据（如文档、流程、规章）快速训练AI代理，无需写代码。例如律所可构建专属文书生成代理，风格和表述都能贴合组织习惯。

- **多代理编排：任务分工、协作处理**在Copilot Studio中可以把多个代理编排成“任务流水线”，如：一个分析文档、一个生成汇总、一个发送邮件，共同完成复杂业务流程。

### 4️⃣ 推动“开放代理网络”（Open Agentic Web）

- 全面支持 **Model Context Protocol（MCP）**类似“AI通信协议”，让不同平台、模型之间共享上下文。GitHub、Azure、Copilot Studio等均已支持，

- NLWeb 项目：像HTML之于网页，NLWeb之于AI交互微软发布的新开放规范，允许网站以自然语言+结构化方式暴露接口，AI模型能更精准理解网页意图并与之交互，推动“语义互联网”建设。

- GitHub 和微软加入 **MCP标准制定委员会**，推进行业标准化。
![](https://assets-v2.circle.so/qqm3vnsp9sbjppk5mjaz3y4228uc)

### 5️⃣ AI + 科学研究：Microsoft Discovery 平台亮相

- **面向科学发现的AI平台**Microsoft Discovery旨在将“AI代理”嵌入科研流程：从数据探索、假设验证、模拟建模、实验设计，到论文撰写、成果分析，全流程加速。适用于制药、生物技术、能源、材料等多个领域，推动基础研究与产业转化效率提升。

## 开源 GitHub Copilot Chat
微软宣布将 **GitHub Copilot Chat ****插件开源**，并逐步把 AI 能力整合进 **VS Code 编辑器核心**。此举标志着 VS Code 正式迈向 “**开源 AI 编程环境**” 的新阶段。
![](https://assets-v2.circle.so/3eclbeabc9149hh10r6bunc9cupz)
### 📌 背景与动因
微软团队总结了当前AI开发与社区反馈的几个关键变化，并以此作为推进开源的决策依据：
1. **大模型能力演进，降低了对“秘方提示词”的依赖**
过去，为了获得更好的生成效果，AI 工具常需借助私有的提示词优化策略；但现在大模型本身的泛化能力更强，使得这种“私有化微调”策略不再是核心壁垒。
2. **用户体验（UX）模式已趋于成熟**
不同编辑器中的 AI 交互方式（如聊天窗口、自动代码补全样式等）越来越标准化。微软希望通过开源方式推动这些功能的开放共享，鼓励社区持续打磨。
3. **AI 插件生态正在扩张**
开发者希望构建自己的 AI 插件，但由于 Copilot Chat 插件是闭源的，调试和对接受限较多。开源后，开发者可更方便地学习其实现逻辑并实现深度集成。
4. **增加数据使用透明度**
社区用户关心 VS Code AI 插件收集了哪些数据，开源插件后，所有数据处理逻辑将一目了然，有助于建立信任。
5. **提升安全性，利用社区发现漏洞**
历史经验表明，开源有助于更快发现与修复安全漏洞。对于 AI 编辑器而言，这种开放机制尤为重要。

### 🧩 技术方案与后续规划
🔓 **Copilot Chat 插件开源**

- 插件代码将采用 **MIT License** 授权；

- 开源后将逐步把核心功能“拆解并融合”到 VS Code 核心模块中；

- 所有贡献者都可参与该插件的优化与重构。

🧪 **提示词测试框架也将开放**

- 为应对大模型推理结果的“非确定性问题”，微软将开放内部使用的**prompt 测试框架**；

- 这将帮助贡献者在提交 Pull Request 时验证功能是否稳定、输出是否可控。

🧩 **开发者贡献路径将简化**

- AI 相关功能将与其他 VS Code 核心功能一样易于参与贡献；

- 未来贡献 prompt、UI 逻辑、模型接入逻辑都将具备统一标准。

📌 版本管理与进展跟踪

- 所有开发进度将按月更新在 VS Code 的 Iteration Plan；

- 官方 FAQ 页面也会同步回答社区常见问题。

### 💡 开源后的实际价值
✅ 对开发者的意义
维度 说明 插件开发 可以学习插件源码、复用通用组件、更好调试 接入定制模型 不再依赖官方 Copilot，可替换为其他 LLM 安全与数据 明确哪些数据会被采集与使用，提高信任感 贡献门槛 更低的学习曲线，更完整的测试基础设施支持
✅ 对整个 AI 编程生态的意义

- 提供稳定的开源基础架构，促进标准化发展；

- 鼓励全球开发者协作，形成多样化的插件与模型适配层；

- 推动 AI 编程从“产品试用”走向“开发者自定义工具链”的新时代。

## 新的编程代理：Copilot Coding Agent
![](https://assets-v2.circle.so/5wphr565bksrnigfvu2x7xhf3xik)同时微软发布了新的Copilot Coding Agent，一个**可被分配任务、自动提交代码、并集成 CI/CD 流程**的 AI 代理，具备自主编码、分析和迭代的能力。
它不再只是辅助写代码，而是一个可以主动**执行开发任务**的“AI代理（Agent）”。

### 核心能力与工作流程
1. **任务驱动型自动开发**

- 可将任意 GitHub Issue 分配给 Copilot Agent（通过 Web、CLI、VS Code、GitHub App 等方式）

- Agent 会自动：
启动安全虚拟环境（基于 GitHub Actions）

- 克隆代码库、解析上下文（使用增强检索 + RAG 技术）

- 编写、推送代码到 Draft PR

- 更新 PR 描述并记录行为日志

2. **具备上下文理解能力**

- 利用 GitHub 代码搜索、文件结构和历史讨论分析任务意图

- 支持从 PR/Issue 中提取图片，进行视觉分析（如 UI Mockup）

- 可响应人类开发者对 Draft PR 的修改评论并持续迭代

3. **多模型调用能力（MCP协议支持）**

- 通过 **Model Context Protocol（MCP）**，Agent 可访问非 GitHub 数据源（如企业内部 API 或外部文档数据库）

- 用户可在项目设置中配置自定义 MCP Server
00:00UnmuteMuteSettingsCaptionsDisabledQuality1080pSpeedNormalCaptionsGo back to previous menuQualityGo back to previous menu480pSD720pHD1080pHDSpeedGo back to previous menu0.5×0.75×Normal1.25×1.5×1.75×2×4×PIPExit fullscreenEnter fullscreenPlay

### 安全与权限控制机制
为了确保团队代码库的安全性，Copilot Agent 设计了一整套严格的保护策略：

![](https://assets-v2.circle.so/n5y5zpp7mvdl75ewellapzxbz7wm)
### 使用场景与适用边界
💡 适用任务类型：

- 中低复杂度、需求清晰、边界明确的任务
Bug 修复、单元测试补全、代码重构、文档更新等

- 初步实现需求模板、迁移代码结构、拆分逻辑模块等

🧭 不适用场景：

- 创新性极强、缺乏明确上下文、跨域依赖极多的任务

- 需要大量主观判断和深度产品理解的需求

### 集成方式与环境支持

- 默认运行环境：**GitHub Actions**

- 本地 Agent 模式支持：VS Code、Xcode、Eclipse、JetBrains、Visual Studio 等主流 IDE

- 企业用户可统一设置激活策略，控制哪些项目可启用 Agent 模式

### 使用政策与计费说明

- **面向用户**：Copilot Enterprise 与 Copilot Pro+ 用户可使用

- **自 2025年6月4日 起**，每次 Agent 请求将计为一次**高级 Copilot 请求**，用于计费结算

### 与传统 Copilot 的区别
![](https://assets-v2.circle.so/xuhvb513p8guq9c3yq4vhgswy543)更多Microsoft Build 2025 大会内容：https://blogs.windows.com/windowsdeveloper/2025/05/19/advancing-windows-for-ai-development-new-platform-capabilities-and-tools-introduced-at-build-2025/
See more