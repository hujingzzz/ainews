---
layout: post
title: OpenAI 发布了四项重大更新 提升了构建 AI 代理能力 新增TypeScript 支持、人类干预机制、新语音模型
date: 2025-06-16 12:00:00 +0800
category: Frontier Trends
thumbnail: /style/image/openai-ai-typescript_1.jpg
icon: link
---
* content
{:toc}

OpenAI 发布了四项重大更新，提升了构建 AI 代理，尤其是语音代理的能力。现在，开发者可以使用 TypeScript 编写 Agents SDK，同时支持人类审批机制，增强了控制力和安全性。新推出的 RealtimeAgent 让语音代理在客户端或服务端轻松运行，具备高级音频处理能力。
Traces 仪表盘也升级了，支持 Realtime API 的语音交互可视化，为调试和分析提供便利。speech-to-speech 模型进行了大幅优化，提升了指令遵循性、工具调用准确性，并可调节语音播报速度。
**Key points**

- **Agents SDK 新增 TypeScript 支持**：具备与 Python 版相同的核心功能（handoffs、guardrails、tracing、MCP 等）。

- **人类审批流程**：允许在工具调用中加入“人类审查”机制，可暂停执行、保存状态、审核并恢复。

- **RealtimeAgent 功能发布**：可在客户端或服务器上构建语音代理，支持工具调用、音频处理、打断等。

- **Traces 仪表板升级**：支持 Realtime API 语音会话可视化，包括输入输出音频、调用过程、打断记录。

- **Speech-to-speech 模型改进**：
更好地遵循指令

- 更稳定的工具调用

- 更合理的中断行为

- 新增 speed 参数可控制语速

**新模型版本发布**：

- gpt-4o-realtime-preview-2025-06-03（用于 Realtime API）

- gpt-4o-audio-preview-2025-06-03（用于 Chat Completions API）

### 🔧 **1. Agents SDK 支持 TypeScript（开发工具更新）**
**说明**：

- OpenAI 的 Agents SDK 现在不仅支持 Python，还新增了 TypeScript 版本。

- 与 Python 版本等效，支持所有主要构建代理所需的“原语”（primitives）：
✅ handoffs：多代理间的任务接力与转移✅ guardrails：行为安全约束和限制✅ tracing：代理执行过程的日志记录与分析✅ MCP（多组件代理架构）

**意义**：

- 面向 Web 和 Node.js 生态系统的开发者更友好。

- 易于集成到 JavaScript 应用中，比如浏览器端语音助手、网页智能客服等。
![](https://assets-v2.circle.so/gdishg1cqd400xq3406xlph17wgv)

### 👤 **2. 支持“**人类审查**”（Human-in-the-loop）机制**
**说明**：

- 在代理调用外部工具（如函数、API）之前，允许人工审批。

- 支持以下操作流程：
**暂停工具执行**

- **序列化并保存代理状态**

- **审核该工具调用（接受或拒绝）**

- **恢复代理执行**

**意义**：

- 可用于高风险、敏感任务中的人工干预（如财务、医疗、客服投诉处理等）。

- 提高系统可靠性、合规性和透明度。

### 🔊 **3. RealtimeAgent 功能：构建语音代理的新方式**
**说明**：

- RealtimeAgent 是一个基于 Realtime API 构建语音交互代理的高层功能。

- 可在客户端或服务器端运行，支持：
工具调用（function calling）

- 会话交接（handoffs）

- 安全护栏（guardrails）

- 自动音频处理（播放、暂停、打断）

- 实时语音输入和响应

**意义**：

- 允许开发者像构建文本代理一样定义语音代理。

- 可打造如 AI 电话客服、语音搜索助手、语音角色扮演等应用。
![](https://assets-v2.circle.so/80bug2ystk2lzhe9qr4531km9gyq)

### 📊 **4. Traces 仪表盘升级：支持语音会话可视化**
**说明**：

- Traces 是用于调试和监控代理运行过程的工具。

- 现在可支持 Realtime API 中的语音代理运行细节，包括：
✅ 用户语音输入和模型语音输出✅ 工具调用和参数✅ 中断点（如用户打断）

**意义**：

- 更直观的调试体验，更清晰的问题定位。

- 帮助开发者优化语音交互设计，提高产品稳定性。
00:00UnmuteMuteSettingsCaptionsDisabledQuality1080pSpeedNormalCaptionsGo back to previous menuQualityGo back to previous menu480pSD720pHD1080pHDSpeedGo back to previous menu0.5×0.75×Normal1.25×1.5×1.75×2×4×PIPExit fullscreenEnter fullscreenPlay

### 🧬 **5. 语音模型 GPT-4o 功能升级**
**说明**：

- speech-to-speech（语音到语音）模型进行了核心升级：
**更可靠地执行用户指令**

- **更一致的工具调用行为**

- **更智能地处理中断和语速调节**

新增 speed 参数，可以控制语音播放速度（如慢速朗读、快速播报）
**模型版本**：

- 在 Realtime API 中可用版本：gpt-4o-realtime-preview-2025-06-03

- 在 Chat Completions API 中的版本：gpt-4o-audio-preview-2025-06-03

### **多个合作方的实战案例**
✅ **Perplexity AI**：

- 使用 Realtime API 构建语音问答助手。

- 得益于新模型，其工具调用更精准，用户体验更流畅自然。
00:00UnmuteMuteSettingsCaptionsDisabledQuality720pSpeedNormalCaptionsGo back to previous menuQualityGo back to previous menu480pSD720pHDSpeedGo back to previous menu0.5×0.75×Normal1.25×1.5×1.75×2×4×PIPExit fullscreenEnter fullscreenPlay
✅ **Intercom（Fin Voice）**：

- 构建电话 AI 客服，支持全天候自动接听。

- 新模型能更好地遵循脚本，减少“幻觉式”回答，提升服务质量。
00:00UnmuteMuteSettingsCaptionsDisabledQuality1080pSpeedNormalCaptionsGo back to previous menuQualityGo back to previous menu480pSD720pHD1080pHDSpeedGo back to previous menu0.5×0.75×Normal1.25×1.5×1.75×2×4×PIPExit fullscreenEnter fullscreenPlay
✅ **Volley Games**：

- 构建基于 AI 地牢主的 RPG 游戏体验。

- 新模型表现出更强的“规则意识”和更富想象力的叙事能力。

相关链接：
https://openai.github.io/openai-agents-js/ 
https://openai.github.io/openai-agents-js/guides/human-in-the-loop/
See more