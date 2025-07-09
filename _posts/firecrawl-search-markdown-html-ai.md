---
layout: post
title: Firecrawl 推出新功能 /search ：可在后台实现搜索 + 抓取网页内容 并返回Markdown、HTML、截图等给AI
date: 2025-06-20
category: Frontier Trends
thumbnail: /style/image/firecrawl-search-markdown-html-ai_1.jpg
icon: game
---
* content
{:toc}

Firecrawl 推出新功能 /search，这是一个专为开发者和 AI 代理打造的网页搜索与抓取接口。用户可以通过一次 API 请求获取搜索结果及其完整内容，返回格式支持 Markdown、HTML、截图等，便于大模型使用。
**功能亮点：**

- **一次 API 调用即可实现搜索 + 抓取网页内容**。

- 在后端直接运行自然语言查询，无需借助浏览器或第三方搜索服务。

- 返回内容格式支持：**Markdown、HTML、纯链接、网页截图**。

- 输出结果对 LLM（大语言模型）友好，便于 AI 处理网页内容。

00:00UnmuteMuteSettingsCaptionsDisabledQuality1080pSpeedNormalCaptionsGo back to previous menuQualityGo back to previous menu480pSD720pHD1080pHDSpeedGo back to previous menu0.5×0.75×Normal1.25×1.5×1.75×2×4×PIPExit fullscreenEnter fullscreenPlay**举个例子：**
你想让一个 AI 去网上搜索“最新 AI 技术”，还要把每个结果的网页内容都提取出来分析。以前你可能需要分两步：
用搜索 API 得到搜索结果
再对每个网址分别抓取内容
现在只需要 **一次调用 /search 接口**，就能：

- 搜索关键词

- 自动抓取每个结果的网页内容

- 得到格式标准、适合 AI 用的数据（比如 Markdown）

## 📌 核心功能
**一体化搜索 + 抓取操作**

- 使用 /search 端点，可在一次调用中进行网络搜索，并可选择抓取搜索结果中的页面内容。

**灵活的结果格式**

- 无论你是在构建 AI 代理（AI agents）、进行深度研究、寻找潜在客户（leads），还是在编程开发中，你都需要**快速获取合适的网页数据**。
使用 /search 接口，你可以一次性获得：
markdown：结构化干净的 Markdown 格式内容；

- html：处理后的 HTML；

- rawHtml：原始 HTML；

- links：页面中提取的链接；

- screenshot / screenshot@fullPage：网页截图（全页或局部）；

- extract：结构化数据抽取。

通过一个视频，展示 /search  通过MCP如何使用的
00:00UnmuteMuteSettingsCaptionsDisabledQuality1080pSpeedNormalCaptionsGo back to previous menuQualityGo back to previous menu480pSD720pHD1080pHDSpeedGo back to previous menu0.5×0.75×Normal1.25×1.5×1.75×2×4×PIPExit fullscreenEnter fullscreenPlay**搜索参数可定制**

- 支持通过参数设置搜索语言（hl）与国家（gl）；

- 时间过滤器支持以下粒度（使用 tbs 参数）：
qdr:h：过去1小时

- qdr:d：过去24小时

- qdr:w：过去一周

- qdr:m：过去一个月

- qdr:y：过去一年

支持设置搜索超时限制。
**响应结构示例**
{
"success": true,
"data": [
{
"title": "Firecrawl - The Ultimate Web Scraping API",
"description": "Firecrawl is a powerful web scraping API...",
"url": "https://firecrawl.dev/",
"markdown": "...",
"links": [...],
"metadata": {
"title": "...",
"description": "...",
"sourceURL": "...",
"statusCode": 200
}
}
]
}

### 🚀 适用场景

- 自动化知识提取

- 搜索结果的结构化整合

- 市场监测和舆情分析

- 内容聚合工具开发

- AI 训练数据构建

详细文档：https://docs.firecrawl.dev/features/search

## Firesearch：AI 驱动的深度网络研究工具
为了展示这个新功能的能力，Firecrawl 还开发了一个开源应用 **Firesearch**，它是一个研究工具，展示了怎么用 /search 来构建一个完整的研究型产品。
**Firesearch** 是一个结合 Firecrawl /search API和 OpenAI GPT-4o 构建的智能搜索工具，可进行多轮、多源的网页信息抓取、分析与整合，适用于复杂问题的研究与问答场景。
![](https://assets-v2.circle.so/z2xprmkyz1zkcm89jsd2lbkbn7b3)
### 🔧 功能亮点
**✅ 智能搜索流程（架构拆解）**
**Query Decomposition**将复杂问题拆解为多个更小、可管理的子问题
**Multi-Search via Firecrawl**每个子问题执行独立搜索，最多生成 12 条搜索请求
**Content Extraction**从每个结果页面中提取 Markdown 内容（使用 scrapeOptions）
**Answer Validation**判断页面内容是否“真正回答了问题”，信度阈值为 0.7+
**Retry Mechanism**未命中时自动更换关键词、调整语义重新查询（最多重试 2 次）
**Answer Synthesis**GPT-4o 将所有命中内容整合为有引用来源的综合答案
00:00UnmuteMuteSettingsCaptionsDisabledQuality1080pSpeedNormalCaptionsGo back to previous menuQualityGo back to previous menu480pSD720pHD1080pHDSpeedGo back to previous menu0.5×0.75×Normal1.25×1.5×1.75×2×4×PIPExit fullscreenEnter fullscreenPlay**📌 高级特性一览**

- ✅ 实时搜索进度更新

- 🔁 自动重试策略：关键词变换、同义词替换、查询重构

- 📎 完整引用：每个答案带网页原始链接

- 🧠 会话记忆：支持上下文追问与多轮查询

- ⚙️ 可配置参数（如最大查询数、最小内容长度、超时等）

### 🧠 核心技术组件
![](https://assets-v2.circle.so/53krff3ol3pyue4r4rngefiuqosx)GitHub：https://github.com/mendableai/firesearch 

## Deep Job Researcher 
**Deep Job Researcher** 是一个基于 **Next.js** 开发的全栈应用，帮助求职者通过上传简历，智能匹配互联网上的职位信息。也是结合了 **Firecrawl** 的 /search 网页抓取能力与 **OpenAI** 的语义分析功能，提供深度个性化的职位推荐。

### 🚀 核心功能
**简历解析**

- 用户上传 PDF 简历；

- 系统通过 OpenAI 模型提取技能、经验和教育背景等关键信息。

**职位匹配**

- 使用 Firecrawl API 进行网络爬虫，抓取真实职位信息；

- OpenAI 对职位描述进行解析，并与简历进行比对打分。

**匹配评分与解释**

- 每个职位附有匹配度评分；

- 提供自然语言解释说明该职位为何适合（或不适合）用户。

**高级过滤器**

- 用户可按职位类型、地区、薪资范围、经验要求等维度筛选结果。
00:00UnmuteMuteSettingsCaptionsDisabledQuality720pSpeedNormalCaptionsGo back to previous menuQualityGo back to previous menu480pSD720pHDSpeedGo back to previous menu0.5×0.75×Normal1.25×1.5×1.75×2×4×PIPExit fullscreenEnter fullscreenPlay
GitHub：https://github.com/mendableai/firecrawl-app-examples/tree/main/deep-job-researcher
See more