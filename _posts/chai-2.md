---
layout: post
title: Chai-2：自动设计抗体模型 能“从零开始”理解并设计新的抗体
date: 2025-06-24
category: Frontier Trends
thumbnail: /style/image/chai-2_1.jpg
icon: game
---
* content
{:toc}

- 传统抗体发现依赖动物免疫或大规模文库筛选，效率低、成本高，且对某些难靶标无效。

- 现有的AI抗体设计方法（如RFdiffusion）在实验命中率（hit rate）通常低于 0.1%，难以脱离高通量筛选。

Chai Discovery 团队发布了一个叫 **Chai-2** 的新AI模型，用来**设计抗体分子（**抗体是用来对抗病毒、癌症等的药物成分**），**也就是医学和生物技术中常用的特殊蛋白质。
Chai-2 的关键特点是 零样本学习（zero-shot） 和 高命中率设计，对抗体设计领域带来了重大突破。
即模型不需要对每一个新的抗体设计目标进行大量的训练数据输入。它能“从零开始”理解并设计新的抗体，只要给定一个目标蛋白，它就能通过已有的知识生成有效的抗体。
它利用多模态生成架构，结合原子级结构预测和生成建模，实现了“零样本”抗体设计。Chai-2 可在没有迭代实验的前提下，仅用两周时间完成从目标设定到分子生成、合成与验证的完整流程，且命中率超过 15%，远超行业标准。该成果显示分子工程正从依赖经验的方法转向可控、确定性的生成策略。
00:00UnmuteMuteSettingsCaptionsDisabledQuality1080pSpeedNormalCaptionsGo back to previous menuQualityGo back to previous menu480pSD720pHD1080pHDSpeedGo back to previous menu0.5×0.75×Normal1.25×1.5×1.75×2×4×PIPExit fullscreenEnter fullscreenPlay**它厉害在哪里？**

- **不需要反复实验**：传统的抗体设计要反复试错，他们这个模型只要一次输入，就能设计出很多有效的分子。

- **效率超级高**：原来可能需要几个月甚至几年做的事，他们**两周就能搞定**。（提升超 100 倍）。

- **命中率不错**：测试 50 个目标，最终有超过 15% 的分子“命中”成功，已经很高了。

- **在miniprotein设计中达到了68%的实验命中率**，并可达皮摩尔（picomolar）亲和力。

- **靠AI就能做**：他们用的是一个非常先进的AI系统，不光理解分子的结构，还能“自己想出来”怎么设计。

**未来应用与愿景**

- 可望实现按需生成**表位特异性结合体**，促进双特异抗体、抗体药物偶联物等复杂疗法的快速开发。

- 支持设计非传统生物药物如**环肽、酶、小分子**等。

- 致力于将生物学转变为“工程学”——从经验性发现迈向**可控、可编程的分子设计**。

## Chai-2 模型

### 模型架构

- **多模态全原子生成模型（Multimodal All-atom Generative Model）**

- 两个核心子模块：
Chai-2d: 设计子模块，用于从目标蛋白和表位直接生成抗体序列和结构。

- Chai-2f: 折叠子模块，用于预测蛋白三维结构、评估结合质量。

**全原子级别设计**：不仅考虑氨基酸序列，还考虑空间结构与结合界面原子级互补
00:00UnmuteMuteSettingsCaptionsDisabledQuality1080pSpeedNormalCaptionsGo back to previous menuQualityGo back to previous menu480pSD720pHD1080pHDSpeedGo back to previous menu0.5×0.75×Normal1.25×1.5×1.75×2×4×PIPExit fullscreenEnter fullscreenPlay
### 🧬 支持多种设计格式

- VHH（单域抗体）

- scFv（单链可变片段）

- mini蛋白（非抗体但能结合靶标的小型蛋白）

### 功能亮点
![](https://assets-v2.circle.so/p1eqau2159i5vg17n3bxtchnz9eu)
## 实验结果与评估
通过一次性输入 50 个靶标，Chai-2 生成分子，实验命中率超 15%，整个流程仅需 2 周，无需迭代优化或高通量筛选。
![](https://assets-v2.circle.so/5xioicrmyvc5g03jebu2h9xnwmij)Chai-2 在 **抗体设计** 和 **mini蛋白设计** 两个方向上均进行大规模实验验证。

### 🧪 抗体设计任务
实验设置：

- 52个全新目标蛋白（无现成抗体记录）

- 每个靶点最多设计并测试20个抗体（scFv或VHH格式）

- 实验方法：Bio-Layer Interferometry（BLI）测定结合能力与亲和力（KD）

![](https://assets-v2.circle.so/973noy1gb5dcasbv27fbonmecct9)
- 相比传统抗体生成方法（<0.1%命中率），提升 **两个数量级以上**。

- 所有设计仅通过**一次实验轮次**完成验证，无需迭代筛选。

### mini蛋白设计任务

- 目标数：5个，包括 PD-L1、IL7Ra、InsulinR、PDGFRβ 和 TNFα。

- 实验：每个目标设计20-25个mini蛋白，使用BLI测定。

命中情况与亲和力示例：
![](https://assets-v2.circle.so/2dweftoxm87joqagoys6os999iye)
- 平均命中率 **>68%**

- TNFα 为结构难度极高靶标，为首次成功的AI设计命中。

## 为什么他们的成功率这么高？
因为 Chai-2：

- **不仅设计结构，还预测效果**：它不是瞎猜，而是结合三维结构模拟和筛选。

- **能设计不同种类的抗体**：包括常见的小型抗体（scFv）、骆驼抗体（VHH）、迷你蛋白（miniproteins）等。

- **可以控制细节**：可以指定目标的位置、抗体的样式，甚至能设计同时作用于**人类和动物**的抗体（跨种属设计）。

### 举几个例子说明：

### ✅ 案例1：对抗TNFα（一个非常难的目标）

- TNFα 结构复杂，以前从未有AI成功为它设计出结合物。

- Chai-2 设计出的抗体**成功粘住了它**，而且是首次实现！

### ✅ 案例2：抗体“双版本”设计

- 对同一个目标蛋白（CCL2），Chai-2 分别设计了两种抗体（scFv 和 VHH），靶向不同位置，结果**两个都成功了**！

### ✅ 案例3：跨物种抗体

- 科学家让 Chai-2 设计能同时结合人类和猴子的同一种蛋白。

- 结果真做到了：设计出的抗体能同时“粘住”两种物种的目标蛋白。

###  他们还做了哪些检查来确保抗体“靠谱”？

- ✅ **专一性检查**：抗体只粘它应该粘的目标，不乱粘别的蛋白。

- ✅ **安全性指标**：AI会提前评估设计是否有可能引发免疫反应（免疫原性）。

- ✅ **稳定性评估**：是否容易变性或聚集，这关系到能不能做成药。

如需使用 Chai-2，请访问：https://www.chaidiscovery.com/product 
技术报告：https://chaiassets.com/chai-2/paper/technical_report.pdf
See more