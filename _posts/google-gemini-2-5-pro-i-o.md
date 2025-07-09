---
layout: post
title: Google 发布了 Gemini 2.5 Pro（I/O 预览版）提升了编码等相关能力，尤其在前端开发方面
date: 2025-06-25
category: Frontier Trends
thumbnail: /style/image/google-gemini-2-5-pro-i-o_1.jpg
icon: note
---
* content
{:toc}

Google 发布了 **Gemini 2.5 Pro（I/O 预览版）**，这是一版专为即将到来的 Google I/O 大会提前发布的模型更新，重点提升了编码相关能力，尤其在前端开发、UI构建、函数调用、视频理解结合代码生成等方面。

## 主要更新：

- **代码能力显著提升**
更好地支持函数调用、模块重构、逻辑判断

- 具备“类资深开发者”的架构理解力

**前端与 UI 开发能力升级**

- 排名 WebDev Arena 第一

- 自动生成美观、结构清晰的网页组件（含 CSS、响应式布局）

- 能识别设计样式并保持风格一致性

**视频理解 + 代码生成融合**

- 视频内容 → 交互式应用（基于 YouTube 内容）

- 多模态 AI 能力增强（VideoMME 评分 84.8%）

**构思到应用落地速度更快**

- 从简单提示快速生成具 UI + 动效的可用 App

- 示例项目：Dictation Starter App

**开发体验优化**

- 错误率降低、函数触发率提升

- 与旧版接口兼容、价格不变、无缝升级

00:00UnmuteMuteSettingsCaptionsDisabledQuality1080pSpeedNormalCaptionsGo back to previous menuQualityGo back to previous menu480pSD720pHD1080pHDSpeedGo back to previous menu0.5×0.75×Normal1.25×1.5×1.75×2×4×PIPExit fullscreenEnter fullscreenPlay
## 详细升级介绍

### 1. 🚀 **代码能力升级**

- 更强的代码生成与重构能力：
在涉及复杂后端重构任务的评测中，**首次成功通过 Cognition 的高级开发者评测用例**，展示出“类资深开发者”水平的抽象与结构选择能力；

- 适用于复杂业务逻辑调整、模块化设计、API重写等任务。

更可靠的函数调用能力（Function Calling）：

- **错误率下降，触发率提升**，开发者可以更流畅地构建基于多步骤函数组合的“Agentic Workflow”；

- Gemini API 接入的开发者无需迁移，系统自动切换到新版。
![](https://assets-v2.circle.so/stwflwumgauuv5eg4mt3yjmvu57o)

### 2. 🧑‍💻 **前端开发支持全面增强**
Gemini 2.5 Pro 在前端开发领域已跃居 **WebDev Arena 排名第一**（衡量人类偏好度的排行榜）。
![](https://assets-v2.circle.so/0k7vhicgwgv2nwefdl3g8e644ctg)可用于以下典型任务：

- 将设计图转为实际网页组件（HTML + CSS + JS）；

- 快速生成 UI 组件并自动适配现有样式；

- 理解按钮交互、字体、边距、动画等视觉元素，并还原成高质量网页；

- 模仿现有应用风格实现新功能（如将视频播放器嵌入现有网页）。

🎯 示例：在 Gemini 95 Starter App 中，开发者只需描述“想要增加一个样式统一的视频播放器”，Gemini 就能自动读取已有设计风格并生成可用组件。

### 3. 🎥 **视频+代码：多模态能力进一步融合**

- 在 VideoMME 基准上得分高达 **84.8%**，是目前领先的“视频理解大模型”之一；

- 可基于一段 YouTube 视频，**自动生成交互式学习 App**，包括内容提取、界面构建与逻辑生成；

- 代表 AI 正从“语言驱动代码”进化为“视频驱动产品”的多模态阶段。

📌 示例：Google AI Studio 的 Video to Learning App 演示了这种新能力。

### 4. ✨ **“从构思到产品”的开发流程加速**
借助 Gemini 2.5 Pro，开发者能快速将一个产品想法实现为具备完整功能与视觉质量的 App。
示例产品：“Dictation Starter App”：

- 自动生成**麦克风动画、响应式布局、按钮悬停特效**；

- 不仅满足功能需求，视觉表现也高度专业；

- 表明模型具备基础审美感知与产品意识。

现在你可以通过 Google AI Studio 中的 Gemini API 选择 Gemini 2.5 Pro（05-06） 进行构建应用，企业客户可以使用 Vertex AI 构建。

- 目前 Gemini 2.5 Pro 预览版以与旧版（03-25）**相同的价格开放使用**；

- 系统已默认将接口指向新版（05-06），开发者无需额外迁移；

- 模型卡已同步更新，记录各项升级细节。

See more