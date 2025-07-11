---
layout: post
title: Multiverse-First by AI Generated multiplayer online game Real-time effects of player behaviourAIA world of simulations.
date: 2025-06-05 12:00:00 +0800
category: Frontier Trends
thumbnail: /style/image/multiverse-ai-ai_1.jpg
icon: book
---
* content
{:toc}

Enigma Labs Launched Multiverse A breakthrough. AI Generate multiplayer games Allow players to build and influence the world together in real timeI don't know.
The model is designed to solve the problem of existing world models that can only be simulated.“At the end of the day,Single SubjectIt's not a good idea, it's not a good idea.Limitations Build Support **Multi-agentmulti-agentI'm not sure what I'm talking about.Perceptions in shared environmentsProjections and interactions**Multi-agentmulti-agentI'm not sure what I'm talking about.Perceptions in shared environmentsProjections and interactionsStructureI don't know.
The whole project costs only. $1.5K But it's in the architecture.Significant innovations in data collection and model design It's completely open.I don't know.

- **Multi-person interaction**Multi-person interaction-Multiple players can access this at the same time. AI A world of simulations. And...**Everyone's behavior affects the world in real time.**Everyone's behavior affects the world in real time.I don't know.For example, you speed up.FloatingOverriding. It'll change the world.I don't know.

- **Low-cost high-impact**Low-cost high-impact-They can't afford it. **1500 United States dollars**1500 United States dollars Training and R & D completed It's normal. PC Run UpI don't know.The secret isn't a lot of math. It's technology innovation.I don't know.

- **Full open source.**Full open source.-They opened up the whole project. Including code.DataModel parametersStructureResearch results Let anyone learn.Use or improveI don't know.

- **Use is not limited to games**Use is not limited to games-Here.“At the end of the day,A multi-person world modelIt's not a good idea, it's not a good idea.It's more than just a game. It can also be applied in a wider simulation environment. Like robotic training.AI Collaboration, etc.I don't know.


## 🏗️ Detailed description of the core technical architecture

### 🔹 Basic structure of a single-person world modelBaselineI'm not sure what I'm talking about.
The traditional monogamous world model usually consists of the following three parts:-
**Action EncoderAction EmbedderI'm not sure what I'm talking about.**Action EncoderAction EmbedderI'm not sure what I'm talking about.Enter PlayerIf you press a keyI'm not sure what I'm talking about.Convert to vector expressionI don't know.
**To the noise network.Denoising NetworkI'm not sure what I'm talking about.**To the noise network.Denoising NetworkI'm not sure what I'm talking about.Based on Diffusion Model Predict the next frame using input actions and previous frames of videoI don't know.
**Up SamplerUpsamplerI'm not sure what I'm talking about.**Up SamplerUpsamplerI'm not sure what I'm talking about.Enhancement of low-resolution images Generate high-resolution outputI don't know.

### 🔸 Multiverse-Structural innovation in multi-person models
To match multiple scenes Multiverse The above structure was redesigned-

- **Double-In Action Encoder**Double-In Action Encoder-Receive control input from two players at the same time. Construct a joint vectorI don't know.

- **Share Noise Network**Share Noise Network-In a unified model Generate video frames from two player perspectives And to ensure time and space consistency.I don't know.

- **Parallel Sampler**Parallel Sampler-Sample two low-resolution frames separately But consistent image style and dynamic informationI don't know.

