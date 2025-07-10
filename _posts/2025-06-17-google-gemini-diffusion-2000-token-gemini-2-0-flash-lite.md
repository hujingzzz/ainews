---
layout: post
title: Google Gemini Diffusion model based on proliferation mechanisms at a speed of 2,000 token/seconds comparable to Gemini 2.0 Flash-Lite
date: 2025-06-17 12:00:00 +0800
category: Frontier Trends
thumbnail: /style/image/google-gemini-diffusion-2000-token-gemini-2-0-flash-lite_1.jpg
icon: image
---
* content
{:toc}

In Google I/O 2025, Google Deepmind first made public the cutting-edge technology it was developing - **Gemini Diffusion**, a new way of applying proliferation models to language modelling.

# What's Gemini Diffusion?

- Traditional language models (e.g. GPT) produce one token at a time using the **autoregressive** mechanism.

- **Gemini Diffusion** draws on the “proliferation model” mechanism in the field of image generation - to produce complete output through gradual noise removal.

This non-negative-causal reasoning has two major advantages: **Apparent rate of generation**: Achievable **2000 token/sec**, including all computational processes such as tokenization, prefilling, filtering, etc. ** Stronger global reasoning**: not relying on step-by-step production, can think on the whole.

# The rationale for the model is the difference between traditional self-regression models

- **self-regression model** (e.g. GPT, PaLM, etc.): predict the next word (token) sequentially, generation one after another.

- Advantages: simple structure and extensive application.

- Deficiencies: slow generation and limited global coherence.

** Gemini Diffusion model** (based on proliferation mechanisms):

- Core idea: ** Gradual “noise” from random noise to produce text**, analogous to image diffusion models (e.g. Stable Diffusion).

- Each step is not a direct generation of words, but rather a fine-tuning and correction of the content currently generated.

- Be able to achieve content construction faster and to correct errors during generation.

(https://assets-v2.circle.so/4zhk4403d7hrdz94va677utgcq9h) ##principal advantage

- Methods of work: first add a “complete text expression” to noise damage, then the training model is gradually “noise” and reverts to a reasonable text.

- **Natural support for error correction and editing**: since each step is essentially “adapted”;

- **According to the generation of complex structures**: for example, mathematics, programming languages, the structure and semantic rigour are required.

** Natural mechanisms for correcting errors**

- Errors in the generation of traditional models require external tool detection and rewriting.

- The proliferation mechanism itself consists of a gradual process of amendment that makes the output more fluid and accurate.

Mathematics and code processing skills.

- Gemini Diffusion is superior in terms of “verifiable structural content”.

- For example, mathematical expressions, program codes that satisfy syntax correctness and logical consistency, and diffusion models are better at such “editorial generation”.

# Case demonstration #

##1. **The programming scene performed excellently** Gemini Diffusion was particularly good at code generation, which Brendan called “**vibe counting**” experience: almost real-time high-quality code writing. Actual velocity **2000 tokens/sec**, including:

- Tokenize

- Prefill (prefill)

- Safe filter.

- Output synthesis

Compared to self-regression models such as GPT-4/Claude, the speed increase is significant and suitable for high-frequency interactions or low-delayed scenarios (e.g. code editor, chat robots, etc.).

## 2. ** Complex mathematical problems can also be easily resolved** Traditional language models (e.g. GPT-4o) are prone to failure in the face of mathematical questions such as “first answer” and “cross-step logic” because they are predictive and each step magnifies previous errors. Gemini Diffusion uses a non-causing structure that “** builds the logical framework of the full answer first, then fills the details**.” Example 1: ** Topic **: ( 81) * (2/3) 2 + (15-3) / (22)” answers should be given first.** Answer: 39  Gemini Diffusion correctly completed, GPT-4o failed to solve.

## 3. ** Non-linear, multistep reasoning** Example  Question 2: ** Topic **: How many prime numbers do you have between 150 and 250? ** Answer: 18 prime numbers, list output [151, 157, ..., 241, 251]  Gemini Diffusion precisely completed, GPT-4o also failed.

##4. ** Non-regression structure = reasoning is no longer restricted by “order”** The non-regression properties of the proliferation mechanism allow models to optimize the structure of the answer on a global scale**, addressing those tasks that require “know the end before write the beginning” and breaking the traditional token-by-token limit.

# Applying perspectives and impacts

♪ ♪ ♪ ♪ apply the scene ♪

- High-reliability language generation (e.g., financial, legal, medical texts)

- Programming aids (code generation, error fixes)

- A mathematical question.

- Text editing, colouring, rewriting tasks

# The future of technology #

- It is expected to be integrated with multi-model diffusion models such as images/sounds;

- Breaking the existing paradigm of large language models and forming a new generation of “post-return-era” structures;

Official presentation: https://deepmind.google/models/gemini-diffusion/