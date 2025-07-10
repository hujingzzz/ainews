---
layout: post
title: OpenAI has made four major updates to build AI proxy capabilities, add TypeScript support, human intervention mechanisms, new voice models.
date: 2025-06-16 12:00:00 +0800
category: Frontier Trends
thumbnail: /style/image/openai-ai-typescript_1.jpg
icon: link
---
* content
{:toc}

OpenAI has released four major updates, enhancing the ability to build AI agents, especially voice agents. Developers can now use TypeScript to write Agents SDKs while supporting human approval mechanisms, enhancing control and security. The newly launched RealtimeAgent allows voice agents to function easily on client or service end with advanced audio processing capabilities. Traces dashboards have also been upgraded to support Realtime API interactive visualization to facilitate calibration and analysis. The Speech-to-speech model has been significantly optimized to improve command compliance, tool accuracy, and can regulate voice broadcasting speed. **Key points**

- **Agents SDK Adds TypeScript Support**: has the same core functionality as Python (handoffs, guardrails, trading, MCP, etc.).

- **Human approval process**: Allows the inclusion of a “human review” mechanism in the tool call, which can be suspended, preserved, reviewed and restored.

- **RealtimeAgent **: Voice agents can be constructed on client or server to support tool calls, audio processing, interruptions, etc.

- **Trace dashboard upgrade**: Supports Realtime API voice session visualization, including input output audio, call process, and interruption of records.

- **Speech-to-speech model improvement**: Better follow instructions

- More stable tools to call.

- More reasonable interruptions.

- Adds speed parameters to control speech speed

** New model version published**:

- gpt-4o-realtime-preview 2025-06-03 (for Realtime API)

- gpt-4o-audio-preview 2025-06-03 (for Chat Commissions API)

## 1. Agents SDK supports TypeScript (development tool update)** notes**:

- OpenAI's Agents SDK now not only supports Python, but also adds the TypeScript version.

- Equivalent to the Python version, supporting the "primitives" required for all major construction agents:  handoffs: task relays and transfers between multiple agents

** Meaning**:

- The developers of the Web and Node.js ecosystems are more friendly.

- Easy to integrate into JavaScript applications, such as browser-end voice assistants, web-based smart clients, etc.[] [] (https://assets-v2.circle.so/gdishg1cqd 400xq3406xlph17wgv)

##  2. Support for the Human Review** (Human-in-the-lop) mechanism** ** Note**:

- Manual approval is allowed before proxy calls for external tools (e.g. functions, API).

- Support the following operating processes: **Pause tool implementation**

- **Serialize and save proxy status**

- ** Audit of the tool's call (accepted or rejected)**

- **Resumed proxy execution**

** Meaning**:

- Can be used for manual intervention in high-risk, sensitive tasks (e.g. finance, medical care, customer service complaints processing, etc.).

- Improving system reliability, compliance and transparency.

RealtimeAgent function: a new way to build a voice agent** ** Annotations**:

- RealtimeAgent is a high-level feature based on Realtime API to construct voice interactive agents.

- Runable on client or server, supported: Tool call (fundaction calling)

- Hand-over (handoffs)

- Security fences (guardrails)

- Automatic audio processing (playing, paused, interrupted)

- Real-time voice input and response

** Meaning**:

- Allow developers to define voice agents like build text agents.

- can be built for applications such as AI telephone service, voice search assistant, voice role play.[] (https://assets-v2.Circle.so/80bug2ystk2lzheh9qr4531km9gyq)

## **4. Trades dashboard upgrade: support voice session visualization** **Note**:

- Traces is a tool for debugging and monitoring proxy operations.

- The voice agent details in Realtime API can now be supported, including:  User voice input and model voice output  Tool call and parameter  breakpoint (e.g. user interruption)

** Meaning**:

- A more intuitive debugging experience, clearer problem positioning.

- Help developers optimize voice-interactive design and improve product stability.

## **5. Voice model GPT-4o functional upgrade**

- core upgrade of the speech-to-speech model: ** more reliable implementation of user instructions**

- **A more consistent tool call behaviour**

- ** More intelligent handling of interruptions and speed adjustments**

Add a new speed parameter to control the speed of voice play (e.g. slow read, quick play) ** model version**:

- Available version in Realtime API: gpt-4o-realtime-preview-2025-06-03

- Version in Chat Commissions API: gpt-4o-audio-preview-2025-06-03

# ** Field cases of multiple partners** ** Policy AI**:

- Use Realtime API to build voice question-and-answer assistants.

- A new model, with tools that are more precise and user-friendly.

**Intercom (Fin Voice)**:

- Build a call for AI service, support the automatic round-the-clock reception.

- The new model will better follow the script, reduce the number of “phantom” answers and improve the quality of services.

**Volley Gomes**:

- Build an AI-based RBG game experience based on a dungeon owner.

- The new model shows a stronger “rule consciousness” and a more imaginative narrative.

Links: https://openai.github.io/openai-agents-js/https://openai.github.io/openai-agents-js/guides/human-in-the-loop/