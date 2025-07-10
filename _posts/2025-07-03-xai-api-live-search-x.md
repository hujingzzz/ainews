---
layout: post
title: xAI Launch Web Search API-LiveSearch is a real-time dynamic search for data sources such as X Platforms, Internet and News
date: 2025-07-03 12:00:00 +0800
category: Frontier Trends
thumbnail: /style/image/xai-api-live-search-x_1.jpg
icon: design
---
* content
{:toc}

xAI Launchs a web search for API: LiveSearch, integrated into its Grok AI model, allowing real-time dynamic search of data sources such as X platforms, Internet and news through API, thus achieving more time-bound and accurate answers.

# Core function

- ** Real-time data search**: Grok has access to X posts, web pages and trend news to answer queries based on the latest information.

- **Flexible controls**: Developers can set search parameters through API, e.g. enable/disable search (search_parameters.mode).

- Limit the number of search results (max_search_resources).

- Specifies the time frame, domain name (including X platform) or whether to include references.

**Transparent reasoning**: In conjunction with DeepSearch functionality, Grok can demonstrate the search and reasoning process and provide a clear source of answers.

# Use the way #

- **API Access**: xAI provides LiveSearch API,** is currently in the free Beta phase (as of 5 June 2025)**. Developers can access the API key via xAI official network (x.ai/api) and start building applications.

- **Python SDK**: Supporting integration through Python requires setting of XAI_API_KEY environment variables and installing SDK.

- **GUI tool**: Community-developed Python applications (e.g. xAI LiveSearch App) provide graphical interfaces to facilitate testing and interaction.

# Apply the scene #

- ** Real-time information query**: e.g. news summaries, social media developments or market trends.

- **Auxiliary research**: Rapid aggregation of multi-source data to support academic or business analysis.

- **Developer Innovation**: Build AI applications based on real-time data, such as chat robots or information aggregation tools.

# working mechanism

# # The core advantage #

- There is no need for manual user management of search logic or tool chain calls;

- Whether or not to search, when to search and what to search for within the model;

- Support customisation of parameters such as data source, date range, area, quantity, etc.

##    (https://assets-v2.circle.so/roc5mfiu4eazhex4o6d6ei)  The type of data source that is accessible (as specified in the sOURces field)  (https://assets-v2.circle.so/zbvky8i40gmor357yibhyquq) Example: Allow models to search news +X platform content: "sources" [{types: neews"}, {types: "x}  Senior parameter configurations] [https://assets-v2.circgm3k2.sjlg9#jlg

- In streaming responses, the fields return only in the last (chunk);

- All requests for structural support for Python examples call.

Payload = messages: [{"rule": "user" , "content": "What's moving in tech news today"? ], "search_parameters": {mode": "auto", "sources": [{"type": "news"}, "return_cities": True, "from_date": "2025-05-20", "to_date": "2025-05-21", "model": "grok-3lates" } Visit: https://docs.xai/docs/sources/live-search