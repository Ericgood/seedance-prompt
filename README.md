# 🎬 Seedance 2.0 Prompts

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

A community-curated collection of high-quality video generation prompts for ByteDance's **Seedance 2.0**.

> Browse the full gallery at **[seedanceprompt.io](https://seedanceprompt.io)**

---

## What's Inside

| Content | Count |
|:---|:---|
| Total Prompts | **106** |
| Featured | **6** |
| With Video | **5** |
| Categories | **9** (Action, Animation, Cinematic, Nature, Music, Horror, Fashion, Creative, Racing) |
| Languages | **EN + ZH** (bilingual titles & descriptions) |

## Structure

```
seedance-prompt/
├── prompts.json              # Core data file (website fetches this)
├── videos/                   # Video files (MP4)
│   ├── 1402.mp4
│   ├── 594.mp4
│   └── ...
├── assets/
│   ├── logo.png
│   └── thumbnails/           # Video thumbnails (JPG)
│       ├── 1402.jpg
│       ├── 594.jpg
│       └── ...
├── README.md
└── LICENSE                   # CC BY 4.0
```

## Data Format

Each prompt in `prompts.json`:

```json
{
  "id": "1402",
  "title": "Seedance 2.0: 15-Second Cinematic Japanese Romance Short Film",
  "title_zh": "Seedance 2.0：15 秒电影感日式浪漫短片",
  "prompt": "15-second cinematic Japanese drama...",
  "description": "A highly detailed multi-scene prompt...",
  "description_zh": "一个高度详细的多场景提示词...",
  "category": "Cinematic",
  "tag": "Cinematic",
  "tag_zh": "电影级",
  "tagColor": "#FF4D00",
  "model": "Seedance 2.0",
  "author": "AIGC｜阳家豪",
  "source": "https://x.com/...",
  "video": "videos/1402.mp4",
  "thumbnail": "assets/thumbnails/1402.jpg",
  "featured": true,
  "date": "March 15, 2026"
}
```

## Credits

Prompts collected from the community for educational purposes. Original authors and sources are credited in each entry.

Data sourced from [awesome-seedance-2-prompts](https://github.com/YouMind-OpenLab/awesome-seedance-2-prompts) (CC BY 4.0).

## Contributing

1. Fork this repo
2. Add your prompt to `prompts.json`
3. Include video (MP4) and thumbnail (JPG)
4. Submit a Pull Request

## License

[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) — free to share and adapt, with attribution.
