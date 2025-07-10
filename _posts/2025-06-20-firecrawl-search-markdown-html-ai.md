---
layout: post
title: Firecrawl introduces new functionality /search: search + fetch web content from backstage and return to Markdown, HTML, screenshot, etc. to AI
date: 2025-06-20 12:00:00 +0800
category: Frontier Trends
thumbnail: /style/image/firecrawl-search-markdown-html-ai_1.jpg
icon: game
---
* content
{:toc}

Firecrawl introduces a new feature /search, a web search and capture interface specially designed for developers and AI agents. Users can request the search results and their full content through an API and return format support Markdown, HTML, screenshots, etc. to facilitate the use of large models. **Focus bright spots: **

- **API call to enable search + fetch web content**.

- Direct operation of natural language queries at the back end without the need for a browser or a third-party search service.

- Return to content format support: **Markdown, HTML, pure link, web screenshot**.

- The output is friendly to the LLM (large language model) and allows AI to process web content.

** To give you an example:** you want an AI to search for the latest AI technology online, and you also need to extract the content of each result from the page. Previously, you might need to take two steps: search API to get the search results and then grab the content separately for each site, and now just need to **call/search interface** to:

- Search keywords.

- Automatically retrieve web content for each result

- Get formatting standards, appropriate data for AI (e.g. Markdown)

#  Core function ** Integrated search + grab operation**

- Using /search endpoints, you can search the network during a call and select to capture the page contents of the search results.

** Flexible results format**

- Whether you're building AI agents, carrying out in-depth research, looking for potential clients (leads), or developing programming, you need** quick access to appropriate web data**. With /search interfaces, you can get one-off: markdown: structured Markdown format content;

- html: processed HTML;

- RawHtml: original HTML;

- Links: links extracted from the page;

- Screenshot / Screenshot@fullPage: Web screenshot (full-page or partial);

- Extract: Structured data extraction.

** Search parameters are custom-made** by displaying /search how they are used via MCP **

- Support for search language (hl) and country (gl) through parameter setting;

- Time filter supports the following particles (using tbs parameters): qdr:h: past 1 hour

- qdr:d: The last 24 hours

- qdr:w: The past week

- qdr:m: The past month

- qdr:y: The past year

Supports the setting of time limits for searches. ** Example of response structure** "Success": true, "data": [{"title": "Firecrawl - The Ultimate Web Scraping API", "Description": "Firecrawl is a powerful web scraping API...", "url": "https://firecrawl.dev", "markdown":...", "links": [...], "metadata: {title":...", "description": "...", "sourceURL":...", "stateCode": 200}

# # # where the scene is # # # where the scene is # # # where it's going to be # # # where it's going to be # # # where it's going to be # # # # where it's going to be # # # # where it's going to be # # # # where it's going to be # # # # # where it's going to be # # # # where it's going to be # # # #

- Automate knowledge extraction

- Structured integration of search results

- Market monitoring and situation analysis

- Content aggregation tool development

- AI Training data construction

Detailed documents: https://docs.firecrawl.dev/features/search

#Firesearch: In order to demonstrate the capability of this new function, Firecrawl has also developed an open source application **Firearch**, which is a research tool showing how to construct a full research product. **Firesearch** is a combination of Firecrawl /search API and OpenAI GPT-4o. ** Firecrawl is a smart search tool built to demonstrate the capability of this new function. **Firecrawl also developed an open source application **Firesearch**, which is a research and question-and-answer site for complex issues. **Firesearch** is a combination of Firecrawl /search API and OpenAI GPT-4.** A smart search process (structure unstructured)** ** Query Debition**

-  Real-time search progress update

-  Auto-retry strategy: keyword conversion, synonym replacement, query re-engineering

-  Full citation: each answer with the original web link

-  Session memory: support context follow-up and multiple rounds of queries

-  Configureable parameters (e.g. maximum number of queries, minimum content length, overtime, etc.)

##  Core technical component![] (https://assets-v2.Circle.so/53krff3pyue4r4rangefiuqosx) GitHub: https://github.com/mendableai/firesearch

#Deep Job Researcher**Deep Job Researcher** is an all-store application based on **Next.js** to help job-seekers to match job information on the Internet by uploading their CVs.

# #  Core function ** résumé **

- User-to-peer PDF curriculum vitae;

- The system extracts key information such as skills, experience and educational background through the OpenAI model.

** Job matching**

- Use Firecrawl API for web-based reptiles to capture real job information;

- OpenAI analyzes the job description and scores it against the curriculum vitae.

** Matching rating and explanation**

- Matching ratings for each position;

- Provide explanations in natural languages as to why the position is suitable (or inappropriate) for users.

** Advanced filter**

- Users can screen results by job type, region, pay range, experience requirements, etc.

GitHub: https://github.com/mendableai/firecrawl-app-examples/tree/main/deep-job-researcher