[![English](https://img.shields.io/badge/English-Switch-blue)](README.md) [![简体中文](https://img.shields.io/badge/简体中文-切换-blue)](README_zh.md) [![日本語](https://img.shields.io/badge/日本語-切替-blue)](README_ja.md) [![한국어](https://img.shields.io/badge/한국어-전환-blue)](README_ko.md)

<div align="center">
  <img src="assets/logo.png" alt="Seedance Prompt Logo" width="200">

  # 🎬 Prompts para Seedance 2.0

  **Coleccion curada por la comunidad de prompts para generacion de video con [Seedance 2.0](https://seed.bytedance.com/en/seedance2_0) de ByteDance**

  [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
  [![GitHub stars](https://img.shields.io/github/stars/Ericgood/seedance-prompt?style=social)](https://github.com/Ericgood/seedance-prompt)
  [![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
  [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/Ericgood/seedance-prompt/pulls)

  **[Explorar Galeria](https://seedanceprompt.io)** | **[Enviar un Prompt](https://github.com/Ericgood/seedance-prompt/issues/new)**

</div>

---

## 🎬 Que es Seedance 2.0?

**Seedance 2.0** es un modelo de generacion de video multimodal desarrollado por el **equipo Seed de ByteDance**, lanzado el **10 de febrero de 2026**. Es el primer modelo de la industria que soporta **entrada simultanea de cuatro modalidades** — imagen, video, audio y texto — con generacion nativa conjunta de audio y video.

### Caracteristicas Principales

- 🏆 **Elo 1,269 en AI Video Arena** — Supero a Google Veo 3, OpenAI Sora 2 y Runway Gen-4.5 desde su lanzamiento
- 🎯 **Sistema de Referencia @** — Vincula hasta 9 imagenes, 3 videos y 3 pistas de audio para un control creativo preciso
- 🔊 **Sincronizacion de Audio Nativa** — Salida estereo con lip-sync en 8+ idiomas, dialogos, sonido ambiental y Foley en una sola generacion
- 🎬 **Narracion Multi-Toma** — Construye secuencias cinematicas completas con continuidad visual, no solo clips aislados
- 📷 **Camara Nivel Director** — Dolly zoom, rack focus, tomas de seguimiento, cambios de POV, camara en mano estable
- ⏱️ **Hasta 15 Segundos** — La mayor duracion de generacion unica entre los principales competidores
- 📐 **720p Nativo** — Con upscale disponible a 1080p y 2K

### Arquitectura y Especificaciones

| Especificacion | Detalle |
|:---|:---|
| **Arquitectura** | Dual-Branch Diffusion Transformer (frames de video + formas de onda de audio conjuntos) |
| **Desarrollador** | ByteDance (Equipo Seed) — lanzado 10 Feb 2026 |
| **Resolucion** | 720p nativo, upscale 1080p / 2K disponible |
| **Duracion** | 4, 5, 6, 8, 10, 12 o 15 segundos por generacion |
| **Modalidades de Entrada** | Texto + Imagenes (x9) + Videos (x3) + Audio (x3) mediante etiquetas @ |
| **Audio** | Salida estereo, lip-sync en 8+ idiomas, Foley y ambiental — en una pasada |
| **Modos de Generacion** | Text-to-Video (T2V), Image-to-Video (I2V), Video-to-Video (V2V) |
| **Disponible en** | CapCut, Dreamina, Spark, Doubao, API |

### Comparativa con la Competencia

| Modelo | Arena Elo | Duracion Max | Entradas Multi-Ref | Sincro Audio |
|:---|:---:|:---:|:---:|:---:|
| **Seedance 2.0** | **1,269** | **15s** | **15 (9+3+3)** | **Estereo** |
| Sora 2 (OpenAI) | ~1,220 | 12s | 2 | Mono |
| Kling 3.0 (Kuaishou) | ~1,248 | 10s | 2 | Mono |
| Veo 3.1 (Google) | ~1,200 | 8s | 1 | Si |
| Runway Gen-4.5 | ~1,180 | 10s | 1 | No |

*Datos de [Artificial Analysis Video Arena](https://artificialanalysis.ai/) y resenas independientes, 2026.*

### Que Dicen los Analistas

> *"El mejor modelo hasta la fecha"* en movimiento dinamico y fisica — **CuriousRefuge**

> *"Una de sus ventajas mas claras"* es el sistema de referencia @ — **Evolink AI**

> *"Una fortaleza real en pruebas practicas"* — la sincronizacion de audio — **WaveSpeed AI**

**Fortalezas:** El mejor sistema de referencias de la industria, excelente sincronizacion de audio, narrativas multi-toma sobresalientes, control cinematico de camara, simulacion de fisica superior.

**Limitaciones:** Resolucion nativa 720p (upscale 2K disponible), curva de aprendizaje pronunciada (sensible a la forma de operar), moderacion estricta de contenido para rostros realistas, velocidad de generacion mas lenta que algunas alternativas.

> *Fuentes de resenas: [CuriousRefuge](https://curiousrefuge.com/blog/seedance-2-review) · [Evolink AI](https://evolink.ai/blog/seedance-2-review-best-ai-video-generator-2026) · [WaveSpeed AI](https://wavespeed.ai/blog/posts/seedance-2-0-review-issues-and-alternatives/)*

---

## 📊 Estadisticas

| Total de Prompts | Destacados | Videos | Ultima Actualizacion |
|:---:|:---:|:---:|:---:|
| **111** | **11** | **10** | Abril 2026 |

---

## 🏆 Demos Destacadas

Prompts seleccionados que muestran las mejores capacidades de Seedance 2.0.

---

### 1. 🌙 Astronauta Esquiando en la Luna

![Featured](https://img.shields.io/badge/⭐_Featured-New-0055FF)

> 8K fotorrealista — fisica de gravedad 1/6, neblina de polvo, Tierra en cuarto creciente sobre el horizonte lunar.

#### 📝 Prompt

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
    <img src="assets/thumbnails/astronaut-moon-ski.jpg" width="700" alt="Astronauta Esquiando en la Luna">
  </a>
  <br>
  <a href="videos/astronaut-moon-ski.mp4">📥 Descargar Video</a> ・ <a href="https://x.com/i/status/2041855477617713535">🐦 Fuente</a>
</div>

---

### 2. 🧛 Transformacion de la Princesa Vampiro

![Featured](https://img.shields.io/badge/⭐_Featured-New-FF4D00)

> Clase magistral de referencias completas — 5 tomas distintas desde la vida cotidiana acogedora hasta vampiro gotico con luna de sangre, mostrando narrativa multi-toma y transiciones VFX.

#### 📝 Prompt

```
镜头一：日常居家 时间段：0:00 至 0:02 中景手持跟拍，女孩穿蜡笔小新睡衣，拿纸望远镜
对准镜头做转场。镜头二：时空隧道转场 0:02-0:04 深红漩涡虫洞效果，极速推进。
镜头三：吸血姬降临 0:04-0:06 白发精灵耳白色华服，慢动作红色花瓣飘落。
镜头四：魅惑定格 0:06-0:09 Glitch故障风、径向模糊、高饱和红色背景。
镜头五：血月飞翔 0:09-0:12 恶魔双翼悬浮夜空，巨大血月背景。
```

<div align="center">
  <a href="videos/vampire-transformation.mp4">
    <img src="assets/thumbnails/vampire-transformation.jpg" width="700" alt="Transformacion de la Princesa Vampiro">
  </a>
  <br>
  <a href="videos/vampire-transformation.mp4">📥 Descargar Video</a> ・ <a href="https://x.com/i/status/2042124667910008998">🐦 Fuente</a>
</div>

---

### 3. ☀️ Ambiente Matutino de Ciudad

![Featured](https://img.shields.io/badge/⭐_Featured-New-FF4D00)

> Multiples cortes de vida cotidiana — cartero, panadero, barista, acordeonista, vendedor de flores, pintor callejero. Calidas vibras de manana europea.

#### 📝 Prompt

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
    <img src="assets/thumbnails/morning-city-ambience.jpg" width="700" alt="Ambiente Matutino de Ciudad">
  </a>
  <br>
  <a href="videos/morning-city-ambience.mp4">📥 Descargar Video</a> ・ <a href="https://x.com/i/status/2038619621419569552">🐦 Fuente</a>
</div>

---

### 4. 🦛 Hipopotamo Kit Kat — Toma de Seguimiento Continua

![Featured](https://img.shields.io/badge/⭐_Featured-New-8C4EFF)

> Toma unica siguiendo una pelota — desde una calle al atardecer a traves de una ventana hasta una habitacion opulenta, revelando un hipopotamo en bata comiendo chocolate. Obra maestra publicitaria surrealista e inexpresiva.

#### 📝 Prompt

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
    <img src="assets/thumbnails/kitkat-hippo-ad.jpg" width="700" alt="Anuncio Kit Kat Hipopotamo">
  </a>
  <br>
  <a href="videos/kitkat-hippo-ad.mp4">📥 Descargar Video</a> ・ <a href="https://x.com/i/status/2041236549317378556">🐦 Fuente</a>
</div>

---

### 5. 🃏 Vuelo de Carta de Poker en Casino — 15s POV

![Featured](https://img.shields.io/badge/⭐_Featured-New-FF4D00)

> Cinematica de 15 segundos desde la perspectiva de la carta: desde una atractiva crupier a traves de escaleras de caracol, salones de inmersion, hasta la entrega oculta de la mano. Demostracion de seguimiento de camara complejo y narrativa multi-toma.

#### 📝 Prompt

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
    <img src="assets/thumbnails/casino-card-flight.jpg" width="700" alt="Vuelo de Carta de Poker en Casino">
  </a>
  <br>
  <a href="videos/casino-card-flight.mp4">📥 Descargar Video</a> ・ <a href="https://x.com/i/status/2040738604188623155">🐦 Fuente</a>
</div>

---

## 🤝 Como Contribuir

Damos la bienvenida a contribuciones de prompts de todos.

### Enviar mediante Pull Request

1. Haz **Fork** de este repositorio
2. **Agrega tu video** a `videos/` y la miniatura a `assets/thumbnails/`
3. **Actualiza** `prompts.json` con tu entrada de prompt
4. **Envia un PR** — lo revisaremos y fusionaremos.

### Enviar mediante Issue

No quieres lidiar con PRs? Simplemente [abre un issue](https://github.com/Ericgood/seedance-prompt/issues/new) con:

- Tu texto del prompt
- Archivo de video o enlace
- Descripcion de lo que genera
- Tu nombre/handle para el credito

### Formato de Datos del Prompt

Cada entrada en `prompts.json`:

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

### Directrices

- ✅ Prompts originales que hayas creado o tengas permiso para compartir
- ✅ Incluir el modelo utilizado (Seedance 2.0)
- ✅ Agregar una descripcion del resultado esperado
- ✅ Se recomiendan encarecidamente previsualizaciones de video/miniatura
- ❌ Sin contenido NSFW
- ❌ Sin reproducciones de personajes con derechos de autor

---

## 📜 Licencia

Este proyecto esta bajo la licencia [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Eres libre de compartir y adaptar los prompts, siempre que otorgues el credito apropiado.

## 🌐 Enlaces

- 🎬 [Seedance 2.0 Oficial](https://seed.bytedance.com/en/seedance2_0) — Equipo Seed de ByteDance
- 🌐 [seedanceprompt.io](https://seedanceprompt.io) — Explora prompts en una galeria visual
- 📊 [Artificial Analysis Video Arena](https://artificialanalysis.ai/) — Rankings de modelos
- 📝 [Resena de CuriousRefuge](https://curiousrefuge.com/blog/seedance-2-review) — "El mejor modelo hasta la fecha"
- 📝 [Resena de Evolink AI](https://evolink.ai/blog/seedance-2-review-best-ai-video-generator-2026) — Analisis exhaustivo de caracteristicas
- 📝 [Resena de WaveSpeed AI](https://wavespeed.ai/blog/posts/seedance-2-0-review-issues-and-alternatives/) — Problemas y alternativas
- 💬 [Discusiones](https://github.com/Ericgood/seedance-prompt/discussions)
- 🐛 [Reportar Problemas](https://github.com/Ericgood/seedance-prompt/issues)

## 🙏 Agradecimientos

- Datos de prompts obtenidos de [awesome-seedance-2-prompts](https://github.com/YouMind-OpenLab/awesome-seedance-2-prompts) (CC BY 4.0)
- Todos los autores originales de prompts estan acreditados en cada entrada
- Al equipo Seed de ByteDance por crear Seedance 2.0

---

<div align="center">

**Si te resulta util, regalanos una ⭐!**

Hecho con ❤️ por la Comunidad de Seedance Prompt

</div>
