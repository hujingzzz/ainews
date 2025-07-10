---
layout: post
title: Kyutai team open-source real-time voice model Kyutai STT listens to text and you're smart enough to judge if you're done talking.
date: 2025-06-12 12:00:00 +0800
category: Frontier Trends
thumbnail: /style/image/kyutai-kyutai-stt_1.jpg
icon: chat
---
* content
{:toc}

** Kyutai STT** is an open source model developed by the Kyutai team specifically for ** real-time speech-to-text.** The main features of the scene are ** low delay, high accuracy, strong co-processing capacity**. ** Kyutai STT** not only can be written with low delay transliteration, but also designed for high-level and real applications (e.g. voice dialogue systems) with ** speech-level activity detection** capabilities. [https://assets-v2.circle.so/sg3ndph2svwjkmu83c480zonm33q] currently has two versions:

- kyutai/stt-1b-en_fr: English + French, low delay, suitable for interactive applications.

- kyutai/stt-2.6b-en: English, greater and more accurate, applicable to scenarios where accuracy is very demanding.

An earlier introduction to Kyutai introduced Unmute: it can be inserted into any model, giving voice to any model. iaoHu.AI Academy Kyutai launched Unmute, a highly modular voice AI system that can quickly add voice functions to any text large-language model (LLMM). That is, it can be inserted into any model, giving voice capability to the model. # core properties # https://www.xiaohu.ai/c/xiaohu-ai/kyutai-unmute! (https://assets-v2.circle.so/bmwwuzlqoxolm4m7xttlqyqo)

## 1. Fluid recognition: turning text while listening Kyutai STT supports** real fluid speech recognition**, i.e.:

- Audio-side input and processing without waiting for the end of the entire segment;

- Real-time return of transpositions containing ** punctuation symbols and word-for-word time stamp**;

- Accuracy of identification in comparison with non-current models (e.g. Whisper) can still be maintained at low delay.

This is critical for real-time voice assistants, live caption generation, conference transfers, etc. [https://assets-v2.circle.so/cqcutjipb078unn6sjfm30cfghp8] ##2.  Semantic VAD **Question Background: ** Traditional dialogue systems must judge whether “user has spoken”, usually by testing whether “user has spoken for a while.” This method is unreliable — humans often paused (e.g., thinkers) and liable to miscalculation. ** Kyutai solution: ** Kyutai STT has a ** semantic speech monitoring module that not only reproduces the text, but also predicts whether the speech is over.

- ** Based on: speech content and synonym** (rather than silence);

- Be able to adapt to different speech styles and be more intelligently “judge whether or not it is the turn of the system to respond”;

- The experiment significantly enhances the natural nature of the dialogue and avoids interruption or non-response for long periods of time.

** Before **: The judgment of “you're done” depends on the pause time, for example, when you stop for one second, the system thinks you're done.** ** ** ** The question: people sometimes stop and don't talk, for example, “I want to eat the pot of fire”, and the system may have misjudged you. ** ** Now: Kyutai STT uses AI to judge the semantic and semantic tone of your speech**, and more intelligently to judge “you're really done” and the accuracy rate is higher.

#3. Very low delay

- st-1b-en_fr: delay 500ms

- st-2.6b-en: Delay 2.5 seconds (save part of real time to improve accuracy)

** “Flush technique”**: To further reduce the delay in response, Kyutai used a “accelerated flushing” mechanism:

- Trigger the model immediately after the user's speech has been tested** to speed up the processing of the remaining voice**

- The model completes the final part of the audio process at 4 times real speed, only ~125ms

- The effect is to bring the voice system's response closer to instantaneous.

##4. High-complex performance Moshi is particularly suitable for large-scale deployment, with the core advantage that its model structure allows natural co-processing:

- Supportable on **NVIDIA H100 GPU** **400 simultaneous voice flow processing**

- Much more efficient than traditional models such as Whisper, which requires complex collage (e. g. Whisper-Streaming) and does not support batch processing, which has a poor capacity to swallow![] (https://assets-v2.Circle.so/39bxzzbsx2au9nivdqet9uxnalm2)

##5. Multi-platform realization support Kyutai provides multiple platform implementations to accommodate different use scenarios: achieve platform application scenario characteristics PyTorch research and experiments easy to call Rust production deployment in Python environment stability and performance support WebSocket MLX iPhone / Mac use Apple hardware to speed up local operations

# Core technical doctrine: Delayed Stream Modeling, a new approach different from traditional Encoder-Decoder, with the following core ideas:

- View voice and text as ** two-time data streams**;

- Text flow is “delayed” by several time frames, allowing the model** to see the sound of the next point** in order to improve accuracy;

- Audio flow remains unchanged, and model learning on how to “fill” the corresponding text over time from the audio stream;

- Modality in reasoning, without the need for full audio;

Another advantage of this modeling approach is expansionability:

- TTS (synthesis of speech) can be achieved only by adjusting the flow order and alignment;

- The current team is developing the Text-to-Speech model based on this structure.

# Model Sufficiency Summary Characteristic Description ** Low Delay** Fast 500 ms for real-time voice interaction ** High Precision** Near or even Better than Non-fluent Model ** High Synergy** Support for hundreds of routes and flow processing, Fit for deployment ** Semantic VAD** Determining whether speech ends with more intelligent and natural ** Multiplatform Support** Support for scientific research, production and mobile end deployment

Online experience: Unmute - real-time voice conversation

-  Model file: kyutai/stt-1b-en_fr@Huging Face

- kyutai/stt-2.6b-en @Huging Face

Source address: https://github.com/kyutai-labs/delayed-streams-modeling