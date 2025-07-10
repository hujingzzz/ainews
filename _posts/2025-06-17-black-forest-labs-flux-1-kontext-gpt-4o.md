---
layout: post
title: A new generation of multi-model image generation and editing models launched by Black Forest Labs-FLUX.1 Kontext can achieve GPT 4o image capability
date: 2025-06-17 12:00:00 +0800
category: Frontier Trends
thumbnail: /style/image/black-forest-labs-flux-1-kontext-gpt-4o_1.jpg
icon: book
---
* content
{:toc}

The new generation of ** multi-model image generation and editing models launched by Black Forest Labs: FLUX.1 Kontext**, unlike the traditional text-map model, Kontext understands ** text and image ** input to achieve true ** context generation and editing**. The traditional **text-to-image (text-generation image) model** such as DALL E, Stable Diffusion, etc., has many limitations:

- Only by word control, which does not allow for a flexible combination of pictures as context;

- The inability to continuously edit or retain character features and the lack of “cognitive continuity”;

- Local editing requires complex masking or ginturing;

- Frequent deterioration of images after multiple rounds of operation (frustration, loss of style);

- Slow editing and failure to meet real-time interactive needs.

###FLUX.1 Kontext's objective: to build a real **Context-aware** image generation and editing engine. In other words: ** You can control image generation and modification, be flexible, efficient, and keep people and style consistent, as naturally as Photoshop + GPT does.** It focuses on:

- **The ability to understand the image context** (not only to generate the image from the text, but also to understand it and modify it)

- ** Rapidly interactive editing capacity** (low delay, step-by-step)

- **Role consistency, local editing, style migration, etc.**

_ (https://assets-v2.circle.so/rgixc9ist6r5iybm8t6v5gk8bbiz) ## Kontext8biz? **Role consistency**: Consistency of people or elements can be maintained in multiple scenarios ** Local editing**: Only specific parts of images can be edited without affecting other regions ** Style reference**: New scenes can be generated under specified style ** Interactive ** Rapid **: Rapid overlap, extremely low delay

## Model version: [] (https://assets-v2.Circle.so/ o3ypo0yuueuvboee3ktkd0p4fbm1) - **FLUX.1 Kontext [pro]** suitable for fast-track editing to support continuous editing, maintaining consistency of roles, identities, styles and features in multiple scenarios

- **FLUX.1 Kontext [max]** High-performance version with greater ability to follow hints, better layout performance and consistency

- **FLUX.1 Kontext [dev]** Open source weight version of our state-of-the-art image editing model is currently in ** private beta**

# Main function

##  1. Text-Mixed Control (Text + Image Prompt) not only can generate images in text, but can upload images and modify them in text. #[!] (https://assets-v2.Circle.so/8ba8qxwqxaec0mfmbttr5o0563)![] (https://assets-v2.circle.so/miiwix7vpuucq6gzrj30dod67r) ###2. Local Editor (Local Editing)

- It can be ** accurate to modify a part of the image** without affecting the overall style or other area.

- There is no need for masking, stratification or image labelling.

This means that:** you can only “do what you want” as a mechanic.**![[https://assets-v2.circle.so/pxbjoiptu5i3m09saytcuxig78oy]** left figure:** input image;** middle figure **: edit according to input: “Replace `YOU HAD ME AT BEER' to `YOU HAD ME AT CONTEXT'”,** right figure:** “Replace the scene to a nightclub”

#3 3. Consistency between character and style (Character & Style Consistency)

- Regardless of how many different scenes you generate, the model automatically maintains the person's face, face and posture, provided that the same reference map or description is provided.

- A uniform expression of style (e.g., cartoons, writings, water colours) can also be maintained.

To construct continuous visual content (e.g. caricature roles, virtual spokespersons) is very valuable. <[!] (https://assets-v2.circle.so/9zeemiyp08z2hmne91ny2pvpc33) [!] (https://assets-v2.circle.so/yvo2psmzrkd0utcn2z236mvvvvgb) [## 4.] (https://assets-v2.circle.so/2ao6j32x4odz72vrcun6yz7izlv) ##4.

- You can change it over and over again to the same figure: "Let her laugh first, then put on the sunglasses, then change the background, then change the clothes."

- Each step of change is based on the retention of the previous round.

This is the first model system to allow multiple rounds of natural language to drive visual modifications.  (https://assets-v2.circle.so/dv035pl7xxypwhjbcz8dtttl9158k) ** left figure: ** entered image;** middle figure **: edited according to input: “Pick her head towards the lens”,** right figure: ** “Let her laugh”

# # 5. Low Latency Infence

- 8 times as fast as the current mainstream model;

- Close to “real-time feedback” can be achieved during editing and generation, which is suitable for fast test errors and adjustments by users.

# How does the assessment work? Is the performance leading? Black Forest Labs has proposed a new test set: ** KontextBnch**, which measures the modelling capabilities of the image task that drives the context. The FLUX.1 model has ** leading performances at the following six dimensions: **Accuracy of text-guided editing** **Accuracy of image authenticity and style consistency** ** Role image has remained constant in multiple images** ** Stable in text layout and content** ** Stability in multi-cycle editing** ** Response speed and reasoning efficiency** Results:

(https://assets-v2.circle.so/cxabocmyo9w3lx4sj7p0tw56zw9g) **FLUX.1 Kontext [pro] is one of the best models of current performance on the core tasks of “role coherence” and “text editing accuracy”.**

# They've also launched an interactive interface

##  FLUX Playgroup Profile: A ** GUI platform for developers, creators** that uses the FLUX model quickly without any code or integration.  Features:

- Enter text or upload images and experience the generation and modification of effects in real time;

- Multiple rounds of editing can be performed to see the comparison of each step;

- A prototype and capability demonstration to be presented to clients or decision makers;

Address: https://playground.bfl.ai/

# Current restrictions and concerns BFL also honestly list current model limitations:

- The possible deterioration of the quality of the image (e.g., colour pseudo-portrait, vague details) after several consecutive revisions;

- In individual cases, the model ' s interpretation of the text deviates from or ignores certain requirements;

- A weak understanding of “world knowledge” (e.g., the possibility of creating an unstructured scenario);

- Some details may be lost during the model compression distillation process (impact on high authenticity applications).

This suggests that it is better suited to the needs of graphic creativity, conceptual drawings, product prototypes, landscape mapping, etc., rather than the final phase of fine-tuning.** Official presentation: *** https://bfl.ai/announments/flux-1-kontext** technical report:**Read the full tech report