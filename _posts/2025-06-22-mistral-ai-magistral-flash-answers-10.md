---
layout: post
title: Mistral AI launched its first open-source model focused on reasoning, Magistral Flash Answers, 10 times faster than the competitor.
date: 2025-06-22 12:00:00 +0800
category: Frontier Trends
thumbnail: /style/image/mistral-ai-magistral-flash-answers-10_1.jpg
icon: game
---
* content
{:toc}

Mistral AI announced the launch of its first linguistic model focused on reasoning **Magistral** aimed at addressing the shortcomings of the current mainstream LLM in the following areas:

- ** Lack of depth of knowledge in the field** and poor performance in professional tasks (e.g. financial modelling, legal analysis).

- ** The reasoning is not transparent** and it is difficult for users to track the logic of the model ' s conclusions.

- ** Weak multilingual reasoning**, especially in non-English languages.

- ** Lack of chain-based thinking support (Chain-of-thought, COT)** which makes complex issues difficult to solve.

Magistral seeks to construct an AI that “** can think like humans**” - with the ability to be structured, verifiable, step-by-step, while supporting multilingual use.[1] (https://assets-v2.Circle.so/1ktkb1h1bolve7kykg6lziw7jov1)** model version**

- Open source version of the **Magistral Small**:24B parameter (Apache 2.0 protocol), which can be downloaded on Hugging Face.

- **Magistral Media**: The more powerful version of the enterprise, through Le Chat, La Plateforme API, Amazon SageMaker @64, will be available in the future to provide the most consistent answer through multiple generation versions, indicating the ability to balance diversity and consistency.[] (https://assets-v2.circle.so/d9isxzj5mj5mh9stwlq2byyztu1hv) The Medium model has reached an accuracy of **90%, close to the top closed source model GPT-4 Turbo, particularly in professional tasks. ** [https://assets-v2.circle.so/n8xdje6quac4d4käfne] - a highly interactive, inter-interpreciated, inter-interpretive mandate;**

- Operationalization in ** professional scenes (law, science and technology, academia)**;

- In the congener open source model (20B-30B) ** is the one with the strongest reasoning**.

# Core technology and architecture bright spots **1.  Chain-of-Thought Native Support** Magistral Original Support Chain Thinking (CoT) and can **auto generate interpretible links of thinking**. This is particularly critical for complex tasks (e.g. legal reasoning, system planning). ** Logic optimization design **

- The model has been fine-tuned specifically for “multistep logical reasoning”.

- Support for the creation of the Inner Thinking Path (inner Monologue), which presents a complete reasoning trajectory.

- The output format is <think>... </think> to distinguish between drafts and summaries and to improve interpretability.

**2. Multilingual high-level reasoning** Models have multi-language reasoning skills, in particular optimizing the following languages:

English, French, German, Spanish, Italian

- Arabic, Russian, Chinese.

Key points: Not only is multi-language input/output supported, but ** the chain of reasoning can also be naturally generated in the target language**. **3.  Flash Answers + Tink Mode (business version only)** via the "Le Chat" platform, which is open by Magistral Medium:

- **Flash Answers**: 10 times the speed of reasoning in mainstream competitions (e.g. ChatGPT).

- **Think Mode**: Optimizing multi-round reasoning response time and efficiency.

- Actual performance: almost “seconds” of results in structured tasks (e.g. decision tree reasoning, logical proof, code planning);

- At the same time, accuracy and logic were maintained.

**4. Transparency in reasoning and traceability** Each production is accompanied by a clear “thinking trajectory” that can be tracked and audited.

# Open source, locally deployable

- Models have been opened up to support commercial uses.

- Quantified to run on single RTX 4090 or MacBook M2(32GB).

- Provide multiple platform support, including: vLLLM (recommended)

- llama.cpp version (GGUF)

- Support tools such as mstudio, llama, unsloth, Axolotl

** Chat template (recommended)** Use of default system hints (system-v2.curcle.so/sfrhxje1qvzfh4rdqxk11zeym1k, official introduction: https://mistral.ai/news/magistral model download: https://huggingface.co/mistral-Small-2506