---
layout: post
title: Google I/O 2025 大会Gemini API 更新大汇总 一文了解Gemini API 都做了哪些更新升级
date: 2025-06-05
category: Frontier Trends
thumbnail: /style/image/google-i-o-2025-gemini-api-gemini-api_1.jpg
icon: image
---
* content
{:toc}

Google 在 I/O 2025 上发布了对 **Gemini API 和 Google AI Studio** 的一系列重要更新，涵盖模型能力扩展、音频与视频输入支持、思维过程可视化、浏览器自动化控制等新功能。
这些更新显著提升了开发者在构建文本、图像、音频、视频、多模态代理方面的能力。
**Gemini API** 已逐步发展为一个完整的多模态智能平台，适用于从代码生成到音频对话、从网页信息提取到浏览器操作控制的广泛场景。允许开发者调用其最先进的文本、图像、音频和视频模型。此次更新聚焦于以下方面：
**新模型与语音能力升级**
**实时音乐生成**
**多模态输入增强（视频理解等）**
**开发工具与API结构更新（如思维摘要、浏览器控制、异步函数调用）**
**为开发者提供更高效、经济的模型访问方式（如批处理 API）**
![](https://assets-v2.circle.so/kv57tyr4qmzos3g0w0zuwddvnt3o)
## 模型更新与能力拓展

### 🧠 1. Gemini 2.5 Flash Preview 新模型

- **版本标识：** gemini-2.5-flash-preview-05-20

- **性能改进：** 在逻辑推理、代码生成、长上下文处理方面超过前代。

- **评测成绩：** 在 LMarena 榜单中排名第二，仅次于 Gemini 2.5 Pro。

- **效率提升：** 评估显示 token 使用效率提高了 **22%**。

### 🔊 2. Gemini 2.5 Pro & Flash TTS（文本转语音）

- **支持语言：** 超过 **24种语言**。

- **支持类型：** 单一发声人、多发声人（multi-speaker），支持**情绪、语气控制**。

- **应用场景：** 创建拟人化AI角色、多轮语音对话代理、音频内容创作等。

### 🗣️ 3. Gemini 2.5 Flash 原生语音对话模型

- **功能特性：**
提供30种不同声音风格

- 自动识别背景与说话者区分

- 响应用户语调/情绪变化

- 使用“思考模型”进行复杂逻辑处理

**适用场景：**

- 呼叫中心智能代理

- 多角色语音故事

- 带语气的个性语音助手

### 🎵 4. Lyria RealTime：实时音乐生成

- **工作原理：** 通过 WebSocket 建立实时流式连接，模型持续生成音乐片段。

- **控制方式：** 文本提示控制生成风格与节奏。

- **应用示例：** Google AI Studio 中的 PromptDJ-MIDI 示例应用。

### 🧮 5. Gemini 2.5 Pro Deep Think（深度思维模式）

- **用途：** 实验性功能，用于处理**复杂数学与编程问题**。

- **表现：** 推理链更长，精度更高，适用于高级代码生成和逻辑求解。

### 💡 6. Gemma 3n（轻量多模态模型）

- **部署平台：** 适用于手机、笔记本、平板等边缘设备。

- **支持模态：** 文本 + 音频 + 图像。

- **技术架构：**
**PLE参数缓存**：按层缓存减少推理负担。

- **MatFormer架构**：降低计算与内存开销。

## API 功能增强与开发者工具

### 🧠 1. 思维摘要（Thought Summaries）

- **用途：** 提取模型在推理时的中间想法（chain-of-thought），帮助开发者理解模型思维路径。

- **展示方式：**
标题分类

- 工具调用链展示

- 与最终回答并列展示

**代码示例（Python）：**
from google import genai
from google.genai import types
client = genai.Client(api_key="GOOGLE_API_KEY")
prompt = "What is the sum of the first 50 prime numbers?"
response = client.models.generate_content(
model="gemini-2.5-flash-preview-05-20",
contents=prompt,
config=types.GenerateContentConfig(
thinking_config=types.ThinkingConfig(
thinking_budget=1024,
include_thoughts=True
)
)
)
for part in response.candidates[0].content.parts:
if part.thought:
print("Thought summary:\n", part.text)
else:
print("Answer:\n", part.text)

### ⚖️ 2. 思考预算（Thinking Budgets）

- **功能：** 控制模型在生成内容时“思考”的深度，以平衡准确率、延迟与成本。

- **应用：** 可限制 token 使用量，适用于低延迟场景。

### 🔗 3. URL Context 工具

- **说明：** 模型可从指定网页自动获取相关上下文信息。

- **组合使用：** 可与 Google Search grounding 工具协同使用，增强研究型代理能力。

- **使用方式：**

tools = [
Tool(url_context=types.UrlContext),
Tool(google_search=types.GoogleSearch)
]
response = client.models.generate_content(
model="gemini-2.5-flash-preview-05-20",
contents="Give me a 3-day schedule based on YOUR_URL...",
config=GenerateContentConfig(tools=tools)
)

### 🌐 4. 浏览器自动化控制（Project Mariner）

- **功能：** 控制浏览器行为，如点击按钮、滚动页面、填表等。

- **部署方式：** 可一键在 Cloud Run 部署浏览器代理。

- **合作企业：** UiPath、Browserbase、Automation Anywhere 等已参与早测。

### 📼 5. 视频理解更新

- **输入支持：** YouTube 视频链接、直接上传视频。

- **支持功能：**
视频总结、分析、翻译

- 视频裁剪（提取片段分析）

- 可变帧率（0.1 ~ 60 FPS）支持游戏/体育等高帧内容

- 分辨率控制：720p / 480p / 360p

### ⚙️ 6. 异步函数调用（Async Function Calling）

- **新特性：** 在 Live API 中实现异步调用，不阻塞对话主流程。

- **设置方式：** 在函数定义中将 behavior 字段设为 NON_BLOCKING。

### 🧾 7. 批处理 API（Batch API）

- **功能：** 支持将多个请求批量发送，最长24小时返回结果。

- **优势：**
成本为交互API的一半

- 提供更高速率限制

**适用场景：** 大规模分析、批量文档处理、离线评估等。

## 总的来说：

### ✅ Gemini API 的新能力使其成为一个：

- 真正多模态的统一接口

- 适用于轻量到重载各种设备

- 涵盖音频、视频、图像、网页、文本等复杂交互场景

- 支持更透明可控的模型输出与思维调试

**开发者可以：**

- 快速原型测试

- 构建可商用的智能代理

- 集成语音、视频、图像等输入输出

- 使用工具调度和自动化控制接口创建智能工作流

### 🧩 推荐场景：

- 构建语音对话机器人

- 开发视频内容摘要工具

- 音乐生成创作应用

- 浏览器自动化测试工具

- 研究型 AI 信息代理

原文：https://developers.googleblog.com/en/gemini-api-io-updates/
📚 查看开发者文档以获取更多示例代码与API指南：https://ai.google.dev
See more