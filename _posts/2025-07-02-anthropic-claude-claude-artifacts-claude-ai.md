---
layout: post
title: Anthropic Claude 推出Claude Artifacts创作空间和应用发布分享功能
date: 2025-07-02 12:00:00 +0800
category: Frontier Trends
thumbnail: /style/image/anthropic-claude-claude-artifacts-claude-ai_1.jpg
icon: web
---
* content
{:toc}

Anthropic 宣布为 Claude 推出两种全新创作方式：
**Artifacts创作空间：**用户可以在里面创建、保存和分享他们用Claude做出来的东西。比如，你可以用Claude创建一个节奏机器（就像视频里展示的），然后分享给别人。
**嵌入AI能力：**当你创建这些东西时，Claude的AI能力可以直接被嵌入到里面，无需申请API，而且你可以直接发布分享你创建的应用。比如你创建一个学习工具，Claude的AI可以根据用户的技能水平提供个性化的辅导或答案。当你分享这些嵌入AI能力的作品时，其他人可以通过他们的Claude账户使用。这些使用会计入他们的订阅，而不是你的。这样，创建者和用户之间的成本和使用权得到了平衡。
00:00UnmuteMuteSettingsCaptionsDisabledQuality1080pSpeedNormalCaptionsGo back to previous menuQualityGo back to previous menu480pSD720pHD1080pHDSpeedGo back to previous menu0.5×0.75×Normal1.25×1.5×1.75×2×4×PIPExit fullscreenEnter fullscreenPlay
## Artifacts 创作空间

### 什么是 Claude Artifacts？
Claude Artifacts 是由 Anthropic 推出的交互式 AI 应用构建模块，可以理解为在 Claude 聊天界面中生成的**带有 Claude 智能能力的可运行“微应用”或原型系统**。
**特点：**

- **无需部署或写代码**：不需要配置 API Key，也不需要担心部署服务器或调用计费。

- **本地运行 + 快速分享**：直接在 Claude 界面运行，点击发布即可分享他人试用。

- **具备一定的逻辑和交互性**：虽然是轻量级原型，但可以响应用户输入，执行基本逻辑操作。

### **主要功能**

- 提供一个集中的界面，管理所有 Claude 生成的项目和创作。

- 用户可以**浏览精选示例（curated examples）**。

- 所有 Artifact 项目都可以被**“fork”** —— 即复制并进行个性化修改。

