[![English](https://img.shields.io/badge/English-Switch-blue)](README.md) [![日本語](https://img.shields.io/badge/日本語-切替-blue)](README_ja.md) [![한국어](https://img.shields.io/badge/한국어-전환-blue)](README_ko.md) [![Español](https://img.shields.io/badge/Español-Cambiar-blue)](README_es.md)

<div align="center">
  <img src="assets/logo.png" alt="Seedance Prompt Logo" width="200">

  # 🎬 Seedance 2.0 提示词合集

  **社区精选的 [Seedance 2.0](https://seed.bytedance.com/en/seedance2_0) 视频生成提示词库（ByteDance 出品）**

  [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
  [![GitHub stars](https://img.shields.io/github/stars/Ericgood/seedance-prompt?style=social)](https://github.com/Ericgood/seedance-prompt)
  [![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
  [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/Ericgood/seedance-prompt/pulls)

  **[浏览画廊](https://seedanceprompt.io)** | **[提交提示词](https://github.com/Ericgood/seedance-prompt/issues/new)**

</div>

---

## 🎬 什么是 Seedance 2.0？

**Seedance 2.0** 是由 **字节跳动 Seed 团队** 开发的多模态视频生成模型，于 **2026 年 2 月 10 日** 正式发布。它是业界首个支持 **四模态同时输入** 的模型——图片、视频、音频和文本——并原生支持音视频联合生成。

### 核心亮点

- 🏆 **AI Video Arena Elo 1,269** — 发布即超越 Google Veo 3、OpenAI Sora 2 和 Runway Gen-4.5
- 🎯 **@ 引用系统** — 最多绑定 9 张图片、3 个视频和 3 条音轨，实现精准创作控制
- 🔊 **原生音频同步** — 立体声输出，支持 8 种以上语言口型同步、对白、环境声和拟音，一次生成
- 🎬 **多镜头叙事** — 构建完整的电影级连续镜头序列，而非孤立片段
- 📷 **导演级运镜** — 推拉变焦、焦点转换、跟踪镜头、POV 切换、手持稳拍
- ⏱️ **最长 15 秒** — 主流竞品中单次生成时长最长
- 📐 **原生 720p** — 可升级至 1080p 和 2K

### 架构与参数

| 参数 | 详情 |
|:---|:---|
| **架构** | 双分支扩散 Transformer（联合视频帧 + 音频波形） |
| **开发者** | 字节跳动（Seed 团队）— 2026 年 2 月 10 日发布 |
| **分辨率** | 原生 720p，可升级至 1080p / 2K |
| **时长** | 每次生成 4、5、6、8、10、12 或 15 秒 |
| **输入模态** | 文本 + 图片 (x9) + 视频 (x3) + 音频 (x3)，通过 @ 标签引用 |
| **音频** | 立体声输出，支持 8 种以上语言口型同步、拟音和环境声 — 一次生成 |
| **生成模式** | 文生视频 (T2V)、图生视频 (I2V)、视频生视频 (V2V) |
| **使用平台** | CapCut、即梦 (Dreamina)、Spark、豆包、API |

### 竞品对比

| 模型 | Arena Elo | 最长时长 | 多引用输入 | 音频同步 |
|:---|:---:|:---:|:---:|:---:|
| **Seedance 2.0** | **1,269** | **15s** | **15 (9+3+3)** | **立体声** |
| Sora 2 (OpenAI) | ~1,220 | 12s | 2 | 单声道 |
| Kling 3.0 (快手) | ~1,248 | 10s | 2 | 单声道 |
| Veo 3.1 (Google) | ~1,200 | 8s | 1 | 支持 |
| Runway Gen-4.5 | ~1,180 | 10s | 1 | 不支持 |

*数据来源：[Artificial Analysis Video Arena](https://artificialanalysis.ai/) 及独立评测，2026 年。*

### 评测声音

> *"迄今最出色的模型"*，尤其在动态运动和物理模拟方面 — **CuriousRefuge**

> *"最显著的优势之一"* 是 @ 引用系统 — **Evolink AI**

> *"在实际测试中展现出真正实力"* — 音频同步能力 — **WaveSpeed AI**

**优势：** 业界最佳引用系统、出色的音频同步、卓越的多镜头叙事、电影级运镜控制、优秀的物理模拟。

**不足：** 原生分辨率 720p（可升级 2K）、学习曲线较陡（对操作方式敏感）、真实人脸内容审核严格、生成速度慢于部分竞品。

> *评测来源：[CuriousRefuge](https://curiousrefuge.com/blog/seedance-2-review) · [Evolink AI](https://evolink.ai/blog/seedance-2-review-best-ai-video-generator-2026) · [WaveSpeed AI](https://wavespeed.ai/blog/posts/seedance-2-0-review-issues-and-alternatives/)*

---

## 📊 数据统计

| 提示词总数 | 精选 | 视频 | 最后更新 |
|:---:|:---:|:---:|:---:|
| **111** | **11** | **10** | 2026 年 4 月 |

---

## 🏆 精选展示

精选提示词，展示 Seedance 2.0 的最强能力。

---

### 1. 🌙 宇航员月球滑雪

![Featured](https://img.shields.io/badge/⭐_Featured-New-0055FF)

> 8K 照片级真实感 — 1/6 重力物理效果、尘雾、月球地平线上的新月形地球。

#### 📝 提示词

```
Wide shot. A lone astronaut in a dusty orange pressure suit with dark blue-gray harness
straps and black boots skis across a vast lunar plain, leaving two long parallel tracks
in the gray regolith behind. The astronaut is mid-stride, poles planted, pushing forward
in 1/6th gravity, each push sending the body drifting slightly upward before settling back.
Fine dust hangs in a low haze along the ski tracks. Behind and above, a crescent Earth sits
just over the soft curve of the lunar horizon, blue-white atmospheric glow against total
black sky. Raw sunlight, crushed shadows, no fill. 8K photorealistic. No logos on the suit.
```

<div align="center">
  <a href="videos/astronaut-moon-ski.mp4">
    <img src="assets/thumbnails/astronaut-moon-ski.jpg" width="700" alt="宇航员月球滑雪">
  </a>
  <br>
  <a href="videos/astronaut-moon-ski.mp4">📥 下载视频</a> ・ <a href="https://x.com/i/status/2041855477617713535">🐦 来源</a>
</div>

---

### 2. 🧛 吸血鬼公主变身

![Featured](https://img.shields.io/badge/⭐_Featured-New-FF4D00)

> 全引用大师课 — 5 个不同镜头，从温馨日常到哥特吸血鬼与血月，展示多镜头叙事和特效转场。

#### 📝 提示词

```
镜头一：日常居家 时间段：0:00 至 0:02 中景手持跟拍，女孩穿蜡笔小新睡衣，拿纸望远镜
对准镜头做转场。镜头二：时空隧道转场 0:02-0:04 深红漩涡虫洞效果，极速推进。
镜头三：吸血姬降临 0:04-0:06 白发精灵耳白色华服，慢动作红色花瓣飘落。
镜头四：魅惑定格 0:06-0:09 Glitch故障风、径向模糊、高饱和红色背景。
镜头五：血月飞翔 0:09-0:12 恶魔双翼悬浮夜空，巨大血月背景。
```

<div align="center">
  <a href="videos/vampire-transformation.mp4">
    <img src="assets/thumbnails/vampire-transformation.jpg" width="700" alt="吸血鬼公主变身">
  </a>
  <br>
  <a href="videos/vampire-transformation.mp4">📥 下载视频</a> ・ <a href="https://x.com/i/status/2042124667910008998">🐦 来源</a>
</div>

---

### 3. ☀️ 清晨城市氛围

![Featured](https://img.shields.io/badge/⭐_Featured-New-FF4D00)

> 多镜头生活切片 — 邮递员、面包师、咖啡师、手风琴演奏者、花贩、街头画家。温暖的欧洲清晨氛围。

#### 📝 提示词

```
Morning city ambience, people walking, cars driving, bikes riding.
[cut] The mailman on the bike drops a newspaper into the mailbox.
[cut] The baker places the buns on the counter.
[cut] The man playing the accordion on the street.
[cut] The woman pushing the baby stroller.
[cut] The barista making coffee.
[cut] The man playing the flute to his dog.
[cut] The man selling tulips on the street.
[cut] The man painting on the street.
```

<div align="center">
  <a href="videos/morning-city-ambience.mp4">
    <img src="assets/thumbnails/morning-city-ambience.jpg" width="700" alt="清晨城市氛围">
  </a>
  <br>
  <a href="videos/morning-city-ambience.mp4">📥 下载视频</a> ・ <a href="https://x.com/i/status/2038619621419569552">🐦 来源</a>
</div>

---

### 4. 🦛 Kit Kat 河马 — 连续跟踪长镜头

![Featured](https://img.shields.io/badge/⭐_Featured-New-8C4EFF)

> 单镜头跟球拍摄 — 从黄金时刻的街道穿过窗户进入一间奢华房间，揭示一只穿浴袍吃巧克力的河马。荒诞冷面风格广告杰作。

#### 📝 提示词

```
Over the shoulder of a young man in a beanie and jacket on a wet urban street at golden
hour. He winds up and hurls a baseball toward the building across the street. The camera
stays attached to the ball as it spins forward crossing the street, rises toward the facade,
passes through a window with glass parting gently around it catching golden light. The ball
continues through the interior of an opulent wood-paneled room, glides over a herringbone
parquet floor scattered with red chocolate wrappers and foil. The ball slows, rolls past
the foot of a velvet sofa and settles on the floor. The camera drifts upward from ball
level revealing a massive hippo in a white bathrobe reclining on the sofa surrounded by
red chocolate bars. He glances down at the ball with lazy curiosity, looks away and keeps
chewing. Hold. Hyper-realistic cinematic single continuous shot, warm golden hour exterior
transitioning seamlessly to rich amber interior. Anamorphic look. Deadpan surreal payoff.
```

<div align="center">
  <a href="videos/kitkat-hippo-ad.mp4">
    <img src="assets/thumbnails/kitkat-hippo-ad.jpg" width="700" alt="Kit Kat 河马广告">
  </a>
  <br>
  <a href="videos/kitkat-hippo-ad.mp4">📥 下载视频</a> ・ <a href="https://x.com/i/status/2041236549317378556">🐦 来源</a>
</div>

---

### 5. 🃏 赌场扑克牌飞行 — 15 秒 POV

![Featured](https://img.shields.io/badge/⭐_Featured-New-FF4D00)

> 15 秒扑克牌视角电影：从性感荷官手中出发，穿越螺旋楼梯、大厅，最终抵达神秘手牌。展示复杂运镜跟踪和多镜头叙事。

#### 📝 提示词

```
15秒赌场扑克牌飞行视频，黑桃K从性感女荷官手中飞出，以紧跟牌的视角穿越整个豪华赌场。
镜头1：女荷官上半身特写，手持黑桃K，牌正面朝向镜头。
镜头2：牌弹出瞬间，紧跟牌背面视角快速掠过赌桌区。
镜头3：牌沿螺旋楼梯弧线轨迹上升。
镜头4：牌高速直线穿越走廊。
镜头5：牌从二楼俯冲进入大堂。
镜头6：牌减速从玩家后方下面接近。
镜头7：牌悄悄传递到手中，翻转展示黑桃K正面。
镜头8：切回女荷官自信微笑特写。
写实风格、电影级质感、高速摄影、运动模糊、戏剧性打光。
```

<div align="center">
  <a href="videos/casino-card-flight.mp4">
    <img src="assets/thumbnails/casino-card-flight.jpg" width="700" alt="赌场扑克牌飞行">
  </a>
  <br>
  <a href="videos/casino-card-flight.mp4">📥 下载视频</a> ・ <a href="https://x.com/i/status/2040738604188623155">🐦 来源</a>
</div>

---

## 🤝 如何贡献

欢迎所有人提交提示词！

### 通过 Pull Request 提交

1. **Fork** 本仓库
2. 将你的 **视频** 添加到 `videos/`，缩略图添加到 `assets/thumbnails/`
3. 在 `prompts.json` 中 **添加** 你的提示词条目
4. **提交 PR** — 我们会审核并合并！

### 通过 Issue 提交

不想处理 PR？直接 [创建 Issue](https://github.com/Ericgood/seedance-prompt/issues/new)，包含以下内容：

- 你的提示词文本
- 视频文件或链接
- 生成效果描述
- 你的名字或账号（用于署名）

### 提示词数据格式

`prompts.json` 中每条记录的格式：

```json
{
  "id": "your-prompt-id",
  "title": "Your Prompt Title",
  "title_zh": "你的提示词标题",
  "prompt": "Your full prompt text...",
  "description": "Brief description of the output",
  "description_zh": "输出的简要描述",
  "category": "Cinematic",
  "tag": "Cinematic",
  "tag_zh": "电影级",
  "tagColor": "#FF4D00",
  "model": "Seedance 2.0",
  "author": "Your Name",
  "source": "https://x.com/...",
  "video": "videos/your-video.mp4",
  "thumbnail": "assets/thumbnails/your-video.jpg",
  "featured": false,
  "date": "April 2026"
}
```

### 提交指南

- ✅ 你原创或有权分享的提示词
- ✅ 注明所用模型（Seedance 2.0）
- ✅ 添加预期输出的描述
- ✅ 强烈建议附带视频/缩略图预览
- ❌ 禁止 NSFW 内容
- ❌ 禁止复制受版权保护的角色

---

## 📜 许可证

本项目采用 [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) 许可证。你可以自由分享和改编这些提示词，但需要注明出处。

## 🌐 相关链接

- 🎬 [Seedance 2.0 官方](https://seed.bytedance.com/en/seedance2_0) — 字节跳动 Seed 团队
- 🌐 [seedanceprompt.io](https://seedanceprompt.io) — 以视觉画廊方式浏览提示词
- 📊 [Artificial Analysis Video Arena](https://artificialanalysis.ai/) — 模型排名
- 📝 [CuriousRefuge 评测](https://curiousrefuge.com/blog/seedance-2-review) — "迄今最出色的模型"
- 📝 [Evolink AI 评测](https://evolink.ai/blog/seedance-2-review-best-ai-video-generator-2026) — 全面功能分析
- 📝 [WaveSpeed AI 评测](https://wavespeed.ai/blog/posts/seedance-2-0-review-issues-and-alternatives/) — 问题与替代方案
- 💬 [讨论区](https://github.com/Ericgood/seedance-prompt/discussions)
- 🐛 [问题反馈](https://github.com/Ericgood/seedance-prompt/issues)

## 🙏 致谢

- 提示词数据来源于 [awesome-seedance-2-prompts](https://github.com/YouMind-OpenLab/awesome-seedance-2-prompts) (CC BY 4.0)
- 所有原创提示词作者均在各条目中署名
- 感谢字节跳动 Seed 团队开发 Seedance 2.0

---

<div align="center">

**如果觉得有用，请给我们一个 ⭐！**

由 Seedance Prompt 社区用 ❤️ 打造

</div>
