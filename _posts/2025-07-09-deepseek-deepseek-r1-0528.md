---
layout: post
title: DeepSeek DeepSeek R1-0528-Significant improvements in code capabilities and writing skills, deeper reasoning capabilities and repair of some problems
date: 2025-07-09 12:00:00 +0800
category: Frontier Trends
thumbnail: /style/image/deepseek-deepseek-r1-0528_1.jpg
icon: book
---
* content
{:toc}

DeepSeek released **DeepSeek R1-0528 update,** which was communicated last night to the WeT community as “** small pilot upgrade**” and was open for testing.

# **DeepSeek R1-0528 Update bright spots**

## 1. Deeper thinking skills have increased significantly, with the DeepSeek-R1-0528 model still using as a base the DeepSeek V3 Base model released in December 2024, but more arithmetic has been invested in the subsequent training process, significantly increasing the depth of thinking and reasoning of the model. The updated R1 model has achieved the highest achievement of all current models in the country in a number of baseline assessments, such as mathematics, programming and universal logic, and is still approaching other top international models, such as o3 and Gemini-2.5-Pro.[] (https://assets-v2.circle.so/vuglp8xg0u64wag0atvqle7cbo) - **technical background: although still based on DeepSeek V3 Base, the model has been significantly enhanced in the reasoning chain** through the use of resource inputs in the course of this enhanced training.

- **AIME 2025 Results of the evaluation**: Accuracy of the old version: 70%

- Accuracy of new editions: **87.5%**

**Token uses comparison** (per question):

- Old edition: 12K

- New edition: 23K shows that the new edition is capable of “slower and deeper thinking” and simulates the path of detailed human reasoning.

##2. Thinking chain distillation to medium scale models train Qwen3-8B Base after distillation by DeepSeek-R1-0528, obtained by DeepSeek-R1-0528-Qwen3-8B. The 8B model is second only to the AIME 2024 test by DeepSeek-R1-0528 and exceeds Qwen3-8B (+10.0%) and is comparable to Qwen3-235B.** We believe that DeepSeek-R1-0528 is important for the study of academic reasoning models and for the development of small models by industry.**

- Based on R1-0528 Distillation **Qwen3-8B Base **.

- The new model is better than Qwen3-8B in AIME 2024, close to Qwen3-235B.

- Demonstrate the high academic and industrial value of the distilled “think chain”.[] (https://assets-v2.circle.so/4cexjbe4m88sxtx2f6vvsuy500ix)

#3. Increased ability to write

- Production capacity has been fine-tuned and optimized.

- Support long text output that is more structured and more closely aligned with humans.

- Substantive enhancement of output capacity, especially for complex literatures, such as ** paper papers, novels, essays.[1] (https://assets-v2.circle.so/6mzro4d69k59nldzrm3ifow3qg3s)

## 4. Error control and hallucination rate drop

- **Imagination optimization goal**: Reduce the “none-in-kind” content of model output.

- **Application scene**: rewrite lubricant

- Read and understand.

- Summary

** Performance enhancement data**:

- Reduced hallucination rate: **approximately 45 ~ 50 %**

- More credible output and improved consistency of information

# # 5. Tool calls and code enhancement

- The new version supports **Function Calling** and **Json Output**.

- **Tau-Bench assessment of achievement**: Airline: 53.5%

- Retail: 63.9%

- Horizontally close to OpenAI o1-high, but slightly lower than O3-high, Claude 4 Sonnet.

(https://assets-v2.circle.so/e1l6gsyx43pif5lhj3zgsj4dvc0w)** front-end code generation capability upgrades** and upscaling in complex multi-cycle dialogue tasks such as role-playing.  (https://assets-v2.circle.so/bxpxjz9ciei6lh55cubt38kevpxp) ###6 ** problems repair and optimization**

- Rehabilitate frequently asked questions from early R1 models: ** Repeated answer**

- ** The format is out of order**

- ** Language mix (CEF)**

Output is more standardized and ** suitable for use in professional settings**.

## Multiple Mission Capability Optimization Performance![] (https://assets-v2.Circle.so/gtq5ems4nbbw7f0el57rexhbefe) - **Benchmark evaluation**: In the evaluation of **LiveCodeBnch** code generation developed by UC Berkeley, MIT and Cornell: R1-0528 is comparable to front-line models such as **OpenAI **, slightly less than **o4 mini**, especially in mathematics, programming and complex reasoning tasks.

- ** Grok 3 Mini and Qwen 3** of Alibababa better than xAI.

DeepSeek’s influence in China’s AI technology competition has been further enhanced.[3] (https://assets-v2.circle.so/io4j1766fe2nu4zu7azekbtz0) DeepSeek has uploaded R1-0528 to Hugging Face, but has not yet published a public description or model description.

# **API update*** ** API has been synchronized and interfaces and calls have remained unchanged. The new version R1 API still supports viewing the model thinking process, with additional support being given to the Fund Action Calling and JsonOutput. We have adjusted the meaning of the parameters for max_tokens in the new version R1 API: now max_tokens are used to limit the total length of a single output of the model (including the reflection process) by default to 32K, with a maximum of 64K. Requests API users to adjust the max_tokens parameters in time to prevent early interruption of the output.

##** Model Open Source*** ** DeepSeek-R1-0528 Using the same base model as the previous DeepSeek-R1 model, only post-training methods have been improved. For privatization deployments, only updated checkpoint and tokenizer_config.json (toool calls) model parameters are 685B (of which 14B is the MTP layer), opening text with 128K (webends, App and API provide 64K above). DeepSeek-R1-0528 model weight downloads are required to be consulted: **ModelScope:** https://modelscope.cn/models/deepseek-ai/DeepSeek-RepSeek-Reek-Reek-R-R-0528 **Hugingface: **https://huggingface.co/deepseek-ai/DeepSeek-Re1-0528, using the old version of Sep-Se-Se-Se-Se-Surb, using the existing version of the model, including the new version of the software, using the new version of the map, using the software.

# ** Recent call to the Web site Deepseek-R1-0528 API**1, Openrooter address: https://openrooter.ai 2. GMI tutt: https://inference-engine.gmicloud.ai 3. Novita tutt: https://novita.ai 4. Nebius tbtit: https://studio.nebius.com 5. Inference toti: https://inference.net Official Presentation: https://api-docs.deepseek.com/zh-cn/news/news2528