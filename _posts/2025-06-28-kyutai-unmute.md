---
layout: post
title: Kyutai 推出了 Unmute：它可以插入到任意的模型当中，让任意模型具有语音能力
date: 2025-06-28 12:00:00 +0800
category: Frontier Trends
thumbnail: /style/image/kyutai-unmute_1.jpg
icon: game
---
* content
{:toc}

Kyutai 推出了 **Unmute**，一个高度模块化的语音 AI 系统，可以为任何文本大语言模型（LLM）快速添加语音功能。
也就是它可以插入到任意的模型当中，让该模型具有语音能力。
00:00UnmuteMuteSettingsCaptionsDisabledQuality1080pSpeedNormalCaptionsGo back to previous menuQualityGo back to previous menu480pSD720pHD1080pHDSpeedGo back to previous menu0.5×0.75×Normal1.25×1.5×1.75×2×4×PIPExit fullscreenEnter fullscreenPlay
- Unmute 包括新的 **语音识别（Speech-to-Text）** 和 **语音合成（Text-to-Speech）** 模块：
**流式识别**，低延迟，具有语义级别的语音活动检测（VAD），能智能判断用户是否说完一句话。

- **TTS 支持个性化语音克隆**，基于 10 秒语音样本生成定制声音。

- TTS 实现“文本流式”合成，支持在文本尚未完全生成时开始说话，进一步降低响应延迟。

00:00UnmuteMuteSettingsCaptionsDisabledQuality1080pSpeedNormalCaptionsGo back to previous menuQualityGo back to previous menu480pSD720pHD1080pHDSpeedGo back to previous menu0.5×0.75×Normal1.25×1.5×1.75×2×4×PIPExit fullscreenEnter fullscreenPlay去年推出的 Moshi 虽然具备低延迟和自然语言能力，但在函数调用、推理能力、上下文学习等方面不如文本模型。Unmute 旨在弥补这一点，把文本模型的强大能力带入语音对话。

- **系统结构**：Unmute 是一个**级联式语音系统**，由三个独立模块组成：
**语音转文本（STT）**：将用户的语音内容转录为文本。

- **语言模型（LLM）**：这里使用的是 **Gemma 3 12B**，基于输入文本生成响应。

- **文本转语音（TTS）**：将 LLM 的响应转换为语音。

- **模块化优势**：
虽然这种级联系统可能丢失情绪、讽刺等语境信息，但其最大的优点是**高度模块化**。

- 因为三个组件是独立的，所以你可以**为任何 LLM 添加语音功能**，无需微调或适配。

- 在演示中，用户可以：
调整 **Gemma 3 的 system prompt**，以自定义数字角色的“性格”；

- 独立改变 TTS 的声音，实现人物个性与语音的自由组合。

**技术细节**：

- **STT 是流式的**，集成了**语义级语音活动检测（semantic VAD）**，无需额外模型判断说话是否结束，低延迟。

- **TTS 也是流式的**，不仅在音频生成上是流式的，甚至在文本生成过程中就开始发声，从而极大降低响应时间。

- 用户只需提供 **10 秒语音样本**，就可以自定义 TTS 的音色与语调。

00:00UnmuteMuteSettingsCaptionsDisabledQuality1080pSpeedNormalCaptionsGo back to previous menuQualityGo back to previous menu480pSD720pHD1080pHDSpeedGo back to previous menu0.5×0.75×Normal1.25×1.5×1.75×2×4×PIPExit fullscreenEnter fullscreenPlay
- Unmute 的语音交互设计支持 **打断、轮流发言（turn-taking）**，更贴近自然人类对话。

- **未来方向**：Kyutai 坚信人机交互的未来在于“自然、全双工语音交互 + 个性化 + 可扩展能力”。

- 官方承诺将在未来几周内将 Unmute 的全部内容 **开源**。

在线体验：unmute.sh
See more