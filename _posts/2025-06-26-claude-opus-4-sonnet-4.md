---
layout: post
title: Claude Opus 4 和 Sonnet 4 发布 专业级编程能力 能够连续运行数小时，处理成百上千个推理步骤
date: 2025-06-26 12:00:00 +0800
category: Frontier Trends
thumbnail: /style/image/claude-opus-4-sonnet-4_1.jpg
icon: note
---
* content
{:toc}

Anthropic 发布了 Claude 模型的第四代系列：**Claude Opus 4** 和 **Claude Sonnet 4**，这不仅是对原有模型的升级，更是面向未来 AI 应用场景的系统性进化。
无论是代码生成、复杂推理、长时间任务处理，还是智能代理构建，它们都展现出显著优势。
![](https://assets-v2.circle.so/smc6wiuchfpfw9wbjbcd4qb9qnky)在 Claude 4 的发布会上 Anthropic CPO Mike Krieger 详细阐述了 **Agent 底层的三大能力**：

- **情境智能（Contextual Intelligence）**：不再是简单的指令执行，而是理解"为什么"和"如何做"。你与 Agent 的第 100 次任务应该比第 1 次好得多，就像新员工的第 100 天应该比第 1 天表现更好；Claude 4 展示了这种能力的极致。在测试中，它会主动创建"记忆文件"保存关键信息。玩 Pokemon 时，它甚至会写导航笔记："尝试 5 次相同方法后卡住；如果卡住，尝试相反方向；室内导航时走到房间另一边。" 这种自主学习和知识积累，正是人类员工的核心价值。

- **长时间执行（Long-running Execution）**：处理需要数小时甚至数天的复杂任务，协调其他 Agent 和人类。这不仅是耐力问题，更是保持目标一致性和上下文连贯性的能力；

- **真正的协作（Genuine Collaboration）：**透明的推理过程，适应人类工作风格。关键是"智能自主"与"人类监督"的平衡 —— AI 处理繁琐细节，人类把控大方向。
00:00UnmuteMuteSettingsCaptionsDisabledQuality1080pSpeedNormalCaptionsGo back to previous menuQualityGo back to previous menu480pSD720pHD1080pHDSpeedGo back to previous menu0.5×0.75×Normal1.25×1.5×1.75×2×4×PIPExit fullscreenEnter fullscreenPlay视频内容来自@**indigo**

## 核心模型介绍

### ✅ Claude Opus 4 — 强大且持久的高级模型

- **主打：专业级编程能力、持续任务执行力**

- 在两个权威代码基准测试中表现领先：
SWE-bench 得分：72.5%

- Terminal-bench 得分：43.2%

**能够连续运行数小时，处理成百上千个推理步骤**，特别适合 AI 代理类任务和长周期研发场景。
应用反馈（真实用户验证）：

- Cursor：认为是“代码理解能力的重大飞跃”。

- Replit：多文件代码修改更精准。

- Block：“在代码编辑与调试中显著提升质量和稳定性”。

- Rakuten：其代理能独立运行7小时，性能稳定。

- Cognition：成功应对过去模型无法处理的复杂决策。

### ✅ Claude Sonnet 4 — 平衡高效的通用模型

- **主打：日常任务中高性能与高效率并存**

- SWE-bench 得分为 72.7%，略高于 Opus 4，特别擅长代码自动化和合理推理。

- 虽整体性能不及 Opus 4，但更加高效、响应更快，适合产品内嵌或即时响应型任务。

应用反馈：

- GitHub Copilot：将以 Sonnet 4 为新引擎，部署到新版智能编程助手。

- iGent：用于多功能自主开发任务，代码导航误差几乎为零。

- Sourcegraph：认为 Sonnet 4 提升了代码质量和任务持续性。

## 新功能亮点

- **支持“工具使用+长期思考”**（beta 版）：
模型可调用搜索等工具进行交替推理，提高回答质量。

- 支持并行使用多个工具，效率提升
![](https://assets-v2.circle.so/qainuoaf7u80fusjdzoov3ckdknv)
**记忆能力大幅提升**：

- 可通过访问本地文件建立“长期记忆”，提取并保留关键事实

示例：Opus 4 在玩宝可梦时，会自动写笔记来记录策略，这些是模型自主生成的真实笔记。
![](https://assets-v2.circle.so/vjxz5oi0kly7t8sn4smsogpzu1b3)**💾 新增“记忆”功能**

- 模型可创建“记忆文件”，用于储存任务关键数据。

- 应用于 AI 代理任务时表现尤为出色，能在连续会话中保持上下文一致性。

**🧮 任务简化与可控思维展示**

- 引入“思维摘要器”，在推理链过长时进行精炼，仅对约 5% 情况使用。

- 开发者可申请“Developer Mode”，查看完整推理轨迹，用于高级 prompt 调试。

## 性能对比与实际验证
📈 **基准测试领先**

- Opus 4 和 Sonnet 4 均在真实软件工程基准（SWE-bench Verified）中居首。

- Opus 4 在多个长时间、多回合推理基准中表现优异，显著超越 Claude 3.7。

- Sonnet 4 虽略逊于 Opus 4，但比 3.7 稳定性与精度大幅提升。
![](https://assets-v2.circle.so/eejtkcv3pr3nra7hbnsh90bshynt)
🧪 **用户反馈验证**

- **Cursor**：最先进的代码模型，深度理解大型代码库。

- **Replit**：多文件修改精度和一致性大幅提升。

- **GitHub Copilot**：将采用 Sonnet 4 驱动其新一代代码代理。

- **iGent / Sourcegraph**：多功能自主开发、错误率接近 0，代码质量提升明显。

## Claude Code 全面上线
00:00UnmuteMuteSettingsCaptionsDisabledQuality1080pSpeedNormalCaptionsGo back to previous menuQualityGo back to previous menu480pSD720pHD1080pHDSpeedGo back to previous menu0.5×0.75×Normal1.25×1.5×1.75×2×4×PIPExit fullscreenEnter fullscreenPlayClaude Code 是为开发者设计的编程助手，现在正式全面开放：
🧰 功能整合与平台兼容

- 支持 GitHub Actions 后台任务处理。

- 原生集成 VS Code 与 JetBrains，模型编辑直接出现在文件中，支持行内注释与变更追踪。

- 可在 IDE 终端中运行 Claude Code，实现“本地 AI 编程伙伴”。

🧪 SDK 与自动化能力

- 发布 Claude Code SDK，可构建自定义 AI 工具和智能代理。

- 示例项目“Claude Code on GitHub”进入 beta 测试，可在 pull request 中：
自动回应评审建议

- 修复 CI 错误

- 修改代码片段

## Anthropic API 推出 AI Agent 构建新能力
Anthropic 正式在其 API 中发布了四项面向 AI 智能代理（agent）开发的新功能。这些功能均已进入公开 beta 阶段，与 Claude Opus 4 与 Sonnet 4 模型共同协作，大幅提升开发者构建智能代理的能力、效率和灵活性。
![](https://assets-v2.circle.so/qj9brzepevpoqlqqjkeawvomxxy5)**代码执行工具**：在 API 层面运行并调试代码。
**MCP 连接器**：连接到多组件工作流或外部服务。
**文件 API**：实现 Claude 与外部文件系统的数据交互。
**Prompt 缓存机制**：prompt 最多缓存1小时，提升性能和一致性。
![](https://assets-v2.circle.so/ulmtz8jkae30re5y6x3x8ltgux8u)
### 四大新功能详细解读
1️⃣ **代码执行工具（Code Execution Tool）**
Claude 不再只是“写代码”，而是能**运行 Python 代码**，具备完整的分析执行能力。

- 在沙箱环境中运行 Python，生成可视化图表与分析报告。

- 可进行：
金融建模（如资产组合分析、预测）

- 科学计算（如模拟与实验数据处理）

- 商业智能（如销售分析、自动报表生成）

- 文档处理（格式转换、数据提取、报表生成）

- 统计分析（如回归、假设检验、预测模型）

📌 **使用政策**：每天免费 50 小时，超出部分按 $0.05/小时/容器计费。
2️⃣ **MCP 连接器（Model Context Protocol Connector）**
这一功能简化了 Claude 连接外部系统的过程，让开发者无需手动编写客户端代码。

- 支持连接至任何远程 MCP 服务，如 Zapier、Asana 等。

- 自动处理以下任务：
连接管理、工具发现、认证与错误处理

- 智能调用远程工具，自动决定调用顺序和参数

**示例**：构建一个项目管理 agent，可以读取 Asana 中的任务、分配工作，并结合代码执行进行数据分析。
![](https://assets-v2.circle.so/z0j0v5pp76wfuccf9mrglb7ha2up)📌 无需手动集成 API，开发效率大幅提升。
3️⃣ **文件 API（Files API）**
这项能力解决了在多轮对话中处理大量文件的效率问题。

- 支持一次上传、多次引用：
无需每轮上传相同文件，适合知识库、技术文档、结构化数据等场景。

文件可被代码执行工具直接访问：

- 如上传一个 CSV 数据集，可持续在多个任务中分析、生成图表、生成摘要等。

📌 减少重复上传和上下文构建成本。
4️⃣ **Prompt 扩展缓存（Extended Prompt Caching）**
优化长期任务或上下文丰富交互的性能与成本：

- 原有缓存 TTL（生存时间）为 5 分钟，现在提供 **1 小时**扩展选项。

- 带来：
**最大 90% 成本下降**

- **最高 85% 延迟降低**

场景包括：

- 多轮工作流

- 分阶段分析或协调任务

- 跨会话保持完整上下文的代理

📌 非常适合需要维护上下文一致性的企业级 Agent 应用。

### 安全与思维透明性

- 模型在复杂任务中减少了 65% 的“捷径”行为。

- 引入“思维总结功能”对仅约 5% 的任务进行摘要，保留更清晰的推理轨迹。

- 提供 Developer Mode 支持高级提示工程（prompt engineering）。

### 产品与定价

- **Opus 4**：输入 $15 / 输出 $75 每百万 token。

- **Sonnet 4**：输入 $3 / 输出 $15，每百万 token。

- 两者均可通过 Anthropic API、Amazon Bedrock 与 Google Cloud Vertex AI 获取。

- Sonnet 4 对免费用户开放；Opus 4 含于 Pro/Max/Team/Enterprise 计划中。

官方介绍：
https://www.anthropic.com/news/claude-4 
https://www.anthropic.com/news/agent-capabilities-api
See more