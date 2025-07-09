---
layout: post
title: MiniMax 发布其最新视频生成模型 Hailuo 02 全球唯一兼顾画质、复杂控制与高性能的视频模型
date: 2025-06-30 12:00:00 +0800
category: Frontier Trends
thumbnail: /style/image/minimax-hailuo-02_1.jpg
icon: design
---
* content
{:toc}

MiniMax 发布其 Hailuo 02（代号“Kangaroo”）的最新AI视频生成模型，在Artificial Analysis评测榜中，全球排名第二，仅次于字节跳动的Seedance 1.0 Pro，超越Google Veo 3。

- **Hailuo 02 是当前唯一公开可用、兼顾画质、复杂控制与高性能的 AI 原生视频生成模型**；

- 对比 Runway、Pika Labs、SVD 等主要视频生成技术玩家，Hailuo 更偏重**真实物理建模**与**复杂动作生成**，适用于动画、CG、广告、电影预演等专业创作场景；
00:00UnmuteMuteSettingsCaptionsDisabledQuality1080pSpeedNormalCaptionsGo back to previous menuQualityGo back to previous menu480pSD720pHD1080pHDSpeedGo back to previous menu0.5×0.75×Normal1.25×1.5×1.75×2×4×PIPExit fullscreenEnter fullscreenPlay

## 生成效果能力与特性
![](https://assets-v2.circle.so/xw121umve9oy1kipjkn3brajngqi)**高分辨率输出**：

- 支持**原生1080p**（1920×1080）分辨率，帧率为24-30fps，提供专业级视觉效果，适合社交媒体、广告原型或短片创作。

- 另提供768p选项，支持6秒或10秒视频，灵活适应不同需求。
![](https://assets-v2.circle.so/6j9c6ctpj93qzkkpodr2cdkbrmoy)
**视频时长**：

- 最大生成**10秒**视频，适合短格式内容，如社交媒体短视频、促销片段或故事板动画，较前代Hailuo 01（6秒）有所提升。

**先进物理模拟**：

- 采用突破性的**Noise-aware Compute Redistribution (NCR)**架构，训练和推理效率提升2.5倍，参数量增加3倍，数据集规模扩大4倍。

- 擅长处理复杂物理场景，如体操动作、流体动力学、碰撞检测和材质交互，生成自然、逼真的运动效果。例如，可精准呈现爆炸、布料褶边或反射光影。

**指令遵循与创意控制**：

- 支持**多语言文本提示**（包括英语、汉语等），能准确解读复杂指令，生成符合用户意图的视频。

- 提供**摄像机指令**功能，用户可指定镜头移动（如平移、倾斜、推拉），生成类似专业Steadicam的电影化效果。

- 角色一致性强，通过高级面部识别和身体跟踪技术，确保角色外观、服装和特征在所有帧中保持一致。

**生成模式**：

- **文本到视频（T2V）**：基于文本描述生成视频，适合从零开始创作。

- **图像到视频（I2V）**：将静态图像动画化，保留艺术风格或细节，适用于将插画或照片转化为动态内容。

- **主体到视频（S2V）**：基于参考图像保持角色一致性，适合多镜头或连续场景。
![](https://assets-v2.circle.so/xzwzn830cpmcnsh3fq4s1iexwuw7)

### 成本策略：

- 由于模型效率提升显著，Hailuo 02 在维持高质量的同时：
成本不升反降；

- 相比行业同类产品（如Runway、Pika、SVD），具有极高性价比；

定价极具竞争力，生成5-10秒768p视频成本约**0.28-0.56美元**，1080p视频每秒约**0.08美元**，比许多国际竞争对手（如Seedance 1.0 Pro）更经济。
生成时间约**30-60秒**（视复杂性而定），部分平台（如GoEnhance）声称最快90秒内交付高清视频。
官方承诺：**不以高门槛限制创作者使用**，技术应普惠。
![](https://assets-v2.circle.so/anwc5kiiapb1fajvlagbiri4aywu)
## 技术创新
Hailuo 02 的发布不仅是简单版本升级，而是在多个维度同时突破的技术跃迁。

### 1️⃣ 架构级创新：**NCR (Noise-aware Compute Redistribution)**
原理：

- “噪声感知的计算重分配”，是一种高效能的训练与推理分布方式；

- 将计算资源动态调配到模型学习任务中更有意义的位置，规避资源浪费；

成果：

- **训练与推理效率提升 2.5 倍**；

- 同等硬件资源下可运行参数量更大的模型；

- 为后续推理优化留出充足空间，**未来仍可加速**。
![](https://assets-v2.circle.so/5frtvtcg32m4sfvmymyupdu7wym9)

### 2️⃣ 模型体量：**参数量扩展至前代的 3 倍**

- 更大的模型意味着：
更强的图像细节生成能力；

- 更复杂语义的理解与执行；

- 更稳定一致的表现逻辑；

得益于 NCR 提高的计算效率，这种扩张并未带来成本上升，反而控制得更合理。

### 3️⃣ 数据规模与质量提升：**训练数据 × 4 倍**

- 数据内容更广泛，包含：
复杂人物动作；

- 写实环境下的光影变化；

- 不同文化和语言背景下的视频内容；

数据多样性大幅提升，显著增强模型泛化能力；
结合 Hailuo 01 的使用反馈，构建高质量标注数据集，实现更精细的目标驱动训练。

### 4️⃣ 指令遵循能力：**State-of-the-Art Instruction Following**

- 可精确响应更复杂的自然语言提示；

- 多段式描述、含抽象意象、动作控制的提示执行表现优秀；

- 在测试中，复杂场景下的**动作协调性、连续性、物理合理性大幅提升**。

## 一些案例

00:00UnmuteMuteSettingsCaptionsDisabledQuality1080pSpeedNormalCaptionsGo back to previous menuQualityGo back to previous menu480pSD720pHD1080pHDSpeedGo back to previous menu0.5×0.75×Normal1.25×1.5×1.75×2×4×PIPExit fullscreenEnter fullscreenPlay00:00UnmuteMuteSettingsCaptionsDisabledQuality1080pSpeedNormalCaptionsGo back to previous menuQualityGo back to previous menu480pSD720pHD1080pHDSpeedGo back to previous menu0.5×0.75×Normal1.25×1.5×1.75×2×4×PIPExit fullscreenEnter fullscreenPlay
00:00UnmuteMuteSettingsCaptionsDisabledQuality720pSpeedNormalCaptionsGo back to previous menuQualityGo back to previous menu480pSD720pHDSpeedGo back to previous menu0.5×0.75×Normal1.25×1.5×1.75×2×4×PIPExit fullscreenEnter fullscreenPlay
00:00UnmuteMuteSettingsCaptionsDisabledQuality1080pSpeedNormalCaptionsGo back to previous menuQualityGo back to previous menu480pSD720pHD1080pHDSpeedGo back to previous menu0.5×0.75×Normal1.25×1.5×1.75×2×4×PIPExit fullscreenEnter fullscreenPlaySee more