- 包括多种模板，如游戏、闪卡、编程工具、创意练习等（从截图和视频中可见）。
![](https://assets-v2.circle.so/6l66pijrmzdswmikwl0jidklo6an)

- **使用场景**
教育应用：生成可互动的学习工具

- 编程学习：快速搭建代码小工具或演示项目

- 创意写作与游戏设计：设计 AI 参与生成的互动内容

## 嵌入 AI 能力到创作中
Artifacts 内部已经集成 Claude 模型，无需再申请 API Key 或构建后端服务。你使用 Claude 的 Artifact 实际是在调用模型本身的推理能力，只要你在 Claude 平台内操作，调用的额度归属于你的账号，不再单独计费。

- **核心功能**
用户可以利用 Claude 的智能，**直接在作品中嵌入 AI 功能**，创建功能性 AI 应用。

- 应用发布后，使用者需使用自己的 Claude 账户登录，**从而实现计费独立（不会占用原作者的 token 或额度）。**

- ✅ 举个例子：
假设你用 Claude Artifacts 做了一个“AI 情绪分析小工具”，并发布生成了一个链接：
你发给朋友A；

- 朋友A点击链接后，会登录自己的 Claude 账户；

- 朋友A开始输入文本，Claude 分析情绪并返回结果；

- **这些操作消耗的是朋友A自己的订阅额度，而不是你的**。

**特点**

- 支持全功能 App 构建，使用 Claude 的能力作为“后端智能核心”。

- 面向创作者、开发者和想要部署 AI 应用的个人。

- 类似“AI 即服务”的形式，原作者无需承担运行成本。

### 如何启用

- 所有 Claude 的 **Free、Pro 和 Max 用户** 均可开启该功能。

- 操作方式：进入 Claude 设置，**开启“Create AI-powered artifacts”** 的测试功能。

- 入口：https://claude.ai/artifacts

## 使用 Claude Artifacts 原型开发 AI 应用指南

## **如何快速构建、测试和分享基于 Claude 的 AI 应用**
过去我们总觉得做一个 AI 应用是很麻烦的事：你得搞 API 密钥、设置服务器、算清成本、处理限流，还要小心别踩坑。现在，有了 **Claude 的 artifacts（作品面板）功能**，一切都变得轻松了许多。
这玩意儿就像是 Claude 里的“小程序引擎”——不需要部署服务器，不需要 API 密钥，Claude 自带“魔法接口”，你直接用 prompt 就能让它动起来，想做点什么就马上开始试，做完还能一键分享。
00:00UnmuteMuteSettingsCaptionsDisabledQuality1080pSpeedNormalCaptionsGo back to previous menuQualityGo back to previous menu480pSD720pHD1080pHDSpeedGo back to previous menu0.5×0.75×Normal1.25×1.5×1.75×2×4×PIPExit fullscreenEnter fullscreenPlay
## ✅ 第一步：打开 Claude 的“AI 应用模式”
打开 Claude 网站，在设置里打开“Create AI-powered artifacts（开启 AI 应用功能）”；
开完之后，Claude 就能识别你想创建的是一个具备 AI 能力的应用原型，而不是单纯的对话；
举个栗子，你可以直接说：“帮我做一个聊天机器人，每次用户说什么，它就夸对方一句”。

- 解析你的意图

- 自动生成带交互功能的 Artifact（可点击右侧面板查看）

- 允许你与 Artifact 进行测试互动

### 🧠 提示设计建议：

- 清晰表达输入和期望输出

- 说明是否需要多轮对话、格式约束、风格等

- 示例：“用户输入一句话，Claude 返回一句温柔鼓励并标注情绪类型（Positive / Neutral / Negative）。”

## 🧪 第二步：测试与迭代你的 Artifact
1. 实时测试
在右侧 Artifact 面板输入内容，观察响应是否符合预期。
✏️ 2. Fork & Edit（创建分支迭代）
对结果不满意？可以：

- 回到任一对话记录，点击“Edit”

- 修改 Prompt 或描述，生成一个新版本 Artifact

- 支持多版本并行测试，不影响原始版本

### ⚠️ 注意：
Claude 的 Artifact 目前支持 **文本补全逻辑**，适合内容生成、分类、总结、对话模拟等类型的 AI 应用。

## 不知道做什么？来几个灵感方向
Claude 支持的 artifacts 不止是工具，也可以是创意作品。你可以从这些方向开始玩起：

- **教学类小助手**：如交互式导师或学习伴侣，能理解用户学习需求的上下文。例如：一个可依据预设风格和最佳实践提供详细反馈的代码审查助手；或一个语言学习工具，让你用首选语言聊天和练习。
![](https://assets-v2.circle.so/m5w4dl6kn6gieaxu56tthzppruku)
- **内容生成工具**：协助头脑风暴、开发和润色创作内容的助手，减少重复劳动。例如：将内部 Slack 帖子整理为适合发到 LinkedIn 的文案，或将输入转化为一页的产品需求文档（PRD）。
![](https://assets-v2.circle.so/dekzeq80o34it77xblftos5ktuy3)
- **分析与决策支持工具**：处理用户数据并通过对话支持决策的智能工具，提升组织效率。例如：基于“5 个为什么”框架帮助团队深入剖析问题的助手。
![](https://assets-v2.circle.so/y5p6rwenwvx2bauebt0k6r2oizhk)
- **灵感创意类**：最棒的应用往往源自奇思妙想和独特视角。比如解梦机器、恋爱语录生成器、电影名推荐器……你脑洞够大，Claude 就能帮你落地。
![](https://assets-v2.circle.so/0cp1x13e8eqgcpyfyygngyrarxkv)

## 📤 第三步：发布并分享你的 AI 应用
Claude artifacts 是为「原型设计」而生的，不需要你搭服务器或者注册 API key，点一下「Publish」，你就可以生成一个链接，发给朋友、同事，甚至贴在社交平台。

- 别人打开后就是你的当前版本；

- 对方可以复制和改造，不会影响你的原始代码；

- 你也可以随时取消分享或者管理分享的作品。
![](https://assets-v2.circle.so/azlyd3b9hlbcbzv4chb0l4xvjppe)
1. 点击“Publish”发布应用
Artifact 面板右上角有“Publish”按钮，点击即可生成唯一访问链接。
2. 分享链接给他人试用

- 他人点击链接可运行你的 AI 应用

- 修改不会影响你的原始版本（自动生成副本）

- 可用于产品演示、用户测试或团队协作开发

3. 查看已发布内容
在 Claude 平台的“Published”标签页可以看到你曾经发布的所有 Artifact 应用。

## 🚀 第四步：从原型走向产品
Artifacts 是快速试验和展示思路的理想平台，但当你准备上线一个正式产品时，虽然 Artifact 本身不能部署成产品，但你可以：
🧾 导出代码
Claude 会在 Artifact 内自动生成可复用的结构代码（HTML/JS/CSS）。
💻 导入本地开发环境
复制代码到你熟悉的开发环境（如 VSCode、Replit）进行增强开发：

- 添加外部 API 调用

- 扩展前端交互样式

- 集成数据库或后台服务

🧑‍💻 Claude Code 助力
使用 Claude Code 模型协助你进行代码结构优化、功能开发、Bug 修复等工程工作。
![](https://assets-v2.circle.so/mgvk31nnql6d6skrvzwvivxzncko)原型有了、思路清晰了、测试通过了，剩下的就是工程化的事了。

## 怎么高效地构建 Claude 应用？
一些实用技巧可以让你更快迭代：

- **让 Claude 反过来采访你**：告诉它你有个点子，它会问你一些关键问题，把想法一步步引导出来；

- **多用“请修改”这类自然语言指令**：比如“帮我改成蓝色主题”、“限制回复不超过 100 字”、“加一个复制按钮”；

- **调 bug 也能用聊天方式**：比如“这个计算器不能算小数”、“这个对话跳转有问题”，Claude 会理解并修正；

- **大胆分支测试**：随时点“编辑”创建分支版本，尝试不同逻辑，不用担心破坏原始版本。

## 小结：Claude Artifacts 是谁的福音？
Claude Artifacts 是一种面向非程序员和产品原型设计者的强大工具。它让你能以最少的开发成本，验证 AI 产品想法，并快速将其呈现为交互式体验。
想从 0 到 1 搭建 AI 应用？这就是最轻量、最快速的方式。

- **不会写代码但有创意的人**：Claude 可以帮你从 0 到 1 快速落地；

- **产品经理、运营人、内容创作者**：不再受限于“有个想法却没人帮忙做”；

- **开发者**：可以快速试验新思路，不再从空白页面起步；

- **创业者**：轻资产验证 MVP，快到飞起。

See more