![](https://assets-v2.circle.so/80znrdzd1n63gccprglqjzf18nku)📌 **Key issues**Key issues-There's a lot of people on the scene. AI You have to create two visions at the same time. But it has to be all right.I don't know.Which means... **You saw the car crash. I have to see the car crash.**You saw the car crash. I have to see the car crash.I don't know.

## 🖼️ Input Data Structure Design-The way the visual perspective blends.
In order to achieve shared perception The team tried two visual ways to integrate.-
**Vertical StackSplit-screenI'm not sure what I'm talking about.**Vertical StackSplit-screenI'm not sure what I'm talking about.-It's like a traditional swab game. Scroll two images up and downI don't know.
**Channel Axis IntegrationChannel StackingI'm not sure what I'm talking about.**Channel Axis IntegrationChannel StackingI'm not sure what I'm talking about.-Bring two frames along RGB Channel dimensions stackThat is, every pixel becomes6A tunnel.I'm sorry, I don't know.
![](https://assets-v2.circle.so/o8n0dy5soppsqijflf8mxg84uj9p)Results-**The axle is better integrated.**The axle is better integrated. Because it's a way to make U-Net The network handles information from both angles in all volume layers at the same time Increase the logical consistency of the imageI don't know.

## 📏 Long-term sequence modelling and context optimization

### 🎯 Problem-Multiple interactive physical phenomenaIf moved relativelyBrake effectsI'm not sure what I'm talking about.**Slow but critical change**Slow but critical change It takes longer windows.I don't know.

- **Short-term developmentsLike brakes.I'm not sure what I'm talking about.**Short-term developmentsLike brakes.I'm not sure what I'm talking about.-Use it. 8 Frame0.25 secI'm not sure what I'm talking about.enough modelling.I don't know.

- **Long-term interactionFor example, overcarrying.CollisionI'm not sure what I'm talking about.**Long-term interactionFor example, overcarrying.CollisionI'm not sure what I'm talking about.-Yes. 0.5~1 Seconds, even longer.I don't know.

![](https://assets-v2.circle.so/9x06ka6sn2e7wfb92qows1179jj2)
### ✅ Solutions-**Scratch time sampling + Tier forecast**Scratch time sampling + Tier forecast

- Use Recent 4 Frame + Every 4 Frame1FrameTotal8FrameI'm not sure what I'm talking about. → To get a longer sense without adding to the visible pressure.I don't know.

- Introduction **Curriculum LearningCourse-based trainingI'm not sure what I'm talking about.**Curriculum LearningCourse-based trainingI'm not sure what I'm talking about.-Training for short-term projections first Gradual transition to the longest. 15 Predictable range of seconds Reconciling learning efficiency with ability to expressI don't know.

## 🧪 Dataset build and training process

### 🎮 Game platform selection-Gran Turismo 4GT4I'm not sure what I'm talking about.

- Use Tsukuba Circuit Scene Easily modeled and reproducedI don't know.

- The game is not supported. 1v1 Mode Team pass. **Reverse Project**Reverse Project Force the real one. 1v1 Game.I don't know.

### 📹 Data collection strategy

- Each game recorded a double-view playback.Perspectives of each playerThis is the first time I've ever seen you.Synchronize laterI don't know.

- Control inputThe throttle.Brake.Turn around.I'm not sure what I'm talking about.Pass.**Computer Visual Reading HUD Elements**Computer Visual Reading HUD Elements No manual recording.I don't know.

### ⚙️ Automation generation mechanism

- Utilization GT4 Medium B-Spec ModeAI Drive.I'm not sure what I'm talking about.+ Script Send Control Command → Batch generation of available video dataI don't know.

- Experimental access OpenPilot Control of autopilot models But because of stability and resource optimization, Final Selection B-SpecI don't know.

## Research values and application prospects

### Core breakthrough.-

- Achieving a multi-faceted perspective**Modelling a Coherence World**Modelling a Coherence Worldsynchronized multi-perspective generationI'm sorry, I don't know.

- Introduction of efficient training strategies and replicable data pipelines Support for open community recovery and certificationI don't know.

### Potential applications-
![](https://assets-v2.circle.so/rolivejo1gd7ku1747rkbzxfwfbh)Official presentation-https://enigma-labs.io/blog 
GitHub-https://github.com/EnigmaLabsAI/multiverse
Model-https://huggingface.co/Enigma-AI
