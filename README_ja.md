[![English](https://img.shields.io/badge/English-Switch-blue)](README.md) [![简体中文](https://img.shields.io/badge/简体中文-切换-blue)](README_zh.md) [![한국어](https://img.shields.io/badge/한국어-전환-blue)](README_ko.md) [![Español](https://img.shields.io/badge/Español-Cambiar-blue)](README_es.md)

<div align="center">
  <img src="assets/logo.png" alt="Seedance Prompt Logo" width="200">

  # 🎬 Seedance 2.0 プロンプト集

  **[Seedance 2.0](https://seed.bytedance.com/en/seedance2_0)（ByteDance）向けの動画生成プロンプトをコミュニティで厳選**

  [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
  [![GitHub stars](https://img.shields.io/github/stars/Ericgood/seedance-prompt?style=social)](https://github.com/Ericgood/seedance-prompt)
  [![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
  [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/Ericgood/seedance-prompt/pulls)

  **[ギャラリーを見る](https://seedanceprompt.io)** | **[プロンプトを投稿](https://github.com/Ericgood/seedance-prompt/issues/new)**

</div>

---

## 🎬 Seedance 2.0 とは？

**Seedance 2.0** は **ByteDance の Seed チーム** が開発したマルチモーダル動画生成モデルで、**2026年2月10日** にリリースされました。画像・動画・音声・テキストの **4モダリティ同時入力** に業界で初めて対応し、音声と映像のネイティブ同時生成を実現しています。

### 主な特長

- 🏆 **AI Video Arena で Elo 1,269** — リリース時に Google Veo 3、OpenAI Sora 2、Runway Gen-4.5 を超越
- 🎯 **@ リファレンスシステム** — 画像最大9枚、動画3本、オーディオ3トラックを紐付けて精密な制作コントロール
- 🔊 **ネイティブ音声同期** — ステレオ出力、8言語以上のリップシンク、セリフ、環境音、フォーリーを一度に生成
- 🎬 **マルチショットストーリーテリング** — 単独クリップではなく、映画的な連続シーケンスを構築
- 📷 **ディレクターレベルのカメラワーク** — ドリーズーム、ラックフォーカス、トラッキングショット、POV切り替え、手持ち風撮影
- ⏱️ **最大15秒** — 主要競合の中で最長の単回生成時間
- 📐 **ネイティブ720p** — 1080p・2Kアップスケール対応

### アーキテクチャと仕様

| 仕様 | 詳細 |
|:---|:---|
| **アーキテクチャ** | デュアルブランチ拡散Transformer（映像フレーム＋音声波形の同時処理） |
| **開発者** | ByteDance（Seed チーム）— 2026年2月10日リリース |
| **解像度** | ネイティブ720p、1080p / 2K アップスケール対応 |
| **再生時間** | 1回の生成で4、5、6、8、10、12、または15秒 |
| **入力モダリティ** | テキスト + 画像 (x9) + 動画 (x3) + 音声 (x3)、@ タグで指定 |
| **音声** | ステレオ出力、8言語以上のリップシンク、フォーリー＆環境音 — 一度に生成 |
| **生成モード** | Text-to-Video (T2V)、Image-to-Video (I2V)、Video-to-Video (V2V) |
| **利用プラットフォーム** | CapCut、Dreamina（即梦）、Spark、Doubao、API |

### 競合比較

| モデル | Arena Elo | 最大時間 | マルチリファレンス入力 | 音声同期 |
|:---|:---:|:---:|:---:|:---:|
| **Seedance 2.0** | **1,269** | **15s** | **15 (9+3+3)** | **ステレオ** |
| Sora 2 (OpenAI) | ~1,220 | 12s | 2 | モノラル |
| Kling 3.0 (Kuaishou) | ~1,248 | 10s | 2 | モノラル |
| Veo 3.1 (Google) | ~1,200 | 8s | 1 | 対応 |
| Runway Gen-4.5 | ~1,180 | 10s | 1 | 非対応 |

*データ出典：[Artificial Analysis Video Arena](https://artificialanalysis.ai/) および各種独立レビュー、2026年。*

### レビュアーの評価

> *「これまでで最高のモデル」* — ダイナミックなモーションと物理演算について — **CuriousRefuge**

> *「最も明確な強みの一つ」* は @ リファレンスシステム — **Evolink AI**

> *「実用テストで真の実力を発揮」* — 音声同期について — **WaveSpeed AI**

**強み：** 業界最高のリファレンスシステム、優れた音声同期、卓越したマルチショットナラティブ、シネマティックなカメラ制御、高品質な物理シミュレーション。

**課題：** ネイティブ解像度が720p（2Kアップスケール可能）、学習コストが高い（操作方法への依存度が高い）、リアルな人物の顔に対する厳格なコンテンツ審査、一部の競合より生成速度が遅い。

> *レビュー出典：[CuriousRefuge](https://curiousrefuge.com/blog/seedance-2-review) · [Evolink AI](https://evolink.ai/blog/seedance-2-review-best-ai-video-generator-2026) · [WaveSpeed AI](https://wavespeed.ai/blog/posts/seedance-2-0-review-issues-and-alternatives/)*

---

## 📊 統計

| プロンプト総数 | 注目 | 動画 | 最終更新 |
|:---:|:---:|:---:|:---:|
| **111** | **11** | **10** | 2026年4月 |

---

## 🏆 注目デモ

Seedance 2.0 の最高の能力を示す厳選プロンプト。

---

### 1. 🌙 月面スキーをする宇宙飛行士

![Featured](https://img.shields.io/badge/⭐_Featured-New-0055FF)

> 8Kフォトリアル — 1/6重力の物理演算、ダストヘイズ、月の地平線に浮かぶ三日月型の地球。

#### 📝 プロンプト

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
    <img src="assets/thumbnails/astronaut-moon-ski.jpg" width="700" alt="月面スキーをする宇宙飛行士">
  </a>
  <br>
  <a href="videos/astronaut-moon-ski.mp4">📥 動画をダウンロード</a> ・ <a href="https://x.com/i/status/2041855477617713535">🐦 ソース</a>
</div>

---

### 2. 🧛 ヴァンパイアプリンセスの変身

![Featured](https://img.shields.io/badge/⭐_Featured-New-FF4D00)

> フルリファレンスの実演 — 5つの異なるショットで、ほのぼの日常からゴシックヴァンパイア＋ブラッドムーンへ。マルチショットナラティブとVFXトランジションのショーケース。

#### 📝 プロンプト

```
镜头一：日常居家 时间段：0:00 至 0:02 中景手持跟拍，女孩穿蜡笔小新睡衣，拿纸望远镜
对准镜头做转场。镜头二：时空隧道转场 0:02-0:04 深红漩涡虫洞效果，极速推进。
镜头三：吸血姬降临 0:04-0:06 白发精灵耳白色华服，慢动作红色花瓣飘落。
镜头四：魅惑定格 0:06-0:09 Glitch故障风、径向模糊、高饱和红色背景。
镜头五：血月飞翔 0:09-0:12 恶魔双翼悬浮夜空，巨大血月背景。
```

<div align="center">
  <a href="videos/vampire-transformation.mp4">
    <img src="assets/thumbnails/vampire-transformation.jpg" width="700" alt="ヴァンパイアプリンセスの変身">
  </a>
  <br>
  <a href="videos/vampire-transformation.mp4">📥 動画をダウンロード</a> ・ <a href="https://x.com/i/status/2042124667910008998">🐦 ソース</a>
</div>

---

### 3. ☀️ 朝の街の風景

![Featured](https://img.shields.io/badge/⭐_Featured-New-FF4D00)

> マルチカットの日常風景 — 郵便配達員、パン屋、バリスタ、アコーディオン奏者、花売り、ストリート画家。温かみのあるヨーロッパの朝の雰囲気。

#### 📝 プロンプト

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
    <img src="assets/thumbnails/morning-city-ambience.jpg" width="700" alt="朝の街の風景">
  </a>
  <br>
  <a href="videos/morning-city-ambience.mp4">📥 動画をダウンロード</a> ・ <a href="https://x.com/i/status/2038619621419569552">🐦 ソース</a>
</div>

---

### 4. 🦛 Kit Kat ヒッポ — 連続トラッキングショット

![Featured](https://img.shields.io/badge/⭐_Featured-New-8C4EFF)

> 一発撮りのボール追跡ショット — ゴールデンアワーの街路から窓を通って豪華な部屋へ。バスローブ姿のカバがチョコレートを食べている姿が明らかに。シュールでデッドパンな広告の傑作。

#### 📝 プロンプト

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
    <img src="assets/thumbnails/kitkat-hippo-ad.jpg" width="700" alt="Kit Kat ヒッポ広告">
  </a>
  <br>
  <a href="videos/kitkat-hippo-ad.mp4">📥 動画をダウンロード</a> ・ <a href="https://x.com/i/status/2041236549317378556">🐦 ソース</a>
</div>

---

### 5. 🃏 カジノポーカーカードの飛行 — 15秒POV

![Featured](https://img.shields.io/badge/⭐_Featured-New-FF4D00)

> 15秒のカード視点シネマティック：セクシーなディーラーから螺旋階段、ダイビングホールを経て、隠された手札の配達まで。複雑なカメラトラッキングとマルチショットナラティブのショーケース。

#### 📝 プロンプト

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
    <img src="assets/thumbnails/casino-card-flight.jpg" width="700" alt="カジノポーカーカードの飛行">
  </a>
  <br>
  <a href="videos/casino-card-flight.mp4">📥 動画をダウンロード</a> ・ <a href="https://x.com/i/status/2040738604188623155">🐦 ソース</a>
</div>

---

## 🤝 コントリビュート方法

プロンプトの投稿をお待ちしています！

### Pull Request で投稿

1. このリポジトリを **Fork** する
2. 動画を `videos/` に、サムネイルを `assets/thumbnails/` に **追加**
3. `prompts.json` にプロンプトエントリを **追記**
4. **PR を提出** — レビューしてマージします！

### Issue で投稿

PR を使いたくない場合は、[Issue を作成](https://github.com/Ericgood/seedance-prompt/issues/new) して以下を記載してください：

- プロンプトのテキスト
- 動画ファイルまたはリンク
- 生成される内容の説明
- クレジット用の名前・ハンドルネーム

### プロンプトデータ形式

`prompts.json` の各エントリ：

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
  "tag_zh": "电影級",
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

### ガイドライン

- ✅ 自分で作成した、または共有許可のあるオリジナルプロンプト
- ✅ 使用モデル（Seedance 2.0）を明記
- ✅ 期待される出力の説明を追加
- ✅ 動画・サムネイルのプレビューを強く推奨
- ❌ NSFW コンテンツ禁止
- ❌ 著作権キャラクターの複製禁止

---

## 📜 ライセンス

このプロジェクトは [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) ライセンスの下で公開されています。適切なクレジットを表示すれば、プロンプトの共有・改変は自由です。

## 🌐 リンク

- 🎬 [Seedance 2.0 公式](https://seed.bytedance.com/en/seedance2_0) — ByteDance Seed チーム
- 🌐 [seedanceprompt.io](https://seedanceprompt.io) — ビジュアルギャラリーでプロンプトを閲覧
- 📊 [Artificial Analysis Video Arena](https://artificialanalysis.ai/) — モデルランキング
- 📝 [CuriousRefuge レビュー](https://curiousrefuge.com/blog/seedance-2-review) — 「これまでで最高のモデル」
- 📝 [Evolink AI レビュー](https://evolink.ai/blog/seedance-2-review-best-ai-video-generator-2026) — 包括的な機能分析
- 📝 [WaveSpeed AI レビュー](https://wavespeed.ai/blog/posts/seedance-2-0-review-issues-and-alternatives/) — 課題と代替案
- 💬 [ディスカッション](https://github.com/Ericgood/seedance-prompt/discussions)
- 🐛 [問題を報告](https://github.com/Ericgood/seedance-prompt/issues)

## 🙏 謝辞

- プロンプトデータは [awesome-seedance-2-prompts](https://github.com/YouMind-OpenLab/awesome-seedance-2-prompts) (CC BY 4.0) を元にしています
- すべてのオリジナルプロンプト作者は各エントリでクレジットされています
- Seedance 2.0 を開発した ByteDance Seed チームに感謝

---

<div align="center">

**お役に立てたら ⭐ をお願いします！**

Seedance Prompt コミュニティが ❤️ を込めて制作

</div>
