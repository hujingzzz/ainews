---
layout: post
title: DeepSeek 发布DeepSeek R1-0528：代码能力和写作能力显著提升、推理能力更深层次 同时修复了一些问题
date: 2025-07-09
category: Frontier Trends
thumbnail: /style/image/deepseek-deepseek-r1-0528_1.jpg
icon: book
---
* content
{:toc}

DeepSeek 发布**DeepSeek R1-0528更新，**昨晚向微信技术群体通报此次更新为“**小规模试验性升级**”，并已开放测试。

## **DeepSeek R1-0528 更新亮点**

### 1. 深度思考能力大幅提升
DeepSeek-R1-0528 仍然使用 2024 年 12 月所发布的 DeepSeek V3 Base 模型作为基座，但在后训练过程中投入了更多算力，显著提升了模型的思维深度与推理能力。
更新后的 R1 模型在数学、编程与通用逻辑等多个基准测评中取得了当前国内所有模型中首屈一指的优异成绩，并且在整体表现上已接近其他国际顶尖模型，如 o3 与 Gemini-2.5-Pro。
![](https://assets-v2.circle.so/vuglp8rxg0u64wag0atpvqle7cbo)
- **技术背景**：虽然仍基于 DeepSeek V3 Base，但本次通过增强后训练过程中的算力资源投入，实现了模型在**推理链条中的显著增强**。

- **AIME 2025 测评结果**：
旧版准确率：70%

- 新版准确率：**87.5%**

**Token 使用对比**（每题）：

- 旧版：12K

- 新版：23K👉 表明新版能“更慢更深地思考”，模拟人类详细推理路径。

### 2. 思维链蒸馏至中等规模模型
通过蒸馏 DeepSeek-R1-0528 的思维链后训练 Qwen3-8B Base，得到了 DeepSeek-R1-0528-Qwen3-8B。该 8B 模型在数学测试 AIME 2024 中仅次于 DeepSeek-R1-0528，超越 Qwen3-8B （+10.0%），与 Qwen3-235B 相当。**我们相信，DeepSeek-R1-0528 的思维链对于学术界推理模型的研究和工业界针对小模型的开发都将具有重要意义。**

- 基于 R1-0528 蒸馏出 **Qwen3-8B Base 版本**。

- 新模型在 AIME 2024 中性能优于 Qwen3-8B，接近 Qwen3-235B。

- 表明蒸馏后的“思维链”具备极高学术与工业价值。
![](https://assets-v2.circle.so/4cexjbe4m88sxtx2f6vvsuy500ix)

### 3.写作能力增强

- 对生成性写作能力做了微调优化。

- 支持结构更完整、风格更贴近人类的长文本输出。

- 尤其针对**议论文、小说、散文等复杂文体**输出能力有实质增强。
![](https://assets-v2.circle.so/6mzro4d69k59nldzrm3ifow3qg3s)

### 4.误差控制与“幻觉率”下降

- **幻觉优化目标**：减少模型输出中“无中生有”的内容。

- **适用场景**：
改写润色

- 阅读理解

- 摘要总结

**性能提升数据**：

- 幻觉率降低：**约45%~50%**

- 输出更加可信，信息一致性提升

### 5.工具调用与代码能力增强

- 新版支持 **Function Calling** 与 **JsonOutput**。

- **Tau-Bench评估成绩**：
Airline: 53.5%

- Retail: 63.9%

- 水平接近 OpenAI o1-high，但略逊于 o3-high、Claude 4 Sonnet。

![](https://assets-v2.circle.so/e1l6gsyx43pif5lhj3zgsj4dvc0w)**前端代码生成能力提升**，并提升在“角色扮演”等多轮对话复杂任务中的表现。
![](https://assets-v2.circle.so/bxpxjz9ciei6lh55cubt38kevpxp)
### 6️⃣ 🛠 **问题修复与优化**

- 修复早期 R1 模型的常见问题：
**重复回答**问题

- **格式混乱**

- **语言混用（中英夹杂）**

输出更规范，**适合专业场景使用**。

### 多任务能力优化表现
![](https://assets-v2.circle.so/gtq5ems4nbbww7f0el57rexhbefe)
- **Benchmark 评测**：在由 UC Berkeley、MIT 和 Cornell 开发的 **LiveCodeBench** 代码生成评测中：
R1-0528 的推理能力与 **OpenAI 的 o3**等前沿模型性能相当，略低于**o4 mini**，尤其在数学、编程和复杂推理任务上表现出色。

- **优于 xAI 的 Grok 3 mini 和阿里巴巴的 Qwen 3**。

推理行为更深思熟虑，链式推理（Chain-of-Thought, CoT）结构更清晰，输出格式更自然。
该成绩进一步增强了 DeepSeek 在中美 AI 技术竞争中的影响力。
![](https://assets-v2.circle.so/io4j1766fe2nu4razu7azekgbtz0)DeepSeek已将 R1-0528 上传至 Hugging Face，但尚未发布公开说明或模型描述。

## **API 更新****​**
API 已同步更新，接口与调用方式保持不变。新版 R1 API 仍支持查看模型思考过程，同时还增加了 Function Calling 和 JsonOutput 的支持。
我们对新版 R1 API 中 max_tokens 参数的含义做了调整：现在 max_tokens用于限制模型单次输出的总长度（包括思考过程），默认为 32K，最大为 64K。请 API 用户及时调整 max_tokens 参数以防输出被提前截断。
R1 模型的使用方法详见 API 指南：https://api-docs.deepseek.com/zh-cn/guides/reasoning_model。
本次 R1 更新后，官方网站、小程序、App 端和 API 中的模型上下文长度仍为 64K。如果用户对更长的上下文长度有需求，可以通过其他第三方平台调用上下文长度为 128K 的开源版本 R1-0528 模型。

## **模型开源****​**
DeepSeek-R1-0528 与之前的 DeepSeek-R1 使用同样的 base 模型，仅改进了后训练方法。私有化部署时只需要更新 checkpoint 和 tokenizer_config.json（tool calls 相关变动）。模型参数为 685B（其中 14B 为 MTP 层），开源版本上下文长度为 128K（网页端、App 和 API 提供 64K 上下文）。
DeepSeek-R1-0528 模型权重下载请参考：
**Model Scope:** https://modelscope.cn/models/deepseek-ai/DeepSeek-R1-0528
**Huggingface:** https://huggingface.co/deepseek-ai/DeepSeek-R1-0528
与旧版本的 DeepSeek-R1 保持一致，此次我们的开源仓库（包括模型权重）仍然统一采用 MIT License，并允许用户利用模型输出、通过模型蒸馏等方式训练其他模型。

## **最新调用Deepseek-R1-0528 API 的网站**
1、Openrouter 地址：https://openrouter.ai
2. GMI tutt: https://inference-engine.gmicloud.ai
3. Novita tutt: https://novita.ai
4. Nebius tbtit: https://studio.nebius.com
5. Inference toti: https://inference.net 
官方介绍：https://api-docs.deepseek.com/zh-cn/news/news250528
See more