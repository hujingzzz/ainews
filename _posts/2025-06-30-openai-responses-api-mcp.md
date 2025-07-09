---
layout: post
title: OpenAI Responses API 功能大升级：支持图像生成、代码解释器、远程 MCP 等新工具
date: 2025-06-30 12:00:00 +0800
category: Frontier Trends
thumbnail: /style/image/openai-responses-api-mcp_1.jpg
icon: web
---
* content
{:toc}

OpenAI 宣布对 **Responses API** 进行重大功能扩展，面向开发者开放更多模块化的能力，使构建多模态、复杂任务链的 AI 应用变得更容易、更可控、更强大。
Responses API 主要用于**构建智能体（agentic applications）**，也就是具备“自主思考 + 工具调用”能力的智能应用。
**📦 它与传统 ChatGPT API 有什么区别？**
![](https://assets-v2.circle.so/8ugtnecd6as5d6n7fuyln3hbxkvl)
## ⚙️ 它能做什么？
**✅ 基础功能**

- 回答问题、聊天、写作、摘要等（类似 ChatGPT API）

**🔧 新增“工具调用”能力（Tool Calling）**
可以让 AI 自动调用以下工具：

- 🔍 Web搜索：实时查找最新信息

- 📂 文件搜索：查找并分析用户上传的文件

- 💻 Code Interpreter：运行代码、画图、算数学题

- 🖼 图像生成工具：根据文字生成图片

- 🌐 远程 MCP 工具：连接其他系统（如 Stripe、Shopify、Twilio 等）

**🧠 强化的“智能思维”**

- 模型可以进行“链式思考”（Chain of Thought），在一个回答中多步推理、分阶段调用工具。

- 支持 **Reasoning Summary**：查看模型是怎么一步步得出答案的。

**⏱ 后台模式（Background Mode）**
可以让 AI 异步完成复杂任务（比如长时间的搜索、分析、绘图），不怕超时断连。

### 🧪 举个例子：Responses API 的用法
你可以用 Responses API 构建一个“财务顾问 AI”，它能做：
读取你上传的 Excel 报表（通过文件搜索）；
分析数据并生成图表（通过 Code Interpreter）；
搜索最近的财经新闻（通过 Web search）；
最后输出一份专业的财务分析报告。
你只需调用一次 API，它会自动分阶段完成所有任务。

## 🧩 新增功能一览：

### 1. ✅ **远程 MCP（Model Context Protocol）服务器支持**

- 现在开发者可以将上下文（Context）从本地扩展到远程 MCP 服务

- 通过几行代码将模型连接至任何 MCP 服务器托管的工具。

- 有利于构建大型、多源、分布式 AI 应用

- 使上下文构建更模块化、更安全、可共享

- OpenAI 也加入了 MCP 的 steering committee，推进协议发展。

- 支持的 MCP 供应商包括：Cloudflare、Stripe、Twilio、Shopify、PayPal、Zapier 等。
![](https://assets-v2.circle.so/d8ahy7o3kc02n7qgjcvekmm08flf)![](https://assets-v2.circle.so/kvuse3uufh4ro1kyr16xukbw133d)

### 2. 🖼️ **图像生成功能接入 Responses API**

- gpt-image-1 模型图像生成可作为工具与语言模型协作使用

- 将 gpt-image-1 模型作为内建工具，支持实时预览与多轮编辑。

- 开发者可直接在推理过程中调用图像生成，并逐步优化结果。

- 支持**流式预览图像**：生成过程可实时可视化

- **支持多轮图像编辑**：逐步细化图像细节，适合创意场景
00:00UnmuteMuteSettingsCaptionsDisabledQuality1080pSpeedNormalCaptionsGo back to previous menuQualityGo back to previous menu480pSD720pHD1080pHDSpeedGo back to previous menu0.5×0.75×Normal1.25×1.5×1.75×2×4×PIPExit fullscreenEnter fullscreenPlay

### 3. 🧮 **Code Interpreter（高级代码工具）接入 Responses API**

- 可通过 Responses API 使用，可进行数据分析、图像处理、复杂数学与编程问题求解。

- 用于：
数据分析

- 数学运算

- 编程计算

- **图像理解任务**（如“看图思考”）

支持 OpenAI o3 和 o4-mini，提升链式推理能力（Chain-of-Thought）
📎 官方说明

### 4. 📂 **文件搜索支持上线**

- 可通过推理模型查找相关文档段落（chunk）

- 支持：
**两个向量数据库同时搜索**

- **属性过滤（Array-based Attribute Filtering）**

📎 查看文件搜索示例

### 5. ⚙️ **新增开发者辅助功能**

- **🔙 Background mode**运行异步任务，无需阻塞当前请求📎 说明文档

- **🧠 Reasoning Summaries**快速查看模型内部推理路径，便于调试和评估

- **🔐 Encrypted Reasoning Items**允许在 ZDR（Zero Data Retention）组织中跨请求重用推理项📎 更多说明

## 💰 价格与可用性
![](https://assets-v2.circle.so/5d3nio1529mzyc1mvy8wlya65rlw)支持模型：GPT-4o 系列、GPT-4.1 系列、OpenAI o1/o3/o4-mini 系列。图像生成功能仅在 o3 中支持。
官方介绍：https://openai.com/index/new-tools-and-features-in-the-responses-api/
See more