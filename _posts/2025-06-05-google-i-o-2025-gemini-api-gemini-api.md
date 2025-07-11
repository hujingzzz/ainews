---
layout: post
title: Google I/O 2025 General AssemblyGemini API Update Large Summary I know everything.Gemini API What upgrades have you made?
date: 2025-06-05 12:00:00 +0800
category: Frontier Trends
thumbnail: /style/image/google-i-o-2025-gemini-api-gemini-api_1.jpg
icon: image
---
* content
{:toc}

Google Yes. I/O 2025 It's published. **Gemini API and Google AI Studio**Gemini API and Google AI Studio A series of important updates. Coverage of model capacity expansionAudio and video input supportVisualization of the thinking processNew features such as browser automation controlsI don't know.
These updates have significantly enhanced the developers' ability to build the text.ImageAudioVideoCapacity for multi-model agentsI don't know.
**Gemini API**Gemini API Gradually developed into a complete multimodule intelligent platform Applies to audio conversations from code generationA wide range of scenes from web-based information to browser operating controlI don't know.Allow developers to call their state-of-the-art textImageAudio and video modelsI don't know.This update focuses on the following:-
**New models and voice upgrades**New models and voice upgrades
**Real-time music generation**Real-time music generation
**Multi-module input enhancementVideo comprehension, etc.I'm not sure what I'm talking about.**Multi-module input enhancementVideo comprehension, etc.I'm not sure what I'm talking about.
**Development of tools andAPIStructural updateIt's like a thought summary.Browser ControlAstral function callsI'm not sure what I'm talking about.**Development of tools andAPIStructural updateIt's like a thought summary.Browser ControlAstral function callsI'm not sure what I'm talking about.
**More efficient for developersModel access to the economyFor example, batch processing APII'm not sure what I'm talking about.**More efficient for developersModel access to the economyFor example, batch processing APII'm not sure what I'm talking about.
![](https://assets-v2.circle.so/kv57tyr4qmzos3g0w0zuwddvnt3o)
## Model update and capacity development

### 🧠 1. Gemini 2.5 Flash Preview New model

- **Version Identification-**Version Identification- gemini-2.5-flash-preview-05-20

- **Performance improvements-**Performance improvements- It's logical.Code GenerationLonger-term context treatment than for previous generationsI don't know.

- **Assessment of achievement-**Assessment of achievement- Yes. LMarena Second in the list. After Gemini 2.5 ProI don't know.

- **Efficiency gains-**Efficiency gains- Evaluation shows token Increased efficiency of use **22%**22%I don't know.

### 🔊 2. Gemini 2.5 Pro & Flash TTSText-to-VoiceI'm not sure what I'm talking about.

- **Support Language-**Support Language- More than **24Languages**24LanguagesI don't know.

- **Type of support-**Type of support- Single voicerIt's loud.multi-speakerThis is the first time I've ever seen you.Support**Emotion.Voice control.**Emotion.Voice control.I don't know.

- **Apply scene-**Apply scene- Create Pseudo-humanizationAIRoleMulti-wheel voice dialogue agentAudio Content Creation, etc.I don't know.

### 🗣️ 3. Gemini 2.5 Flash Original voice dialogue model

- **Function Features-**Function Features-
Provision30It's a different sound style.

- Auto-identify background from speaking person

- Respond to user tone/Emotional change

- Use“At the end of the day,Thinking ModelsIt's not a good idea, it's not a good idea.Complex logical processing

**Applied scene-**Applied scene-

- Call Center Smart Agent.

- Multi-role voice story.

- A voice-boggling personal voice assistant.

### 🎵 4. Lyria RealTime-Real-time music generation

- **Principles of work-**Principles of work- Pass. WebSocket Create real-time current connections Models generate music segments on an ongoing basisI don't know.

- **Method of control-**Method of control- Texttip Control Generation Style and RhythmI don't know.

- **Apply Example-**Apply Example- Google AI Studio Medium PromptDJ-MIDI Example applicationI don't know.

### 🧮 5. Gemini 2.5 Pro Deep ThinkDeep Thought ModeI'm not sure what I'm talking about.

- **Use-**Use- Experimental function For processing**Complex math and programming issues**Complex math and programming issuesI don't know.

- **Performance-**Performance- Longer chain of reasoning. Higher Precision For advanced code generation and logical resolutionI don't know.

### 💡 6. Gemma 3nLight multimodule modelI'm not sure what I'm talking about.

- **Deployment platform-**Deployment platform- It's for cell phones.Notebook.Edge devices such as tabletsI don't know.

- **Support Model-**Support Model- Text + Audio + ImageI don't know.

- **Technical architecture-**Technical architecture-
**PLEParameter Cache**PLEParameter Cache-Decrease the burden of reasoning by layer of cacheI don't know.

- **MatFormerStructure**MatFormerStructure-Reduce computational and memory costsI don't know.

## API Function Enhancement and Developer Tool

### 🧠 1. Thinking summaryThought SummariesI'm not sure what I'm talking about.

- **Use-**Use- The middle thought of extracting models in reasoningchain-of-thoughtThis is the first time I've ever seen you.Help developers understand model thinking pathsI don't know.

- **Presentation-**Presentation-
Title Category

- Tool Call Chain Presentation

- Show with the final answer

**Code ExamplePython:**Code ExamplePython:
from google import genai
from google.genai import types
client = genai.Client(api_key="GOOGLE_API_KEY")
prompt = "What is the sum of the first 50 prime numbers?"
response = client.models.generate_content(
model="gemini-2.5-flash-preview-05-20",
contents=prompt,
config=types.GenerateContentConfig(
thinking_config=types.ThinkingConfig(
thinking_budget=1024,
include_thoughts=True
)
)
)
for part in response.candidates[0].content.parts:
if part.thought:
print("Thought summary:\n", part.text)
else:
print("Answer:\n", part.text)

### ⚖️ 2. Thinking about the budget.Thinking BudgetsI'm not sure what I'm talking about.

- **Functions-**Functions- Control model when generating content“At the end of the day,Thinking.It's not a good idea, it's not a good idea.Depth Balance accuracy rateDelays and costsI don't know.

- **Apply-**Apply- Limitable token Usage Applicable to low-delayed scenarioI don't know.

### 🔗 3. URL Context Tools

- **Annotations-**Annotations- Models can automatically access relevant context information from specified web pagesI don't know.

- **Group Use-**Group Use- Can be associated with Google Search grounding Synergy of tools Enhancing research agent capabilitiesI don't know.

- **Usage-**Usage-

tools = [
Tool(url_context=types.UrlContext),
Tool(google_search=types.GoogleSearch)
]
response = client.models.generate_content(
model="gemini-2.5-flash-preview-05-20",
contents="Give me a 3-day schedule based on YOUR_URL...",
config=GenerateContentConfig(tools=tools)
)

### 🌐 4. Browser Automation ControlProject MarinerI'm not sure what I'm talking about.

- **Functions-**Functions- Control Browser Behavior If you click a buttonScroll PageFill out forms, etc.I don't know.

- **Modalities of deployment-**Modalities of deployment- But there's one key. Cloud Run Deployment Browser AgentI don't know.

- **Cooperative enterprises-**Cooperative enterprises- UiPathBrowserbaseAutomation Anywhere By the time we're involved in the early detection,I don't know.

### 📼 5. Video Understanding Update

- **Input Support-**Input Support- YouTube Video LinksDirectly Upload VideoI don't know.

- **Support Functions-**Support Functions-
Video summaryAnalysisTranslation

- Video CropExtract Snippet AnalysisI'm not sure what I'm talking about.

- Alignable Frame Rate0.1 ~ 60 FPSI'm not sure what I'm talking about.Support Game/High frame content such as sports

- Resolution Control-720p / 480p / 360p

### ⚙️ 6. Astral function callsAsync Function CallingI'm not sure what I'm talking about.

- **New Feature-**New Feature- Yes. Live API To achieve aneurysm Do not block dialogue main processI don't know.

- **Settings-**Settings- In Function Definition behavior Set Fields As NON_BLOCKINGI don't know.

### 🧾 7. Batch processing APIBatch APII'm not sure what I'm talking about.

- **Functions-**Functions- Support for sending multiple requests Maximum24Hour returns resultI don't know.

- **Advantages-**Advantages-
Cost is interactiveAPIHalf of it.

- Provide for higher rate limits

**Applied scene-**Applied scene- Large-scale analysisBatch Document ProcessingOffline assessment, etc.I don't know.

## On the whole.-

### ✅ Gemini API ♪ New ability to make it one ♪-

- Real multi-model unified interface

- Applies to light to heavy loads of equipment

- Cover AudioVideoImageWeb pageComplex interactive scenes such as text

- Support for more transparent and controlled model output and mind debugging

**Developer can.-**Developer can.-

- Fast Prototype Testing

- Build commercial smart agents

- Integrated VoiceVideoInput output for images etc.

- Create smart workflows using tool scheduling and automated control interfaces

### 🧩 Suggested scenes-

- Build voice dialogue robots

- Develop a video content summary tool

- Music generation creative applications

- Browser Automation Test Tool

- Research type AI Information Agent

Original-https://developers.googleblog.com/en/gemini-api-io-updates/
📚 View Developer documents to get more example codes andAPIGuide-https://ai.google.dev
