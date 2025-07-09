---
layout: post
title: Google 发布了一种全新的 AI 编码代理：AlphaEvolve 它可以自己写代码、自己评估测试、然后自己自我改进
date: 2025-06-05
category: Frontier Trends
thumbnail: /style/image/google-ai-alphaevolve_1.jpg
icon: book
---
* content
{:toc}

Google DeepMind发布了一种全新的 AI 编码代理：AlphaEvolve，它可以自动优化算法并进行科学发现
**AlphaEvolve** 的核心定位是：
**一个基于大语言模型（LLMs）+ 进化算法 + 自动评估器的通用算法发现与优化平台。**
它不仅能写代码，还能自动评估这些代码的表现，然后根据评估结果调整策略、迭代生成更好的方案。这一过程本质上是**模拟“算法自然进化”**。

### 它厉害在哪里？

- 不需要人类一步步写优化方案，它**自己想改法、自己测试、自己改进**。

- 比其他AI更强的是，它可以修改**整段程序**，不是只改一两个小函数。

- 它能学会在不同问题下用不同策略，比如复杂问题用搜索算法，结构化问题用构造法。

- 成果已经**真实投入Google大规模生产使用**，不是实验室玩具。

可以理解为它是一个超级“AI程序员”，它能：

- 自动写代码解决复杂问题；

- 自己测试自己的代码；

- 如果效果不好，自动改进并尝试新方法；

- 最终像“进化论”一样，筛选出最优秀的算法方案。

它已经被用在：

- 提高谷歌数据中心效率；

- 加速AI模型训练；

- 帮助数学家解决难题；

- 甚至给芯片设计师提供Verilog代码建议！

**举个例子！**
它解决了一个50多年没人改进的问题——如何最有效地做“4×4矩阵乘法”。旧方法需要49次乘法，它发现了只用48次的新方法！

## AlphaEvolve 与以往 AI 系统的根本区别
![](https://assets-v2.circle.so/h2nns3bbkqxbdlgsr905q3mgz5xy)**通用性**： 

- 与 DeepMind 之前的 AlphaFold（专为蛋白质折叠）或 AlphaTensor（专为矩阵乘法）不同，AlphaEvolve 是通用 AI，可应用于任何可表达为代码且可自动评估的问题。

- 其“搜索算法而非直接搜索解”的方法使其适用于广泛领域，从数学到系统优化。

## 工作机制详解
AlphaEvolve 不是简单地依靠单一语言模型完成任务，而是一个**多组件、多阶段联动系统**，包含以下核心模块：
![](https://assets-v2.circle.so/qtvapq4duz6hexbd36utghclgpbi)
### 系统结构
AlphaEvolve 的整体流程由多个模块组成，彼此协同构建了一个 **进化式自动算法设计系统**：
**1. 输入阶段**
用户提供：

- 初始程序代码；

- 需要优化的问题定义；

- 自动化评估函数（如代码性能、输出正确性等）。

**2. 核心模块构成**
🧩 Prompt Sampler（提示构建器）

- 组合历史优秀方案 + 问题上下文，构建复杂 prompt；

- 支持人类提供的背景知识、公式、代码片段等；

- 还能生成“元提示”（meta-prompts）来优化生成质量。

🤖 LLM Ensemble（LLM集成）

- 使用 Gemini Flash 快速生成大量候选程序；

- 使用 Gemini Pro 深度优化关键建议；

- 共同驱动“进化”过程，提出多样化代码修改建议。

🧪 Evaluators（自动评估器）

- 自动运行并评估每个程序在任务中的表现；

- 支持多指标优化、级联评估、并行分布式执行；

- 可附加 LLM 辅助判断（如程序可读性、简洁性等）。

📦 Program Database（程序数据库）

- 储存历史方案、评估分数、修改记录；

- 用于构造新一代 Prompt，实现类似“遗传记忆”的演化。

### **进化算法（Evolutionary Loop）**
AlphaEvolve 的核心是 **LLM驱动的“进化式搜索”**：

- 选择一个“父程序”，从数据库中提取其最优结构；

- 通过 Prompt 构建当前任务和上下文；

- LLM 生成新的代码差异（diff）；

- 应用差异形成“子程序”；

- 用评估器跑结果、打分；

- 如果子程序优于父程序，入库，下一轮进化继续。

这一过程不仅演化代码，还可以演化 prompt 本身、评价指标等，实现高度自适应的搜索优化。

- 将表现最好的代码片段“保留下来”，用于下一轮生成的输入；

- 系统也会引入“变异”——对已有代码进行小幅调整尝试新解；

- 这一过程会不断迭代优化，直至产生最优解或新颖有效的算法。

## 已落地的应用与成果
AlphaEvolve 已不只是研究原型，而是已经**部署在真实生产系统中并产生了明显成效**。几个关键应用场景如下：

### ✅ 数据中心调度优化（Google Borg 系统）

- 为 Google 的 Borg 集群管理系统设计了一种调度启发式算法，已投入使用超一年，**可持续回收约 0.7% 的计算资源**

- 解决了“搁浅资源”问题（例如内存耗尽但 CPU 仍可用）。

- 生成的代码简单且人类可读，便于工程师调试和部署。
![](https://assets-v2.circle.so/j9nc9a8ewjzqd1miq145xkjb0817)

### ✅ AI 芯片设计协同（Verilog级别）

- 对 Google TPU 中的某个矩阵乘法电路进行了 Verilog 级别的重写，去除冗余位，保持功能正确性；

- 这一建议已被采纳进入未来一代芯片设计流程中，显著节省面积与能耗。
![](https://assets-v2.circle.so/t1b7kmis84mjantvb6ttego7lzz8)

### ✅ AI 模型训练加速（包括 Gemini 自身）

- 优化了 Gemini 模型训练中的矩阵乘法内核，加速 23%，整体训练时间缩短 1%，在 Google 的计算规模下节省了大量能源和资源。

- 对 FlashAttention 内核的低级 GPU 指令进行重构，速度提升达 **32.5%**。

### ✅ 数学与算法发现

- 在 50 个数学问题（涵盖几何、组合数学等领域）的测试中，AlphaEvolve 在 75% 的情况下重现了已知最优解，在 20% 的情况下发现了优于已有解的新解。
![](https://assets-v2.circle.so/xatol7vw96fyyyo3u9phpuf852we)
- **接触球数问题**：在 11 维空间中，将接触球数（非重叠单位球体可同时接触中心球体的数量）的下界从 592 提高到 593，打破了现有记录（上界为 868）。
![](https://assets-v2.circle.so/3qlxo3a8gljxk5ujnhnibwt6n3rp)
- **矩阵乘法**：发现了比 1969 年 Strassen 算法更高效的 4×4 复数矩阵乘法算法，减少了标量乘法次数，提升了计算效率。
00:00UnmuteMuteSettingsCaptionsDisabledQuality1080pSpeedNormalCaptionsGo back to previous menuQualityGo back to previous menu480pSD720pHD1080pHDSpeedGo back to previous menu0.5×0.75×Normal1.25×1.5×1.75×2×4×PIPExit fullscreenEnter fullscreenPlay

官方介绍：https://deepmind.google/discover/blog/alphaevolve-a-gemini-powered-coding-agent-for-designing-advanced-algorithms/ 
技术报告
See more