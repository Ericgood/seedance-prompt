# 更新日志（CHANGELOG）

本文件记录 seedance-prompt 的每次发布。每个版本都带时间戳，并对应一条同名的 GitHub Release。
格式参考 [Keep a Changelog](https://keepachangelog.com/zh-CN/1.1.0/)，版本号遵循[语义化版本](https://semver.org/lang/zh-CN/)。
变更的详细背景见 [docs/](docs/README.md)。

## [未发布]

### 新增

- 2026-10-29 10:16 -0700 收录 20 条 MiniMax H3 提示词（`model` 为「MiniMax H3」），`prompts.json` 共 145 条；补齐 23 张缩略图（20 条 H3，另外 3 条是原先缺失的 2966 / 2899 / 2825）。Owner 10-30 决定 H3 放进现有仓库，仓库名不改。
- 2026-10-29 10:16 -0700 五种语言 README 加「MiniMax H3 Prompts」分区，链到 https://seedanceprompt.io/prompts/model/minimax-h3 。

### 变更

- 2026-10-29 10:18 -0700 五种语言 README 大标题改为「Seedance & MiniMax H3 Video Prompts」（各语言照译），库里已有 2.5 和 H3，原标题「Seedance 2.0 Prompts」不准确。
- 2026-10-29 10:16 -0700 五种语言 README 开头的定位句改为 Seedance 和 MiniMax H3 视频提示词；「Latest Prompts」和统计块按网站库重新生成。GitHub 仓库简介改为包含 MiniMax H3，并加 topics：seedance、minimax-h3、hailuo、ai-video、text-to-video、prompts。
- 2026-10-29 08:47 -0700 五种语言 README 加入「声明」一节：本库为独立非官方提示词库，与 ByteDance、MiniMax 均无关系（网站同步加入 MiniMax 后的口径）。

## [v0.1.0] - 2026-10-29 06:03 -0700

基线版本：接入维护规范时的项目快照。GitHub Release：https://github.com/Ericgood/seedance-prompt/releases/tag/v0.1.0

### 新增

- 125 条提示词数据（`prompts.json`）：112 条 Seedance 2.0、13 条 Seedance 2.5，附缩略图和媒体服务器上的视频链接（补记，2026-04-09 至 2026-10-27 的历史提交）
- 英文、中文、日文、韩文、西班牙文 README 与 CONTRIBUTING 投稿指南（补记）
- 2026-10-29 06:03 -0700 项目接入维护规范：建立 `docs/`、`CHANGELOG.md` 和 `AGENTS.md` / `CLAUDE.md` 中的项目规则（见 [docs/2026-10-29-接入维护规范.md](docs/2026-10-29-接入维护规范.md)）
