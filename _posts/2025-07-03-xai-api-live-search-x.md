---
layout: post
title: xAI 推出网页搜索API：Live Search 可实时动态搜索 X 平台、互联网和新闻等数据源
date: 2025-07-03 12:00:00 +0800
category: Frontier Trends
thumbnail: /style/image/xai-api-live-search-x_1.jpg
icon: design
---
* content
{:toc}

 xAI 推出网页搜索API：Live Search，集成于其 Grok AI 模型，允许通过 API 实时动态搜索 X 平台、互联网和新闻等数据源，从而实现更时效性与准确性的回答。

### 核心功能

- **实时数据搜索**：Grok 可访问 X 帖子、网页和趋势新闻，回答基于最新信息的查询。

- **灵活控制**：开发者可通过 API 设置搜索参数，例如：
启用/禁用搜索（search_parameters.mode）。

- 限制搜索结果数量（max_search_results）。

- 指定时间范围、域名（包括 X 平台）或是否包含引用。

**透明推理**：结合 DeepSearch 功能，Grok 可展示搜索和推理过程，提供清晰的答案来源。

### 使用方式

- **API 访问**：xAI 提供 Live Search API，**目前处于免费 Beta 阶段（截至 2025 年 6 月 5 日）**。开发者可通过 xAI 官网（x.ai/api）获取 API 密钥并开始构建应用。

- **Python SDK**：支持通过 Python 集成，需设置 XAI_API_KEY 环境变量并安装 SDK。

- **GUI 工具**：社区开发的 Python 应用（如 xAI Live Search App）提供图形界面，方便测试和交互。

### 应用场景

- **实时信息查询**：如新闻摘要、社交媒体动态或市场趋势。

- **研究辅助**：快速汇总多源数据，支持学术或商业分析。

- **开发者创新**：构建基于实时数据的 AI 应用，如聊天机器人或信息聚合工具。

![](https://assets-v2.circle.so/t3d3brramkgact4ubme7f00pr0yv)
## 工作机制

### ✅ 核心优势

- 无需用户手动管理搜索逻辑或工具链调用；

- 模型内部可自主决定是否搜索、何时搜索、搜索什么；

- 支持限定数据来源、日期范围、地区、数量等参数定制。

### 📥 开启方式
在 chat completions 请求中添加字段：
"search_parameters": {
"mode": "on" / "auto" / "off"
}![](https://assets-v2.circle.so/roc5lmfiu4eazyhex4o6rll0d6ei)🌐 可接入的数据源类型（通过 sources 字段指定）
![](https://assets-v2.circle.so/zbgvky8i40gicgmor357yibhyquq)示例：允许模型查找新闻+X 平台内容：
"sources": [
{ "type": "news" },
{ "type": "x" }
]⚙️ 高级参数配置支持
![](https://assets-v2.circle.so/9hclggzg6ilg9c8ooouica1jkl9c)
## 📤 输出行为说明

- 在流式响应（streaming）中，citations 字段只在最后一段（chunk）返回；

- 所有请求结构支持 Python requests 示例调用。

payload = {
"messages": [{"role": "user", "content": "What's trending in tech news today?"}],
"search_parameters": {
"mode": "auto",
"sources": [{"type": "news"}],
"return_citations": True,
"from_date": "2025-05-20",
"to_date": "2025-05-21"
},
"model": "grok-3-latest"
}访问：https://docs.x.ai/docs/guides/live-search
See more