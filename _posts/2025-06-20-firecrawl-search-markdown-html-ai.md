---
layout: post
title: Firecrawl Introduction of new functionality /search -Searchable from backstage + Fetch Web Contents And backMarkdownHTMLI'll wait for the screenshot.AI
date: 2025-06-20 12:00:00 +0800
category: Frontier Trends
thumbnail: /style/image/firecrawl-search-markdown-html-ai_1.jpg
icon: game
---
* content
{:toc}

Firecrawl Introduction of new functionality /search It's for developers and for developers. AI Cannot initialise Evolution's mail component.I don't know.Users can do it once. API Requesting access to search results and their full content Back Format Support MarkdownHTMLScreenshot et cetera To facilitate the use of large modelsI don't know.
**Function Highlights-**Function Highlights-

- **Once. API Call to enable search + Fetch Web Contents**Once. API Call to enable search + Fetch Web ContentsI don't know.

- Run natural language queries directly on backend Do not need a browser or a third-party search serviceI don't know.

- Return content format support-**MarkdownHTMLPure LinkWeb Screenshot**MarkdownHTMLPure LinkWeb ScreenshotI don't know.

- Output Results Right LLMLarge-language modelI'm not sure what I'm talking about.Friendly. Easy. AI Process web contentI don't know.

**Let me give you an example.-**Let me give you an example.-
You want one? AI Search the Internet.“At the end of the day,Latest AI TechnologyI'm not sure what I'm going to do.I'm also going to have to extract and analyze the content of each of the results.I don't know.You used to have to take two steps.-
Search with API Get the search results.
Retrieve content separately for each site
Now all we need to do is... **Call one time. /search Interface**Call one time. /search Interface I can.-

- Search keywords

- Automatically fetch web content for each result

- Obtaining formatting standardsFit AI Data usedLike what? MarkdownI'm not sure what I'm talking about.

## 📌 Core Functions
**Integrated Search + Capture Operation**Integrated Search + Capture Operation

- Use /search End A web search can be conducted during a call and selects to capture the page contents of the search resultsI don't know.

**Flexible results format**Flexible results format

- Whether you're building it or not. AI ProxyAI agents.Conducting in-depth researchLooking for potential clientsleadsThis is the first time I've ever seen you.It's still programming. You all need it.**Quick access to appropriate web data**Quick access to appropriate web dataI don't know.
Use /search Interface You can get it once and for all.-
markdown-It's structured. Markdown Format Contents;

- html-After processing HTML;

- rawHtml-Original HTML;

- links-Links extracted from the page;

- screenshot / screenshot@fullPage-Web ScreenshotFull Page or Part);

- extract-Structured data extractionI don't know.

Through a video Presentation /search  Pass.MCPHow do you use it?
**Search parameters can be customised**Search parameters can be customised

- Support search language through parameter settingshlI'm not sure what I'm talking about.with the Stategl);

- Time filter supports the following particle sizesUse tbs Parameters:
qdr:h-Get over there.1Hours

- qdr:d-Get over there.24Hours

- qdr:w-The last week.

- qdr:m-The last month.

- qdr:y-Over the past year

Support the setting of time limits for searchingI don't know.
**Example of response structure**Example of response structure
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

### 🚀 Applied scene

- Automated knowledge extraction

- Structured integration of search results

- Market monitoring and situation analysis

- Content aggregation tool development

- AI Training data construction

Detailed Document-https://docs.firecrawl.dev/features/search

## Firesearch-AI A driver-driven research tool for in-depth networks
To demonstrate the ability of this new function, Firecrawl And an open source application has been developed. **Firesearch**Firesearch It's a research tool. Show me how to use it. /search To build a complete research productI don't know.
**Firesearch**Firesearch It's a combination. Firecrawl /search APIand OpenAI GPT-4o Constructed Smart Search Tool Multiple rounds can take place.Multi-source Web Info FetchAnalysis and integration Research and question and answer scenes applicable to complex issuesI don't know.
![](https://assets-v2.circle.so/z2xprmkyz1zkcm89jsd2lbkbn7b3)
### 🔧 Function Highlights
**✅ Smart search processStructure DismantlingI'm not sure what I'm talking about.**✅ Smart search processStructure DismantlingI'm not sure what I'm talking about.
**Query Decomposition**Query DecompositionDismantling complex issues into smaller onesManageable sub-issues
**Multi-Search via Firecrawl**Multi-Search via FirecrawlConduct an independent search for each sub-issue Generate up to 12 Search request
**Content Extraction**Content ExtractionExtract from each result page Markdown ContentsUse scrapeOptionsI'm not sure what I'm talking about.
**Answer Validation**Answer ValidationDetermining whether page contents are“At the end of the day,Really answered the question.I'm not sure what I'm going to do.Confidence threshold is 0.7+
**Retry Mechanism**Retry MechanismAutomatically replace keywords when hitAdjust semantic reQueryTry again at most 2 Number of timesI'm not sure what I'm talking about.
**Answer Synthesis**Answer SynthesisGPT-4o Combining all hits into combined answers with referenced sources
**📌 Advanced Features Overview**📌 Advanced Features Overview

- ✅ Search progress updates in real time

- 🔁 Automatic Retry Policy-Variation of keywordsSynonym replacementQuery Restructure

- 📎 Full citation-Each answer with the original web link

- 🧠 Sessional memory-Support context queries and multiple rounds of queries

- ⚙️ Configureable ParametersIf maximum number of queriesMinimum content lengthTimeout waitingI'm not sure what I'm talking about.

### 🧠 Core technical components
![](https://assets-v2.circle.so/53krff3ol3pyue4r4rngefiuqosx)GitHub-https://github.com/mendableai/firesearch 

## Deep Job Researcher 
**Deep Job Researcher**Deep Job Researcher It's based on **Next.js**Next.js Development of a full-store application Helping job seekers to upload curricula vitae Smart matches job information on the InternetI don't know.It's a combination. **Firecrawl**Firecrawl It's... it's... it's... /search Web capture capabilities and **OpenAI**OpenAI synonyms for synonyms Provide in-depth personalized job referralsI don't know.

### 🚀 Core Functions
**Diagnosis of curricula vitae**Diagnosis of curricula vitae

- User Upload PDF Curricula vitae;

- System pass. OpenAI Model extraction skillsKey information such as experience and educational backgroundI don't know.

**Job Matching**Job Matching

- Use Firecrawl API We're going to do a web reptiles. Fetch real job information;

- OpenAI Parsing job descriptions And score with the résumé.I don't know.

**Match Ratings and Explanations**Match Ratings and Explanations

- Matching scoring per position;

- Provide a natural language explanation as to why the post is suitableOr not.I'm not sure what I'm talking about.UserI don't know.

**Advanced Filter**Advanced Filter

- Users by job typeRegionSalary scaleEmpirical requirements for sieve results etc.I don't know.

GitHub-https://github.com/mendableai/firecrawl-app-examples/tree/main/deep-job-researcher
