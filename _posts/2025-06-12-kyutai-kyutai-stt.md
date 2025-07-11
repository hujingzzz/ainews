---
layout: post
title: Kyutai Group open-source real-time voice model Kyutai STT Listen to the text and change the text. You're smart enough to judge if you're finished. Don't interrupt blindly.
date: 2025-06-12 12:00:00 +0800
category: Frontier Trends
thumbnail: /style/image/kyutai-kyutai-stt_1.jpg
icon: chat
---
* content
{:toc}

**Kyutai STT**Kyutai STT Yes. Kyutai It's a team development thing. **Real-time voice-to-textspeech-to-textI'm not sure what I'm talking about.**Real-time voice-to-textspeech-to-textI'm not sure what I'm talking about. Open source model for scenario optimization The main feature is... **Low delayHigh AccuracyStrong hand-in-hand capacity**Low delayHigh AccuracyStrong hand-in-hand capacityI don't know.
**Kyutai STT **Kyutai STT It's not just a low-delayed transliteration. Also dedicated to high-synchronous and real-life applications.Like voice-to-mouth systems.I'm not sure what I'm talking about.Design Availability**Sensory-level voice activity detection**Sensory-level voice activity detectionCapacityI don't know.
![](https://assets-v2.circle.so/sg3ndph2svwjkmu83c480zonm33q)Two versions of the model are now available.-

- kyutai/stt-1b-en_fr: English+French Low delay Fit for interactive applicationsI don't know.

- kyutai/stt-2.6b-en: English Bigger and more accurate. It applies to scenes that require a very high degree of accuracy.I don't know.

Prior introduction
Kyutai Launched Unmute-It can be inserted into any model. Makes any model soundable. | XiaoHu.AI CollegesKyutai Launched Unmute A highly modular voice. AI System Could be a model for any large text languageLLMI'm not sure what I'm talking about.Quick Add VoiceI don't know.  Which means it can be inserted into any model. Give the model voice-powering.I don't know.  Unmu...https://www.xiaohu.ai/c/xiaohu-ai/kyutai-unmute![](https://assets-v2.circle.so/bmwhuzzllqoxolrm4m7xxttlqyqo)
## Detailed description of core characteristics

### 1. Fluid Recognition-Listen to the text and change the text.
Kyutai STT Support**Real fluid voice recognition.**Real fluid voice recognition. i.e.,-

- Audio Edge Input and Process You don't have to wait for the whole thing to end.;

- Returns the transposition in real time Organisation**Punctuation symbol and word-by-word time stamp**Punctuation symbol and word-by-word time stamp;

- Under low delay It's still able to maintain a non-fluorescent model.Like WhisperI'm not sure what I'm talking about.Identification AccuracyI don't know.

These are real-time voice assistants.Live Subtitle GenerationApplications such as conference transcription are crucial.I don't know.
![](https://assets-v2.circle.so/cqcutjipb078unn6sjfm30cfghp8)
### 2. Sensual voice activity detectionSemantic VADI'm not sure what I'm talking about.
**Background to the issue-**Background to the issue-The traditional system of dialogue must be judged.“At the end of the day,Is the user finished?I'm not sure what I'm going to do.It's usually through testing.“At the end of the day,Quiet for a while.It's not a good idea, it's not a good idea.Let's judge.I don't know.But this isn't a reliable method.——Humans often stop when they talk.Like thinking.This is the first time I've ever seen you.It's easy to misjudge.I don't know.
**Kyutai Solution-**Kyutai Solution-Kyutai STT  One is built.**Sensory-level speech activity detection module**Sensory-level speech activity detection module It doesn't just transcribe text. It also predicts whether the conversation is over or not.I don't know.

- **Basis of judgement-Voice content and synonyms**Basis of judgement-Voice content and synonymsInstead of being silent for a long time.);

- It's adapted to a different tone of speech. More intelligent.“At the end of the day,To determine whether or not it is the turn of the system to respond.); and

- The experiment will significantly enhance the nature of the conversation. Avoiding interruptions or prolonged failure to respondI don't know.

**I used to.**I used to.-Judgement“At the end of the day,Are you done?It's not a good idea, it's not a good idea.It's time to stop. For example, you're stopping. 1 sec The system thinks you're done.I don't know.
**Problem**Problem-Sometimes a man stops and doesn't talk. Like what?“At the end of the day,I want to eat.I'm sorry, I'm sorry.Hotpot.I'm not sure what I'm going to do.The system may have misjudged you.I don't know.
**Now.**Now.-Kyutai STT Use it. AI You're the judge of what you're talking about.**Semantics and semantics**Semantics and semantics Smarter judgment.“At the end of the day,Are you sure you're done?I'm not sure what I'm going to do.Higher rate of accuracyI don't know.

### 3. Very low delay

- stt-1b-en_fr-Delay 500ms

- stt-2.6b-en-Delay 2.5 secSacrifice part-time to improve accuracy.I'm not sure what I'm talking about.

**“At the end of the day,Flush SkillsIt's not a good idea, it's not a good idea.**“At the end of the day,Flush SkillsIt's not a good idea, it's not a good idea.-To further reduce the delay in response Kyutai I've used one.“At the end of the day,Let's go. Let's go.It's not a good idea, it's not a good idea.Mechanisms-

- After testing the user's speech, Immediate trigger model.**Speed up the remaining voice processing.**Speed up the remaining voice processing.

- Models 4 Finish the last part of the audio process at multiple real-time speed Only needed ~125ms

- The effect is to bring the voice system's response closer to instantaneous.

### 4. High-synchronous performance
Moshi Especially suitable for large-scale deployment The central advantage is that its model structure allows natural co-processing.-

- Yes. **NVIDIA H100 GPU**NVIDIA H100 GPU Could be supported. **400 It's voice flow processing at the same time.**400 It's voice flow processing at the same time.

- By comparison Whisper It's much more efficient to wait for traditional models. The latter requires complex collage.Like Whisper-StreamingI'm not sure what I'm talking about.and does not support batch processing I don't know. I don't know. I don't know.
![](https://assets-v2.circle.so/39bxzzbsx2au9nivdqet9uxnalm2)

### 5. Multi-platform realization support
Kyutai Delivery under multiple platforms provided To adapt to different use scenarios-
Realizing the platform Applied scene Characteristics PyTorch Research and experiments It's easy. Python Call in the environment Rust Production deployment StableIt's strong. Support WebSocket MLXAppleI'm not sure what I'm talking about. iPhone / Mac Use Apple Hardware acceleration Local Run

## Core technical principles-Delay current modellingDelayed Streams ModelingI'm not sure what I'm talking about.
It's different from tradition. Encoder-Decoder New methods The core ideas are as follows:-

- I think it's voice and text.**Two time-consorted data streams**Two time-consorted data streams;

- Text Streamed“At the end of the day,DelayIt's not a good idea, it's not a good idea.A few time frames. Allow Models**I see a little voice in the future.**I see a little voice in the future.To improve accuracy.;

- The audio stream stays the same. Models learn how to move from the audio stream.“At the end of the day,FillIt's not a good idea, it's not a good idea.Corresponding Text;

- Step in time in reasoning. No need for full audio;

Another advantage of this modeling is scalability.-

- We just need to adjust the flow order and alignment. That's what I'm gonna do. TTSText Synthesis);

- The current team is developing based on this architecture Text-to-Speech ModelI don't know.

## Summary of Model Strengths
Features Description **Low delay**Low delay As fast as you can. 500ms Fits for real-time voice interaction **High Precision**High Precision Close to or even superior to a non-fluent model. **High symmetry.**High symmetry. Support hundreds of roads and fluids. Suitable for deployment **Semantic Level VAD**Semantic Level VAD It's more intelligent to judge whether a word ends.It's more natural. **Multi-platform support**Multi-platform support Support for scientific researchProduction and mobile end deployment

- 🔗 Online experience-Unmute - Real-time voice conversation

- 📦 Model Files-
kyutai/stt-1b-en_fr @ Hugging Face

- kyutai/stt-2.6b-en @ Hugging Face

📁 Source Address-https://github.com/kyutai-labs/delayed-streams-modeling
Official presentation-https://kyutai.org/next/stt
