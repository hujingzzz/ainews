---
layout: post
title: Google Gemma 3n: A new generation of lightweight multimoderated AI models with a response speed increase of about 1.5 times 2GB memory cell phones running.
date: 2025-06-15 12:00:00 +0800
category: Frontier Trends
thumbnail: /style/image/google-gemma-3n-ai-1-5-2gb_1.jpg
icon: link
---
* content
{:toc}

**Gemma 3n** ("n" means Nano or Next-gen) is the latest lightweight open source AI model launched by Google, which aims to achieve the three objectives of "**on-device+ multi-module perception + low-efficiency delay**" and is the first prototype of a model architecture to optimize mobile devices** following the Gemma 3 series (support to desktop/coated reasoning)** and also forms the technical basis of the next generation **Gemini Nano series model**.

- Parameters size: 5B and 8B (5 billion and 8 billion parameters, respectively)

- Support of patterns: text, images, audio (voice recognition and translation), video (to be opened)

~ (https://assets-v2.circle.so/hnczcohntm5qbb9qlgslbwgln) # Core Point Function (compatibility of performance, efficiency and privacy)

# # 1. Extremely light and quick response

- **The response speed is about 1.5 times higher ** (cf. Gemma 3 4B) to achieve a <500ms delay in the first word on the high end Android mobile phone.

**Per-Layer Embeddings (PLE)**, which benefited from Deepmind innovation, has been significantly reduced in memory occupancy; although the model parameters are: 5B (5 billion) and 8B (8 billion);

The memory required at the time of actual operation is only:

- **~2GB (5B model)**

- **~3GB (8B model)**

This means that:** middle-end Android mobile phones can also run large model reasoning** without cloud support. Fit to mobile hardware platforms such as Qualcomm, MediaTek, Samsung, etc.

##2. Dynamic modifiable model structure (Mix'n'Match architecture) "**Mix'n'Match**" structure allows the 5B model to automatically switch to an embedded 2B submodel;

- The model structure embedded an embedded submodel (2B active memory model embedded in the 4B master model), which the developer can ** dynamic adjustment accuracy and reasoning speed** and adapt to different use scenarios;

- A balance between accuracy and speed, depending on the capacity of the equipment or the user's needs;

- Such a structure would achieve "one model covering multiple scenarios"

- Excellent performance in energy consumption and control, especially for battery-sensitive equipment (cell phones, glasses, headphones, peripherals).

# # 3. Full local operation, privacy priority

- The operation of the reasoned task without the need for networking;

- All data are processed on the equipment, not on the cloud, and the privacy of users is guaranteed;

- For mobile phones, notebooks, peripherals, etc.

## Multi-modular capacity enhancement Gemma 3n is one of the most advanced currently available ** mobile multi-module open source models in Google**, supported by: [x] [https://assets-v2.circle.so/cpksy3sc0xplnt493agu9jpuq523] #model uses: building the next generation of “aside-intelligent experiences”  expected application scenes![] (https://assets-v2.circle.so/g7c93o6x5jnbec10e85xlig94a8f) #how the sex can **the natural language task ** Google described its model as “high ahead” in the Chatbot Arena row, in the user preference:

- Comparable to mainstream open source models such as **Mistral 7B, Phi-3, LLama 3**;

- To demonstrate stability in the bilingual Chinese and English missions, particularly in dealing with the multi-round dialogue**, the production of long texts, and the logical question-and-answer**.

(a) Multilingual performance:

- Scores in multilingual benchmark (e.g. **WT24+**, ChrF) **50.1%**;

- Special performance in the ** Japanese, German, Korean, French, Spanish** tasks;

- This suggests that it is superior to many Western-led models in terms of the adaptability of international markets.

#one of the key technology bright spots for the elaboration of the Gemma 3n with ** significant reduction of memory occupancy during operation** is achieved in three ways:

#1 Per-Layer Embedding (PLE)

- ** What**: a new embedded strategy proposed by Google Deepmind;

- ** Activation**: Each layer uses an independent low-dimensional embedding vector instead of a full model sharing of embedding tables;

- **Success**: Reduction of memory replication;

- Better compression of the expression space;

- Support for loading on demand (lazy load);

**Efficacy**: Reduce the dynamic running memory of the 5B/ 8B parameter model to **approximately 2GB/ 3GB**;

- Runs a lightweight version similar to a 2B or 4B " disguise " of the large model.

#2Key-Value Cache Sharing (KVC Sharing)

- ** What**: Transformer models need to store intermediate results of attention mechanisms in their reasoning (Key and Value);

- ** Activation**: multiple layers or steps to share this cache, reducing double counting and memory redundancy;

- **Success**: Reduction of the intellectual memory expense;

- Speed up sequence generation and increase multiple rounds of interactive experience.

#3 Advanced Activation Quality (AAQ)

- ** What**: Quantify intermediate activation values (e.g. from float32 to int8 or infourth);

- ** Activation**: Significant reduction of model computing and memory bandwidth requirements;

- **Success**: Keeping models accurate while reducing size;

- Supporting the efficient operation of models on mobile chips (Qualcomm, MediaTek);

- In conjunction with PLE, KVC, further compressed to acceptable levels of mobile equipment.

## Mixed architecture design: Mix'n'Match mechanism ** “A set of models, multiple capabilities”** Gemma 3n internalized through the **MatFormer training strategy** achieved an embedded submodel mechanism: model structure function exemplifies that the main model (e.g. 4B) has a high-precision reasoning submodel (e.g. 2B) performance light, response rapid dynamic switching based on task complexity, automatic selection of the operational path sub-models' weights for equipment resources are shared by the main model, avoiding duplication of deployment, and this structure has the following advantages:

- Developers do not need to deploy multiple model versions;

- The trade-off between dynamic reconciliation quality and delay at running (e.g. navigational assistant vs semantic translation);

- Improve energy consumption control capabilities and adapt to high-end low-end equipment.

# How to use Gemma 3n? Google is open in two ways for different groups: Mode 1: **AI Studio (web version)**

- Without installation, to experience text interpretation and generation of the model directly in the browser;

- Fit for product managers, developers to preview model effects.

Address: Google AI Studio (google account required) Mode II: **Google AI Edge**** (local development tool)**

- Fit for developers to integrate models into APPs, local systems, hardware equipment;

- Provide SDK, documents, code examples to support the deployment of text and image models;

- Support for Android, Chrome, embedded equipment, etc.

## Detailed presentation: Official presentation: https://developments.googleblog.com/en/introduction-gemma-3n/