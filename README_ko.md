[![English](https://img.shields.io/badge/English-Switch-blue)](README.md) [![简体中文](https://img.shields.io/badge/简体中文-切换-blue)](README_zh.md) [![日本語](https://img.shields.io/badge/日本語-切替-blue)](README_ja.md) [![Español](https://img.shields.io/badge/Español-Cambiar-blue)](README_es.md)

<div align="center">
  <img src="assets/logo.png" alt="Seedance Prompt Logo" width="200">

  # 🎬 Seedance 2.0 프롬프트 모음

  **[Seedance 2.0](https://seed.bytedance.com/en/seedance2_0)(ByteDance) 영상 생성을 위한 커뮤니티 큐레이션 프롬프트 컬렉션**

  [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
  [![GitHub stars](https://img.shields.io/github/stars/Ericgood/seedance-prompt?style=social)](https://github.com/Ericgood/seedance-prompt)
  [![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
  [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/Ericgood/seedance-prompt/pulls)

  **[갤러리 둘러보기](https://seedanceprompt.io)** | **[프롬프트 제출](https://github.com/Ericgood/seedance-prompt/issues/new)**

</div>

---

## 🎬 Seedance 2.0이란?

**Seedance 2.0**은 **ByteDance의 Seed 팀**이 개발한 멀티모달 영상 생성 모델로, **2026년 2월 10일**에 출시되었습니다. 이미지, 영상, 오디오, 텍스트의 **4가지 모달리티 동시 입력**을 업계 최초로 지원하며, 네이티브 오디오-비디오 동시 생성 기능을 갖추고 있습니다.

### 주요 특징

- 🏆 **AI Video Arena Elo 1,269** — 출시와 동시에 Google Veo 3, OpenAI Sora 2, Runway Gen-4.5를 추월
- 🎯 **@ 레퍼런스 시스템** — 이미지 최대 9장, 영상 3개, 오디오 트랙 3개를 바인딩하여 정밀한 창작 제어
- 🔊 **네이티브 오디오 동기화** — 스테레오 출력, 8개 이상 언어 립싱크, 대사, 환경음, 폴리를 한 번에 생성
- 🎬 **멀티샷 스토리텔링** — 단독 클립이 아닌 시각적 연속성을 갖춘 시네마틱 시퀀스 구축
- 📷 **디렉터급 카메라워크** — 돌리 줌, 랙 포커스, 트래킹 샷, POV 전환, 핸드헬드 촬영
- ⏱️ **최대 15초** — 주요 경쟁 모델 중 가장 긴 단일 생성 시간
- 📐 **네이티브 720p** — 1080p 및 2K 업스케일 지원

### 아키텍처 및 사양

| 사양 | 상세 |
|:---|:---|
| **아키텍처** | 듀얼 브랜치 디퓨전 트랜스포머 (영상 프레임 + 오디오 파형 동시 처리) |
| **개발사** | ByteDance (Seed 팀) — 2026년 2월 10일 출시 |
| **해상도** | 네이티브 720p, 1080p / 2K 업스케일 지원 |
| **길이** | 1회 생성당 4, 5, 6, 8, 10, 12 또는 15초 |
| **입력 모달리티** | 텍스트 + 이미지 (x9) + 영상 (x3) + 오디오 (x3), @ 태그로 지정 |
| **오디오** | 스테레오 출력, 8개 이상 언어 립싱크, 폴리 & 환경음 — 한 번에 생성 |
| **생성 모드** | Text-to-Video (T2V), Image-to-Video (I2V), Video-to-Video (V2V) |
| **이용 플랫폼** | CapCut, Dreamina (즉몽), Spark, Doubao, API |

### 경쟁 모델 비교

| 모델 | Arena Elo | 최대 길이 | 멀티 레퍼런스 입력 | 오디오 동기화 |
|:---|:---:|:---:|:---:|:---:|
| **Seedance 2.0** | **1,269** | **15s** | **15 (9+3+3)** | **스테레오** |
| Sora 2 (OpenAI) | ~1,220 | 12s | 2 | 모노 |
| Kling 3.0 (Kuaishou) | ~1,248 | 10s | 2 | 모노 |
| Veo 3.1 (Google) | ~1,200 | 8s | 1 | 지원 |
| Runway Gen-4.5 | ~1,180 | 10s | 1 | 미지원 |

*데이터 출처: [Artificial Analysis Video Arena](https://artificialanalysis.ai/) 및 독립 리뷰, 2026년.*

### 리뷰어 평가

> *"지금까지 가장 뛰어난 모델"* — 다이내믹한 모션과 물리 시뮬레이션 부문 — **CuriousRefuge**

> *"가장 확실한 장점 중 하나"*는 @ 레퍼런스 시스템 — **Evolink AI**

> *"실전 테스트에서 진정한 강점을 보여준"* — 오디오 동기화 — **WaveSpeed AI**

**강점:** 최고 수준의 레퍼런스 시스템, 뛰어난 오디오 동기화, 우수한 멀티샷 내러티브, 시네마틱 카메라 제어, 우수한 물리 시뮬레이션.

**한계:** 네이티브 720p 해상도 (2K 업스케일 가능), 높은 학습 곡선 (조작 방식에 민감), 사실적 얼굴에 대한 엄격한 콘텐츠 심사, 일부 경쟁 모델 대비 느린 생성 속도.

> *리뷰 출처: [CuriousRefuge](https://curiousrefuge.com/blog/seedance-2-review) · [Evolink AI](https://evolink.ai/blog/seedance-2-review-best-ai-video-generator-2026) · [WaveSpeed AI](https://wavespeed.ai/blog/posts/seedance-2-0-review-issues-and-alternatives/)*

---

## 📊 통계

| 총 프롬프트 수 | 추천 | 영상 | 최종 업데이트 |
|:---:|:---:|:---:|:---:|
| **111** | **11** | **10** | 2026년 4월 |

---

## 🏆 추천 데모

Seedance 2.0의 최고 성능을 보여주는 엄선된 프롬프트.

---

### 1. 🌙 달에서 스키 타는 우주비행사

![Featured](https://img.shields.io/badge/⭐_Featured-New-0055FF)

> 8K 포토리얼 — 1/6 중력 물리, 먼지 안개, 달 지평선 위의 초승달 지구.

#### 📝 프롬프트

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
    <img src="assets/thumbnails/astronaut-moon-ski.jpg" width="700" alt="달에서 스키 타는 우주비행사">
  </a>
  <br>
  <a href="videos/astronaut-moon-ski.mp4">📥 영상 다운로드</a> ・ <a href="https://x.com/i/status/2041855477617713535">🐦 출처</a>
</div>

---

### 2. 🧛 뱀파이어 공주의 변신

![Featured](https://img.shields.io/badge/⭐_Featured-New-FF4D00)

> 풀 레퍼런스 마스터클래스 — 5개의 서로 다른 샷으로, 편안한 일상에서 고딕 뱀파이어와 블러드 문까지. 멀티샷 내러티브와 VFX 전환 쇼케이스.

#### 📝 프롬프트

```
镜头一：日常居家 时间段：0:00 至 0:02 中景手持跟拍，女孩穿蜡笔小新睡衣，拿纸望远镜
对准镜头做转场。镜头二：时空隧道转场 0:02-0:04 深红漩涡虫洞效果，极速推进。
镜头三：吸血姬降临 0:04-0:06 白发精灵耳白色华服，慢动作红色花瓣飘落。
镜头四：魅惑定格 0:06-0:09 Glitch故障风、径向模糊、高饱和红色背景。
镜头五：血月飞翔 0:09-0:12 恶魔双翼悬浮夜空，巨大血月背景。
```

<div align="center">
  <a href="videos/vampire-transformation.mp4">
    <img src="assets/thumbnails/vampire-transformation.jpg" width="700" alt="뱀파이어 공주의 변신">
  </a>
  <br>
  <a href="videos/vampire-transformation.mp4">📥 영상 다운로드</a> ・ <a href="https://x.com/i/status/2042124667910008998">🐦 출처</a>
</div>

---

### 3. ☀️ 아침 도시 풍경

![Featured](https://img.shields.io/badge/⭐_Featured-New-FF4D00)

> 멀티컷 일상 — 우편배달부, 제빵사, 바리스타, 아코디언 연주자, 꽃 판매원, 거리 화가. 따뜻한 유럽 아침 분위기.

#### 📝 프롬프트

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
    <img src="assets/thumbnails/morning-city-ambience.jpg" width="700" alt="아침 도시 풍경">
  </a>
  <br>
  <a href="videos/morning-city-ambience.mp4">📥 영상 다운로드</a> ・ <a href="https://x.com/i/status/2038619621419569552">🐦 출처</a>
</div>

---

### 4. 🦛 Kit Kat 하마 — 연속 트래킹 샷

![Featured](https://img.shields.io/badge/⭐_Featured-New-8C4EFF)

> 단일 연속 볼 추적 샷 — 골든아워의 거리에서 창문을 통과해 호화로운 방으로, 목욕 가운을 입고 초콜릿을 먹는 하마가 드러남. 초현실적 무표정 광고의 걸작.

#### 📝 프롬프트

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
    <img src="assets/thumbnails/kitkat-hippo-ad.jpg" width="700" alt="Kit Kat 하마 광고">
  </a>
  <br>
  <a href="videos/kitkat-hippo-ad.mp4">📥 영상 다운로드</a> ・ <a href="https://x.com/i/status/2041236549317378556">🐦 출처</a>
</div>

---

### 5. 🃏 카지노 포커 카드 비행 — 15초 POV

![Featured](https://img.shields.io/badge/⭐_Featured-New-FF4D00)

> 15초 카드 시점 시네마틱: 섹시한 딜러에서 나선형 계단, 다이빙 홀을 거쳐 숨겨진 핸드 딜리버리까지. 복잡한 카메라 트래킹과 멀티샷 내러티브 쇼케이스.

#### 📝 프롬프트

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
    <img src="assets/thumbnails/casino-card-flight.jpg" width="700" alt="카지노 포커 카드 비행">
  </a>
  <br>
  <a href="videos/casino-card-flight.mp4">📥 영상 다운로드</a> ・ <a href="https://x.com/i/status/2040738604188623155">🐦 출처</a>
</div>

---

## 🤝 기여 방법

프롬프트 기여를 환영합니다!

### Pull Request로 제출

1. 이 저장소를 **Fork**
2. 영상을 `videos/`에, 썸네일을 `assets/thumbnails/`에 **추가**
3. `prompts.json`에 프롬프트 항목을 **작성**
4. **PR 제출** — 검토 후 머지하겠습니다!

### Issue로 제출

PR이 번거로우시다면 [Issue를 생성](https://github.com/Ericgood/seedance-prompt/issues/new)하고 다음을 포함해 주세요:

- 프롬프트 텍스트
- 영상 파일 또는 링크
- 생성 결과 설명
- 크레딧용 이름/핸들

### 프롬프트 데이터 형식

`prompts.json`의 각 항목:

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

### 가이드라인

- ✅ 직접 만들었거나 공유 권한이 있는 오리지널 프롬프트
- ✅ 사용 모델 명시 (Seedance 2.0)
- ✅ 예상 출력 결과 설명 추가
- ✅ 영상/썸네일 미리보기 적극 권장
- ❌ NSFW 콘텐츠 금지
- ❌ 저작권 캐릭터 복제 금지

---

## 📜 라이선스

이 프로젝트는 [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) 라이선스로 공개됩니다. 적절한 크레딧을 표시하면 프롬프트를 자유롭게 공유하고 수정할 수 있습니다.

## 🌐 링크

- 🎬 [Seedance 2.0 공식](https://seed.bytedance.com/en/seedance2_0) — ByteDance Seed 팀
- 🌐 [seedanceprompt.io](https://seedanceprompt.io) — 비주얼 갤러리로 프롬프트 탐색
- 📊 [Artificial Analysis Video Arena](https://artificialanalysis.ai/) — 모델 랭킹
- 📝 [CuriousRefuge 리뷰](https://curiousrefuge.com/blog/seedance-2-review) — "지금까지 가장 뛰어난 모델"
- 📝 [Evolink AI 리뷰](https://evolink.ai/blog/seedance-2-review-best-ai-video-generator-2026) — 종합 기능 분석
- 📝 [WaveSpeed AI 리뷰](https://wavespeed.ai/blog/posts/seedance-2-0-review-issues-and-alternatives/) — 문제점과 대안
- 💬 [토론](https://github.com/Ericgood/seedance-prompt/discussions)
- 🐛 [이슈 신고](https://github.com/Ericgood/seedance-prompt/issues)

## 🙏 감사의 말

- 프롬프트 데이터는 [awesome-seedance-2-prompts](https://github.com/YouMind-OpenLab/awesome-seedance-2-prompts) (CC BY 4.0)에서 제공
- 모든 원작 프롬프트 작성자는 각 항목에 크레딧 표시
- Seedance 2.0을 개발한 ByteDance Seed 팀에 감사

---

<div align="center">

**유용하셨다면 ⭐ 부탁드립니다!**

Seedance Prompt 커뮤니티가 ❤️을 담아 제작

</div>
