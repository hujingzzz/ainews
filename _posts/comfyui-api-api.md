---
layout: post
title: ComfyUI 推出原生 API 节点 可以直接在工作流中调用主流的图像和视频模型API 直接进行统一编排生成任务
date: 2025-06-11
category: Frontier Trends
thumbnail: /style/image/comfyui-api-api_1.jpg
icon: chat
---
* content
{:toc}

ComfyUI 推出了 **“原生 API 节点（Native API Nodes）”** 功能，使用户可以**直接在工作流中调用多个付费模型 API**，例如 Google Veo2、OpenAI GPT-4o image、Stability AI、Luma、Recraft、Pika 2.2、PixVerse、Ideogram 等共 **11 个模型系列、65 个节点**。
这意味着，用户可以在同一个 ComfyUI 流程中并行调用图像、视频生成、文本转视频等不同模型，**无需退出界面，统一编排生成任务**。
00:00UnmuteMuteSettingsCaptionsDisabledQuality1080pSpeedNormalCaptionsGo back to previous menuQualityGo back to previous menu480pSD720pHD1080pHDSpeedGo back to previous menu0.5×0.75×Normal1.25×1.5×1.75×2×4×PIPExit fullscreenEnter fullscreenPlay此外，ComfyUI 还支持：

- **用户自带 API key**（复用已有平台账户）；

- **并行执行 API 请求**（加快多模型调用速度）；

- **首次支持 VIDEO 类型**（原生视频生成任务）；

- **全新 UI 视觉品牌升级**（90年代动漫 + Y2K 科技风）；

所有 API 节点功能均为**可选**，ComfyUI 本体仍然 **完全免费开源**。

## ComfyUI 原生 API 节点是什么？
ComfyUI 过去是一个以图形节点方式驱动的本地图像生成工具，广泛用于 Stable Diffusion 社区。但本次更新，它引入了全新的组件：
**原生 API 节点（Native API Nodes）**：让用户在 ComfyUI 中，**无需离开界面、无需写代码，即可直接调用多个主流的“外部付费大模型 API”**。
这意味着：**你可以在一个工作流中，灵活混合调用多种商业模型（图像 / 视频 / 多模态）**，统一调度与生成，大幅提升创作效率。

## 目前支持的模型与API一览
ComfyUI 新增对以下 **11 个模型系列** 的原生接入支持，总计 **65 个节点**，涵盖图像、视频、文本转视频、图像转视频等多模态任务。

### 📌 支持模型包括：
![](https://assets-v2.circle.so/fgk399zgqypd1otehvj7m3scovy5)![](https://assets-v2.circle.so/djh9a87lxsny63szj5i4t73g3n0k)👉 用户通过拖放这些节点即可调用模型，无需单独登录每个平台，支持组合调用。

## 工作流中的具体使用方式

### 🧰 使用流程：
**更新 ComfyUI 或 ComfyUI Desktop**
登录 / 注册账户，购买或绑定已有平台的 API 积分
打开：Workflow → Browse Templates → Image API / Video API
选择模板直接运行
![](https://assets-v2.circle.so/w3dmoa9s88gak2vnoqi070mqzvt0)![](https://assets-v2.circle.so/cfgfllq6zmy347pryiq08kkf4nvd)![](https://assets-v2.circle.so/k37s4gj8nita6onhu57j0p17q4kz)![](https://assets-v2.circle.so/kb8nww6lez7evajyu3mwkbbieoca)✅ 你也可以使用“**Bring Your Own API Key（自带 Key）**”模式，绑定自己在其他平台已有的 API 凭证，例如你在 Pika、Luma、OpenAI 上已有订阅或额度。

### 🔄 支持并行执行：
在调用多个外部 API（如图像+视频+字幕）时，ComfyUI 会自动并行执行不同节点，大幅提升整体生成速度。
多模型协作示例：

- 文字 → GPT-Image 生成人物素描

- 素描图 → Luma Photon 加上真实感照明

- 场景图 + Prompt → PixVerse 生成视频片段

- 视频 + 描述 → Pika 生成动画对白镜头

![](https://assets-v2.circle.so/3rx51q3es60o55mkr9xu5n9ajpwr)
## 首次引入 VIDEO 类型原生支持
这是 ComfyUI 首次原生支持“视频生成”类型节点（VIDEO 类型），意味着：

- 不再局限于图像任务；

- 支持视频-图像组合型流程；

- 支持跨模态协作（如图像转视频、视频生成再提取片段重构等）；

- 为下一步音频/3D节点扩展打下基础。

## 视觉品牌全新升级
除了技术功能更新，ComfyUI 也正式推出全新品牌视觉系统：

- **Logo：**由多个模块组成，呼应“节点图形化工作流”；

- **字体与配色：**加入 90 年代动漫风格 + Y2K 数字感；

- **理念表达：**保留“自由、可拓展、可黑客化”的社区精神，强调工具性与创作开放性并存。
![](https://assets-v2.circle.so/5zfpponn56jnchf08pte3hpn295m)
官方原话：“我们想传达的是：ComfyUI 依然是自由、开放的。但它也已经成为真正能在生产流程中使用的强大工具。”

## 几点总结价值亮点
1. **统一式多模型接入平台**
一个工作流中整合多个主流 API 调用，不再需要切换平台、手动上传下载素材。
2. **免费本体 + 可选商用API**
ComfyUI 主体仍开源、免费，API 节点为按需使用。既保留创作者自由度，也提供商业级模型能力。
3. **真正面向创作者的“多模态生成管线”**
图片、视频、文字、结构数据、样式统一融合，未来将可能加入音频/3D节点。

### 谁适合用这些功能？

- 图文内容创作者（如微博、公众号、短视频配图）

- AI视频编辑者（使用 Pika、Veo2、PixVerse 的用户）

- Stable Diffusion 高级用户（想混合使用其他模型）

- 设计师/广告创意人（图像风格混搭生成）

- 教育内容开发者（视频转图文、视频配AI动画）

- 产品经理/开发者（构建 AI工作流原型）

官方介绍：https://blog.comfy.org/p/comfyui-native-api-nodes
See more