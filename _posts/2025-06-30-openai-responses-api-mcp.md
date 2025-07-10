---
layout: post
title: OpenAI Responses API major upgrade-supports new tools such as image generation, code interpreter, remote MCP
date: 2025-06-30 12:00:00 +0800
category: Frontier Trends
thumbnail: /style/image/openai-responses-api-mcp_1.jpg
icon: web
---
* content
{:toc}

OpenAI announces a major functional extension of **Responses API** to open up more modular capabilities to developers, making AI applications to construct multi-module, complex task chains easier, more manageable and stronger. Responses API is mainly used for **building intelligence applications**, i.e. smart applications with the ability to "think autonomously plus tools". **  What is the difference between it and the traditional ChatGPT API? **[https://assets-v2.circle.so/8ugtnecd6as5d6n7fuyln3hxvl] # What can it do? ** Basic function**! **[https://assets-v2.circle.so/8ugtnecd6as5d6n7fyln3hxkvl] #

- Answer questions, chats, writings, summaries, etc. (like ChatGPT API)

** New Tool Calling** allows AI to call the following tools automatically:

-  Web search: real-time search for up-to-date information

-  File search: search and analyse files uploaded by users

- Code Interpreter: running code, drawing, math

-  Image Generation Tool: Images generated from text

- Remote MCP tool: Connect to other systems (e. g. Stripe, Shopify, Twilio, etc.)

** The enhanced “intelligent thinking”**

- Models can be “chained thinking” (Chain of Thought), multi-step reasoning and phased-in tools in one response.

- Support **Reasoning Summer**: Seeing how models step by step to come up with answers.

** Backstage mode (Background Mode)** allows AI to do complex tasks (e.g. long search, analysis, drawing) without fear of time-lapse.

# # for example: the use of Responses API, you can use Responses API to build a "financial consultant " AI, which can do: read the Excel report that you uploaded (through file search); analyse the data and generate a chart (through Code Interpreter); search the latest financial news (through Web search); and finally produce a professional financial analysis. You just need to call API, which will automatically phase out all the tasks.

#  Add a new feature at a glance:

## 1.  ** Remote MCP server support**

- Developer can now extend context (Context) from local to remote MCP service

- A tool to connect the model to any MCP server hosted through several lines of code.

- To build large, multi-source, distributed AI applications

- Making context construction more modular, safer and shared

- OpenAI also joined MCP's steering committee to push the deal forward.

- MCP suppliers supported include: Cloudflare, Stripe, Twilio, Shopiny, PayPal, Zapier, etc. []![] (https://assets-v2.circle.so/d8ahy7o3kc02n7qjjdvekkklff] [https://assets-v2.circle.so/kvuse3uufh4ro1kyr16xukbw133d)

##2.  ** Image Generations Access Responses API**

- gpt-image-1 model image generation can be used as a tool in collaboration with language models

- Use the gpt-image-1 model as an in-house tool to support real-time preview and multi-cycle editing.

- Developers can directly call for image generation in the reasoning process and progressively optimize results.

- Supports **stream preview of images**: generating processes that can be visualized in real time

- **In support of multi-wheel image editing**: step-by-step refinement of image details to fit the creative scene

#3  **Code Interpreter (Advanced Code Tool) Access Responses API**

- Data analysis, image processing, complex mathematical and programming problems can be solved using Responses API.

- For: data analysis

- Mathematical operations.

- Programming calculations

- **Image understanding task** (e.g., “Look at the picture thinking”)

Support OpenAI o3 and o4-mini, upgrading chain reasoning (Chain-of-Thought)  Official note

##4.  ** File search support online**

- The relevant document paragraph (chunk) can be found using the reasoning model

- Support: **two vector databases searching simultaneously**

- **Array-based Attribute Filtering**

View file search examples

##5. **New Developer Support**

- **Background mode** running an asynchronous task without blocking the current request to specify the document

- **Reasoning Summers** quick look at the path of reasoning within the model to facilitate debugging and evaluation

- **Encryped Reasoning Items** allows cross-requesting re-use of reasoning in ZDR (Zero Data Retion)

#  Prices and usability! [https://assets-v2. Circle. so/5d3nio1529mzyc1mvy8wlya65rlw] support model: GPS-4o series, GPS-4.1 series, OpenAI o1/ o3/ o4-mini series. Image generation function is supported only in o3. Official introduction: https://openai.com/index/new-tools-and-features-in-the-responses-api/