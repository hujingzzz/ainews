---
layout: post
title: Gemini 2.0 Flash 图像生成功能升级 提升视觉质量和文字渲染能力 减少了内容安全拦截
date: 2025-06-11
category: Frontier Trends
thumbnail: /style/image/gemini-2-0-flash-b8d3b9_1.jpg
icon: web
---
* content
{:toc}

Google 宣布：其**Gemini 2.0 Flash 图像生成功能现已在预览阶段开放**，开发者可通过 Google AI Studio 和 Vertex AI 使用模型 gemini-2.0-flash-preview-image-generation 来创建和编辑图像。
同时Gemini 2.0 Flash 图像生成功能进行了升级

## Gemini 2.0 Flash 图像生成的升级内容：

- **更高的视觉质量**（相较于之前的实验版本）

- **更精准的文字渲染**

- **更少的内容过滤拦截率**（更易通过）
![](https://assets-v2.circle.so/pn39r5q0rn4q58126n5oadas5cv4)

## **一些案例**
**🖼️ 1. 产品图换背景**
举个例子，你想展示一个水杯，你可以说：“把这个水杯放在办公室桌子上”，AI 会自动生成一张合适的图。
![](https://assets-v2.circle.so/x78gmtxtzryjaokp79eysg1id14c)**✍️ 2. 对话式图片修改**
你可以对一张图片说：“把右下角的草地改成海滩”，AI 只会修改那一部分，其他地方不变。
![](https://assets-v2.circle.so/vtfqrlky9t8gnjqh3ia5g2v0zra7)**👩‍🎨 3. 实时协作绘图**
可以和 Gemini 一起“共绘”，像设计师团队一样协作画图（Co-Drawing Sample App）。
00:00UnmuteMuteSettingsCaptionsDisabledQuality1080pSpeedNormalCaptionsGo back to previous menuQualityGo back to previous menu480pSD720pHD1080pHDSpeedGo back to previous menu0.5×0.75×Normal1.25×1.5×1.75×2×4×PIPExit fullscreenEnter fullscreenPlay🔤 4. 图文结合：生成带文字的图
比如可以生成带有新品名称、价格标签的产品图，方便用在电商、广告中。
![](https://assets-v2.circle.so/wydiz0d9a2n6yro64iplcni2j7f5)![](https://assets-v2.circle.so/rficxxi1mlxmw0otul75ihgdatnv)💡 5. 帮你头脑风暴
你说：“帮我想一些手绘风格的马卡龙教程图”，它就能把你脑子里的创意画出来。
00:00UnmuteMuteSettingsCaptionsDisabledQuality1080pSpeedNormalCaptionsGo back to previous menuQualityGo back to previous menu480pSD720pHD1080pHDSpeedGo back to previous menu0.5×0.75×Normal1.25×1.5×1.75×2×4×PIPExit fullscreenEnter fullscreenPlay
## 💡 开发者可实现的图像生成功能：
**重新构图**：将产品置于不同环境中。
**实时协同编辑图像**：例如使用 Co-Drawing App 与 Gemini 共同编辑。
**局部图像编辑**：仅修改图像某一部分，其它区域保持不变。
**动态生成产品 SKU 图像**：结合文本生成新产品形象。
**创意辅助**：与 Gemini 协作构思、设计产品图像。
**💻 示例代码（调用 Gemini 图像生成）：**
开发者可以用 Google 的 API 这么写（Python 代码）：
from google import genai
from google.genai import types
client = genai.Client(api_key="你的API密钥")
response = client.models.generate_content(
model="gemini-2.0-flash-preview-image-generation",
contents="展示如何制作马卡龙的图文教程",
config=types.GenerateContentConfig(
response_modalities=["TEXT", "IMAGE"]
),
)
你会拿到一张 AI 生成的图，配上文字，像一个简短的教学卡片。
See more