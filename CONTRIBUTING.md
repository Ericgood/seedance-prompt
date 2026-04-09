# Contributing to Seedance Prompt

Thank you for your interest in contributing to the Seedance Prompt collection! This guide will help you get started.

## Table of Contents

- [Ways to Contribute](#ways-to-contribute)
- [Submitting a Prompt via Pull Request](#submitting-a-prompt-via-pull-request)
- [Submitting a Prompt via Issue](#submitting-a-prompt-via-issue)
- [Prompt Data Format](#prompt-data-format)
- [Categories](#categories)
- [Content Guidelines](#content-guidelines)
- [Code of Conduct](#code-of-conduct)

---

## Ways to Contribute

There are several ways you can contribute to this project:

1. **Submit a new prompt** — Share a Seedance 2.0 prompt that produces great results
2. **Improve existing prompts** — Suggest edits or refinements to prompts already in the collection
3. **Add translations** — Help translate prompt titles and descriptions into other languages
4. **Report issues** — Found a broken link, incorrect data, or formatting problem? Let us know
5. **Spread the word** — Star the repo and share it with the AI video community

---

## Submitting a Prompt via Pull Request

This is the preferred method for contributing prompts.

### Step-by-Step

1. **Fork** the repository on GitHub
2. **Clone** your fork locally:
   ```bash
   git clone https://github.com/YOUR-USERNAME/seedance-prompt.git
   cd seedance-prompt
   ```
3. **Create a new branch** for your contribution:
   ```bash
   git checkout -b add-prompt/your-prompt-name
   ```
4. **Add your files:**
   - Place your video file in `videos/` (MP4 format, under 50MB recommended)
   - Place a thumbnail image in `assets/thumbnails/` (JPG format, 16:9 ratio, 700px wide recommended)
5. **Add your prompt entry** to `prompts.json` (see [Prompt Data Format](#prompt-data-format) below)
6. **Commit and push** your changes:
   ```bash
   git add .
   git commit -m "Add prompt: Your Prompt Title"
   git push origin add-prompt/your-prompt-name
   ```
7. **Open a Pull Request** against the `main` branch with a clear description of your prompt

### PR Review Process

- A maintainer will review your PR within a few days
- We may suggest edits to your prompt text, metadata, or media files
- Once approved, your contribution will be merged and appear on [seedanceprompt.io](https://seedanceprompt.io)

---

## Submitting a Prompt via Issue

If you prefer not to work with Git, you can submit via a GitHub Issue.

1. Go to [Issues > New Issue](https://github.com/Ericgood/seedance-prompt/issues/new)
2. Use the title format: `[New Prompt] Your Prompt Title`
3. Include the following in the issue body:
   - **Prompt text** (the full prompt you used)
   - **Video** (upload directly to the issue, or provide a link)
   - **Description** (what the prompt generates)
   - **Category** (see [Categories](#categories))
   - **Credit** (your name or handle for attribution)
   - **Source link** (optional — tweet, post, or page where you shared it)

A maintainer will format and add your prompt to the collection.

---

## Prompt Data Format

Each prompt is stored as a JSON object in `prompts.json`. Here is the full schema:

```json
{
  "id": "your-prompt-id",
  "title": "Your Prompt Title",
  "title_zh": "中文标题",
  "prompt": "Your full prompt text goes here...",
  "description": "Brief description of what the video shows",
  "description_zh": "视频内容的简要描述",
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

### Field Descriptions

| Field | Required | Description |
|:---|:---:|:---|
| `id` | Yes | Unique kebab-case identifier (e.g., `astronaut-moon-ski`) |
| `title` | Yes | English title for the prompt |
| `title_zh` | No | Chinese (Simplified) title |
| `prompt` | Yes | The full prompt text exactly as used with Seedance 2.0 |
| `description` | Yes | 1-2 sentence description of the generated output |
| `description_zh` | No | Chinese description |
| `category` | Yes | One of the available categories (see below) |
| `tag` | Yes | Display tag (usually matches category) |
| `tag_zh` | No | Chinese display tag |
| `tagColor` | Yes | Hex color code for the tag badge |
| `model` | Yes | Always `"Seedance 2.0"` |
| `author` | Yes | Your name or handle |
| `source` | No | URL to the original post (tweet, blog, etc.) |
| `video` | Yes | Path to the video file in `videos/` |
| `thumbnail` | Yes | Path to the thumbnail in `assets/thumbnails/` |
| `featured` | No | Set to `true` only by maintainers |
| `date` | Yes | Month and year of submission (e.g., `"April 2026"`) |

---

## Categories

Choose the category that best fits your prompt:

| Category | Tag Color | Description |
|:---|:---:|:---|
| **Action** | `#FF4D00` | Fight scenes, stunts, explosions, chase sequences |
| **Animation** | `#8C4EFF` | Cartoon, anime, stop-motion, and stylized animation |
| **Cinematic** | `#FF4D00` | Film-quality shots, multi-shot narratives, dramatic lighting |
| **Nature** | `#00AA55` | Landscapes, wildlife, weather, natural phenomena |
| **Music** | `#E91E63` | Music videos, performances, rhythm-synced visuals |
| **Horror** | `#880000` | Scary, eerie, suspenseful, or dark-themed content |
| **Fashion** | `#FF69B4` | Runway, styling, lookbooks, fashion photography |
| **Creative** | `#0055FF` | Abstract, experimental, surreal, or artistic concepts |
| **Racing** | `#FF8C00` | Vehicles, motorsport, speed, driving sequences |
| **Sci-Fi** | `#0055FF` | Futuristic, space, technology, speculative fiction |

If your prompt does not fit neatly into one of these categories, choose the closest match or suggest a new category in your PR description.

---

## Content Guidelines

### Accepted

- Original prompts you created or have explicit permission to share
- Prompts that specify the model used (Seedance 2.0)
- Entries that include a clear description of the expected output
- Video and thumbnail previews (highly encouraged)
- Prompts in any language (English and Chinese are the most common)

### Not Accepted

- **NSFW content** — No nudity, graphic violence, or sexually explicit material
- **Copyrighted character reproductions** — Do not submit prompts designed to replicate specific copyrighted characters (e.g., Disney, Marvel, etc.)
- **Hate speech or discriminatory content** — No content targeting individuals or groups
- **Misleading deepfakes** — No prompts intended to create deceptive impersonations of real people
- **Spam or low-effort submissions** — Prompts should produce meaningful, interesting results

### Media File Requirements

- **Video:** MP4 format, under 50MB. If your video is larger, consider compressing it or linking to an external host
- **Thumbnail:** JPG format, 16:9 aspect ratio, approximately 700px wide. Should be a representative frame from the video
- **Naming convention:** Use kebab-case matching your prompt ID (e.g., `astronaut-moon-ski.mp4`, `astronaut-moon-ski.jpg`)

---

## Code of Conduct

By participating in this project, you agree to:

- Be respectful and constructive in all interactions
- Welcome contributors of all experience levels
- Give proper credit to original prompt authors
- Follow the content guidelines above
- Help maintain a positive and inclusive community

---

## Questions?

- Open a [Discussion](https://github.com/Ericgood/seedance-prompt/discussions) for general questions
- File an [Issue](https://github.com/Ericgood/seedance-prompt/issues) for bugs or problems
- Check the [README](README.md) for project overview and links

Thank you for helping grow the Seedance Prompt community!
