# seedance-prompt

Seedance 2.0 视频生成提示词社区合集：提示词数据、视频与缩略图

<!-- project-rules:start -->
## 项目维护规则（必须遵守）

> 由「新建项目」技能于 2026-10-29 06:03 -0700 写入。
> 核心目的：以后回溯或拉取最新项目时，能看清项目的**历史变化**和**当前最新状态**。
> GitHub 仓库：https://github.com/Ericgood/seedance-prompt

### 1. 每次变更都上传 GitHub

- 任何改动（代码、配置、文档）完成并验证后，立即提交（commit）并推送（push）到 GitHub。
- 不在本地堆积未推送的提交：一轮工作结束前，`git status` 应为空，`git log origin/<分支>..HEAD` 应为空。
- 提交信息格式：`<type>: <描述>`，type 取 feat / fix / refactor / docs / test / chore / perf / ci。
- 推送前确认不含密钥、令牌、`.env` 等敏感文件；禁止 `--force` 推送。

### 2. docs/：记录变更内容、需求与技术细节和背景（带时间戳）

- 每次有意义的变更（新功能、需求调整、技术方案/架构决定、重要 bug 修复）都在 `docs/` 新建一篇 md。
- 文件名：`docs/YYYY-MM-DD-<主题>.md`；文件开头写完整时间戳 `YYYY-MM-DD HH:MM ±时区`（用 `date "+%Y-%m-%d %H:%M %z"` 生成，例如 `2026-10-28 15:20 +0800`）。
- 内容至少包含：**背景**（为什么做）、**内容/细节**（产品需求或技术实现）、**影响范围**、**关联**（提交、版本、相关文档）。
- 不改写旧文档的历史结论：有新进展就在文末追加「更新记录（时间戳）」，或新建一篇并互相链接。
- `docs/README.md` 是索引：新增文档时在表格**最上方**追加一行（时间倒序）。

### 3. CHANGELOG.md：记录每次发布，并与 GitHub Release 一一对应

- 平时的变更先写进 `## [未发布]` 区（分「新增 / 变更 / 修复 / 移除」）。
- 发布新版本时：
  1. 把 `[未发布]` 的内容移到新标题 `## [vX.Y.Z] - YYYY-MM-DD HH:MM ±时区` 下，并写上该版本的 GitHub Release 链接和相关 docs；
  2. 提交并推送，然后打标签、建 Release，Release 说明直接取 CHANGELOG 该版本段落：

     ```bash
     V=vX.Y.Z
     git tag -a "$V" -m "$V" && git push origin "$V"
     NOTES=$(mktemp)
     awk -v v="## [$V]" 'index($0,v)==1{f=1;next} /^## \[/{f=0} f' CHANGELOG.md > "$NOTES"
     gh release create "$V" --title "$V" --notes-file "$NOTES"; rm -f "$NOTES"
     gh release view "$V"   # 核对
     ```

- 版本号遵循语义化版本（SemVer）：不兼容改动升主版本，新功能升次版本，修复升修订号。
- 每个 CHANGELOG 版本都必须有同名 GitHub Release，反之亦然。

### 4. 接手或拉取项目时

- 先 `git pull`，再读 `CHANGELOG.md` 最上面的版本和 `docs/README.md` 最新几篇，了解当前状态后再动手。
<!-- project-rules:end -->
