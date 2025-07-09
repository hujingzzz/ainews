---
layout: post
title: OpenAI 推出 Deep Research API 并发布o3/o4 mini-Deep-Research 模型 o3、o3-pro 和 o4-mini 现已支持网络搜索
date: 2025-06-10
category: Frontier Trends
thumbnail: /style/image/openai-deep-research-api-o3-o4-mini-deep-research-o3-o3-pro-o4-mini_1.jpg
icon: game
---
* content
{:toc}

Deep Research API 是 OpenAI 提供的高级 API 接口，用于**自动化、结构化和基于真实信息的研究任务**，支持复杂任务的：

- 推理（Reasoning）；

- 规划（Planning）；

- 信息综合（Synthesis）；

- 实时搜索和数据处理（Web Search + Code Interpreter）；

- 引用标注和来源透明（Citation-Backed Reports）；

- 多步骤任务追踪（Agent-like execution tracing）；

它是一个“Agentic Research Pipeline”，提供远超 ChatGPT 的研究控制力。
![](https://assets-v2.circle.so/cbn4lqh4wotyraksqz4xptvq6wtk)OpenAI 还推出了两款专为深度研究任务优化的 API 模型

- **o3-deep-research（06-25）**：基于 o3 模型，适用于需要深入分析和高质量输出的任务，速度较慢。定价为每100万输入代币10美元，每100万输出代币40美元。
![](https://assets-v2.circle.so/qnvinzyitibihf7d8vqueadc3yo5)
- **o4-mini-deep-research（06-25）**：基于 o4-mini 模型，提供更快、更经济的选择，适合对延迟敏感的应用场景。定价为每100万输入代币2美元，每100万输出代币8美元。
![](https://assets-v2.circle.so/70w78ynckh16ngkavly9ala39ggu)
这两款模型能够自动规划子问题，利用网页搜索和代码执行等工具，生成结构化、带有引用的报告，适用于金融、科研、政策分析等领域。
这两个模型是ChatGPT深度研究功能中使用的o3和o4-mini模型的后期训练版本。它们支持高级功能，如MCP（搜索/获取）、代码解释器，并能够从互联网或通过MCP连接器引入的用户数据中合成信息。它们专为复杂的多步骤研究任务设计。
详细：
https://platform.openai.com/docs/models/o3-deep-research 
https://platform.openai.com/docs/models/o4-mini-deep-research

## **网络搜索增强：** 

- o3、o3-pro 和 o4-mini 现已支持网络搜索，允许它们在思维链过程中执行网络搜索。

- **定价**：对于 o3、o4-mini 及其深度研究版本，网页搜索工具的调用费用为每 1,000 次调用 $10

- 4o和4.1模型的网络搜索价格降为每1000次25美元，搜索内容token按模型费率计费（每1,000次调用10美元），加上o3和o4-mini模型的输入代币费率。

- 这使得开发者在使用网页搜索功能时，成本更可控，适合构建需要实时信息获取的应用。

详细：https://platform.openai.com/docs/guides/tools-web-search?api-mode=responses

## 异步事件处理支持 Webhooks
OpenAI API 现已支持通过 Webhooks 进行异步事件处理。
这意味着您可以在以下事件发生时接收实时通知

- 批处理任务完成

- 后台响应生成

- 微调作业完成

通过设置 Webhook，您的系统可以在事件发生时立即获知，无需持续轮询 API，从而提高效率。
详细：https://platform.openai.com/docs/guides/webhooks 

## **活动公告：**
OpenAI DevDay 2025定于2025年10月6日在旧金山举行。
本次活动被认为是迄今为止规模最大的，预计将有超过1,500名开发者参加。
活动将包括直播开幕主题演讲、与最新模型和工具的动手构建环节、多舞台展示和更多演示。
![](https://assets-v2.circle.so/1e71n5fut684tx0a0hu1oe719cln)报名：https://www.devday.openai.com/

### 
See more