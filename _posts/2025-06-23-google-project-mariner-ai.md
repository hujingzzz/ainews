---
layout: post
title: Google Project Mariner：通过自然语言快速调度一个或多个 AI 智能代理，在浏览器环境中模拟人类完成执行复杂的任务
date: 2025-06-23 12:00:00 +0800
category: Frontier Trends
thumbnail: /style/image/google-project-mariner-ai_1.jpg
icon: web
---
* content
{:toc}

Project Mariner 是 DeepMind 针对未来 AI 自动化工作流推出的原型项目，它通过自然语言控制多个智能体在虚拟浏览器中同时执行任务。
✅ **核心目标**
该系统旨在让用户通过自然语言指令，快速调度一个或多个 AI 智能代理，在浏览器环境中模拟人类完成执行复杂的任务。
Mariner 名字的寓意来自于“航海者”，象征 AI 能够在信息的“海洋”中自主导航与执行任务。
✅ **任务类型**

- 信息检索（搜索、比对、筛选）

- 网页交互（点击、表单填写、滚动、复制等）

- 数据录入与整合（如从多个网页抓取结构化信息）

- 多任务调度（并发处理多个窗口或标签页）
00:00UnmuteMuteSettingsCaptionsDisabledQuality1080pSpeedNormalCaptionsGo back to previous menuQualityGo back to previous menu480pSD720pHD1080pHDSpeedGo back to previous menu0.5×0.75×Normal1.25×1.5×1.75×2×4×PIPExit fullscreenEnter fullscreenPlay

## 系统能力与工作方式

### 1. **语言驱动控制**
用户使用自然语言描述任务，系统将其转化为可执行的计划。例如：
“请帮我查找三家2023年提供AI课程的大学网站，并整理出课程名称、学费和官网链接。”
系统无需用户逐步指导，而是**自主理解任务结构并规划执行流程**。
![](https://assets-v2.circle.so/iidzbbb2btziubmdr1xu0kp7ajk7)
### 2. **虚拟浏览器操作环境**

- 所有任务操作均通过模拟真实用户行为在虚拟浏览器中完成；

- 智能体可进行 DOM 操作，如点击、输入、拖动、导航、提交表单等；

- 浏览器运行在沙箱中，支持任务隔离与并发运行。

### 3. **多任务并行调度**
Project Mariner 能够**并行执行多个子任务**（multi-agent concurrent execution）：

- 每个任务在独立浏览器实例中运行；

- 控制模块协调任务执行顺序、数据共享与进度跟踪；

- 可动态生成、终止或调整任务代理的行为。
00:00UnmuteMuteSettingsCaptionsDisabledQuality1080pSpeedNormalCaptionsGo back to previous menuQualityGo back to previous menu480pSD720pHD1080pHDSpeedGo back to previous menu0.5×0.75×Normal1.25×1.5×1.75×2×4×PIPExit fullscreenEnter fullscreenPlay

### **4.增强学习与任务反馈机制**

- 系统支持从用户反馈中进行学习。

- 引入奖励信号与回报机制优化任务执行策略。

详细了解：https://deepmind.google/models/project-mariner
See more