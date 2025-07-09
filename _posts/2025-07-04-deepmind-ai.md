---
layout: post
title: Deepmind 推出新一代机器人AI模型 它可以在机器人本体上独立运行 无需依赖云端计算资源
date: 2025-07-04 12:00:00 +0800
category: Frontier Trends
thumbnail: /style/image/deepmind-ai_1.jpg
icon: game
---
* content
{:toc}

Deepmind 推出新一代 Gemini Robotics On-Device 机器人AI模型，它可以**在机器人本体上独立运行**，无需依赖云端计算资源。该模型整合了视觉、语言理解和动作决策能力，能够完成高度灵巧且多变的实际任务。
✅ **它解决的核心问题：**

- **减少对云计算的依赖** → 降低延迟，提升响应速度。

- **在网络不稳定环境下正常运行** → 提高可靠性。

- **实现通用操作能力和快速适应新任务** → 提高机器人通用性。

**Gemini Robotics机器人模型 **最早于2025年3月推出，基于Gemini模型，结合视觉、语言与动作（VLA）的能力，引入物理世界的操作推理。
![](https://assets-v2.circle.so/0p2ci3src0jg5k3qdfecah25nkhn)
## 模型能力：它能做什么？
![](https://assets-v2.circle.so/dgiokkn48zb7b75r6y954a4prehh)00:00UnmuteMuteSettingsCaptionsDisabledQuality1080pSpeedNormalCaptionsGo back to previous menuQualityGo back to previous menu480pSD720pHD1080pHDSpeedGo back to previous menu0.5×0.75×Normal1.25×1.5×1.75×2×4×PIPExit fullscreenEnter fullscreenPlay
## 技术特点
📌 1. 本地部署优化

- 模型进行了**计算资源压缩优化**，使其可以运行在算力受限的机器人设备上。

- 不需要 GPU 服务器，CPU 或小型AI芯片也能支持推理。

📌 2. 多模态整合能力

- 基于 DeepMind 的 Gemini 2.0 模型结构，集成了视觉、语言和行为控制。

- 具备**图像感知 + 指令理解 + 动作执行**的一体化能力。

📌 3. Few-shot 微调机制

- 支持极少样本（仅50~100条演示）下完成新任务适应，这大幅降低开发和部署门槛。

### 表现到底怎么样？
✅ 在多项测试中，表现优于现有模型：

- **任务完成率更高**：特别是在之前没见过的任务或新环境中，模型展现出更强的泛化能力。
![](https://assets-v2.circle.so/gfm4bayqbl47ft4fk5i614p8u2n2)
- **指令遵循：**在更具挑战性的分布外任务和复杂多步骤指令上也优于其他本地替代方案。
![](https://assets-v2.circle.so/zaxjzqrcht2tv6j648oiajud96j2)
- **响应更快**：得益于本地运行，无需等云端返回结果。

- **执行更稳定**：在不同机器人平台上也能维持较高的一致性表现。

**📈 实验任务示例：**
![](https://assets-v2.circle.so/mjbfvr6hf0e52znqr5wee7ngr3b0)
### 适配能力：不仅能运行，还能跨平台

- 在 ALOHA 平台训练后，迁移到：
**Franka FR3 双臂机器人**：完成工业级别装配任务。
00:00UnmuteMuteSettingsCaptionsDisabledQuality1080pSpeedNormalCaptionsGo back to previous menuQualityGo back to previous menu480pSD720pHD1080pHDSpeedGo back to previous menu0.5×0.75×Normal1.25×1.5×1.75×2×4×PIPExit fullscreenEnter fullscreenPlay
- **Apollo 仿人机器人**：在家庭/服务类环境中执行自然语言操作。
00:00UnmuteMuteSettingsCaptionsDisabledQuality1080pSpeedNormalCaptionsGo back to previous menuQualityGo back to previous menu480pSD720pHD1080pHDSpeedGo back to previous menu0.5×0.75×Normal1.25×1.5×1.75×2×4×PIPExit fullscreenEnter fullscreenPlay
👉 值得注意的是：这类跨平台迁移**无需重新训练模型**，只需轻微调整，即可使用相同的智能能力。
![](https://assets-v2.circle.so/dfl0wl73hm3c5nr9330vnrj0zcva)
### 开发者支持：如何参与与使用？
![](https://assets-v2.circle.so/pgc6wk4pzcdxm0qj7v157acafob3)MuJoCo
Gemini Robotics SDK
Gemini Robotics tech report
**Gemini Robotics On-Device 标志着机器人AI迈入“可用”、“可部署”、“可泛化”的新阶段。**
它具有的意义包括：

- ✅ **边缘智能普及化**：机器人可以独立思考、执行任务，不再依赖外部服务器。

- ✅ **部署成本下降**：适应性强 + 快速微调 → 降低行业应用门槛。

- ✅ **跨硬件统一模型架构**：未来可实现一个模型适配各种形态的机器人设备。

官方介绍：https://deepmind.google/discover/blog/gemini-robotics-on-device-brings-ai-to-local-robotic-devices/
See more