---
layout: post
title: Mistral AI 推出其首个专注推理的开源模型 Magistral Flash Answers 模式下 推理速度比竞争对手快10倍
date: 2025-06-22
category: Frontier Trends
thumbnail: /style/image/mistral-ai-magistral-flash-answers-10_1.jpg
icon: game
---
* content
{:toc}

Mistral AI 宣布推出其首个专注推理的语言模型 **Magistral**，旨在解决当前主流 LLM 在以下方面的不足：

- **缺乏领域知识深度**，在专业任务（如金融建模、法律分析）中表现不佳。

- **推理不透明**，用户难以追踪模型得出结论的逻辑。

- **多语言推理能力薄弱**，尤其在非英语语言中表现不一致。

- **缺乏链式思维支持（Chain-of-thought, CoT）**，使复杂问题难以解决。

Magistral 试图构建一个“**能像人类一样思考**”的 AI——具有结构化、可验证、逐步推理的能力，同时支持多语言使用。
![](https://assets-v2.circle.so/1ktkb1h1bolve7kykg6lziw7jov1)**模型版本**

- **Magistral Small**：24B 参数的开源版本（Apache 2.0协议），可在 Hugging Face 上下载。

- **Magistral Medium**：功能更强大的企业版本，可通过 Le Chat、La Plateforme API、Amazon SageMaker 访问，未来将上线 IBM WatsonX、Azure AI 和 Google Cloud。
![](https://assets-v2.circle.so/d9isxzj5h8mg9stwlq2byyztu1hv)
多数投票（majority voting @64）是通过多个生成版本得出最一致答案，表示在多样性与一致性之间平衡的能力。
Medium 模型达到 **90%** 的准确率，接近顶级闭源模型 GPT-4 Turbo 的水平，尤其在专业任务中表现突出。
![](https://assets-v2.circle.so/n8dfxejaje6qu3aic4d6o4fkane9)
- 在**复杂逻辑任务、跨领域问答、可解释推理**方面非常突出；

- 在**专业场景（法律、科技、学术）**中已具备实用性；

- 在同体量开源模型（20B～30B）中是**推理能力最强的一批**。

## 核心技术与架构亮点
**1. 🧩 Chain-of-Thought 原生支持**
Magistral 原生支持链式思维（CoT），并能**自动生成可解释的思维链条**。这对于复杂任务（如法律推理、系统规划）尤其关键。
**推理优化设计（Reasoning-Oriented）**

- 模型专门针对“多步骤逻辑推理”进行了微调。

- 支持“内在思考路径（inner monologue）”生成，可呈现完整的推理轨迹。

- 输出格式采用 <think>...</think> 来区分草稿与总结，提高可解释性。

**2. 🌍 多语言高保真推理**
模型具备多语言推理能力，特别优化了以下语言：

- 英语、法语、德语、西班牙语、意大利语

- 阿拉伯语、俄语、简体中文

→ 关键点：不仅支持多语言输入/输出，而且**推理链条也能在目标语言中自然生成**。
**3. ⚡ Flash Answers + Think Mode（仅限企业版）**
通过“Le Chat”平台，Magistral Medium 可开启：

- **Flash Answers**：10 倍于主流竞品（如 ChatGPT）的推理速度。

- **Think Mode**：优化多轮推理响应时间与效率。

- 🧠 实际表现：
在结构化任务（例如决策树推理、逻辑证明、代码规划）中几乎“秒出”结果；

- 同时保持了准确率与逻辑严谨性。

**4. 🔍 推理透明性与可追溯性**
每一个生成结果都附带清晰的“思考轨迹”，可以追踪、审计。特别适合监管行业（法律、金融、医疗等）。

## 开源、可本地部署

- 模型已开源，支持商业用途。

- 量化后可运行在单张 RTX 4090 或 MacBook M2（32GB）上。

- 提供多个平台支持，包括：
vLLM（推荐）

- llama.cpp 版本（GGUF）

- 支持 lmstudio、ollama、unsloth、Axolotl 等工具链

** Chat 模板（推荐使用）**
使用默认的系统提示词（system prompt）可获得最佳推理效果：
[SYSTEM_PROMPT]
你应该先展示思考过程（inner monologue），再给出一个清晰的答案总结。
你的回答必须使用与用户相同的语言。
请使用 Markdown 格式输出。
## 应用推荐场景
![](https://assets-v2.circle.so/sfrhxje1qvzfh4rdqcxk11zeym1k)官方介绍：https://mistral.ai/news/magistral
模型下载：https://huggingface.co/mistralai/Magistral-Small-2506
在线体验：https://chat.mistral.ai/chat
See more