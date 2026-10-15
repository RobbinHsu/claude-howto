<picture>
  <source media="(prefers-color-scheme: dark)" srcset="resources/logos/claude-howto-logo-dark.svg">
  <img alt="Claude How To" src="resources/logos/claude-howto-logo.svg">
</picture>

<p align="center">
  <a href="https://github.com/trending">
    <img src="https://img.shields.io/badge/GitHub-🔥%20%231%20Trending-purple?style=for-the-badge&logo=github"/>
  </a>
</p>

[![GitHub Stars](https://img.shields.io/github/stars/luongnv89/claude-howto?style=flat&color=gold)](https://github.com/luongnv89/claude-howto/stargazers)
[![GitHub Forks](https://img.shields.io/github/forks/luongnv89/claude-howto?style=flat)](https://github.com/luongnv89/claude-howto/network/members)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Version](https://img.shields.io/badge/version-2.1.296-brightgreen)](CHANGELOG.md)
[![Claude Code](https://img.shields.io/badge/Claude_Code-2.1+-purple)](https://code.claude.com)

🌐 **語言 / Language / Ngôn ngữ / 语言 / Мова：** [繁體中文](README.md) | [Tiếng Việt](vi/README.md) | [简体中文](zh/README.md) | [Українська](uk/README.md) | [日本語](ja/README.md) | [English（原始版本）](https://github.com/RobbinHsu/claude-howto/blob/main/README.md)

# 在一個週末掌握 Claude Code

從輸入 `claude` 開始，逐步學會協調 Agents、Hooks、Skills 與 MCP 伺服器——透過視覺化教學、可直接複製貼上的範本，以及循序漸進的學習路線來完成。

**[15 分鐘快速入門](#15-分鐘快速入門)** | **[找到適合自己的起點](#不知道從哪裡開始)** | **[瀏覽功能目錄](CATALOG.md)**

---

## 目錄

- [遇到的問題](#遇到的問題)
- [Claude How To 如何解決這些問題](#claude-how-to-如何解決這些問題)
- [運作方式](#運作方式)
- [不知道從哪裡開始？](#不知道從哪裡開始)
- [15 分鐘快速入門](#15-分鐘快速入門)
- [你能用它打造什麼？](#你能用它打造什麼)
- [常見問題](#常見問題)
- [參與貢獻](#參與貢獻)
- [授權條款](#授權條款)

---

## 遇到的問題

你安裝了 Claude Code，也嘗試過幾次提示詞。接下來呢？

- **官方文件說明個別功能，卻沒有展示如何組合運用。** 你知道有斜線指令，卻不知道如何將它們與 Hooks、記憶及 Subagents 串接，形成真正能節省數小時的工作流程。
- **缺乏明確的學習路線。** 應該先學 MCP，還是先學 Hooks？先學 Skills，還是 Subagents？最後每項都只是略讀，卻沒有真正掌握。
- **範例過於基礎。** 一個「Hello World」等級的斜線指令，無法幫你建構正式環境可用的程式碼審查流程——這種流程需要使用記憶、將工作委派給專業代理，並自動執行安全性掃描。

Claude Code 有 90% 的能力被你閒置，而你甚至不知道自己還有哪些事情尚未了解。

---

## Claude How To 如何解決這些問題

這不是另一份功能參考手冊，而是一份**結構化、視覺化、以範例為核心的指南**。它會教你使用 Claude Code 的各項功能，並提供可以立即複製到專案使用的實際情境範本。

| | 官方文件 | 本指南 |
|--|----------|--------|
| **形式** | 參考文件 | 搭配 Mermaid 圖表的視覺化教學 |
| **深度** | 功能描述 | 深入了解底層運作方式 |
| **範例** | 基本程式片段 | 可立即使用的正式環境範本 |
| **結構** | 依功能分類 | 從初學者到進階使用者的漸進式學習路線 |
| **入門引導** | 自行探索 | 附預估時間的引導式學習地圖 |
| **自我評估** | 無 | 互動式測驗，找出知識缺口並規劃個人學習路線 |

### 你可以取得：

- **10 個教學模組**，涵蓋 Claude Code 的各項功能——從斜線指令到自訂代理團隊
- **可複製貼上的設定**——包括斜線指令、CLAUDE.md 範本、Hook 腳本、MCP 設定、Subagent 定義與完整 Plugin 套件
- **Mermaid 圖表**，呈現各功能在內部如何運作，讓你不只了解「怎麼做」，也了解「為什麼」
- **引導式學習路線**，用 11–13 小時從初學者進階到熟練使用者
- **內建自我評估**——直接在 Claude Code 執行 `/self-assessment` 或 `/lesson-quiz hooks`，找出尚未掌握的部分

**[開始學習路線 →](LEARNING-ROADMAP.md)**

---

## 運作方式

### 1. 找到自己的程度

完成[自我評估測驗](LEARNING-ROADMAP.md#-find-your-level)，或在 Claude Code 執行 `/self-assessment`。系統會根據你已具備的知識產生個人化學習路線。

### 2. 跟著引導路線學習

依順序完成 10 個模組——每個模組都建立在前一個模組的基礎上。學習過程中可直接將範本複製到自己的專案。

### 3. 將功能組合成工作流程

真正的威力來自功能組合。學會串接斜線指令、記憶、Subagents 和 Hooks，建立可處理程式碼審查、部署及文件產生的自動化流程。

### 4. 測試自己的理解程度

完成每個模組後，執行 `/lesson-quiz [topic]`。測驗會指出你尚未掌握的內容，協助你迅速補足知識缺口。

**[15 分鐘快速入門](#15-分鐘快速入門)**

---

## 受到開發者信賴

- **GitHub Stars**——來自每天使用 Claude Code 的開發者
- **Forks**——來自將本指南調整為團隊工作流程的使用者
- **持續維護**——隨 Claude Code 各版本更新（最新：2026 年 10 月的 v2.1.296）
- **社群驅動**——由分享實際設定的開發者共同貢獻

[![Star History Chart](https://api.star-history.com/svg?repos=luongnv89/claude-howto&type=Date)](https://star-history.com/#luongnv89/claude-howto&Date)

---

## 不知道從哪裡開始？

先進行自我評估，或選擇符合你的程度：

| 程度 | 你已經能夠…… | 從這裡開始 | 時間 |
|------|--------------|------------|------|
| **初學者** | 啟動 Claude Code 並與其對話 | [斜線指令](01-slash-commands/) | 約 2.5 小時 |
| **中階** | 使用 CLAUDE.md 和自訂指令 | [Skills](03-skills/) | 約 3.5 小時 |
| **進階** | 設定 MCP 伺服器及 Hooks | [進階功能](09-advanced-features/) | 約 5 小時 |

**包含全部 10 個模組的完整學習路線：**

| 順序 | 模組 | 程度 | 時間 |
|------|------|------|------|
| 1 | [斜線指令](01-slash-commands/) | 初學者 | 30 分鐘 |
| 2 | [記憶](02-memory/) | 初學者+ | 45 分鐘 |
| 3 | [檢查點](08-checkpoints/) | 中階 | 45 分鐘 |
| 4 | [CLI 基礎](10-cli/) | 初學者+ | 30 分鐘 |
| 5 | [Skills](03-skills/) | 中階 | 1 小時 |
| 6 | [Hooks](06-hooks/) | 中階 | 1 小時 |
| 7 | [MCP](05-mcp/) | 中階+ | 1 小時 |
| 8 | [Subagents](04-subagents/) | 中階+ | 1.5 小時 |
| 9 | [進階功能](09-advanced-features/) | 進階 | 2–3 小時 |
| 10 | [Plugins](07-plugins/) | 進階 | 2 小時 |

**[完整學習路線 →](LEARNING-ROADMAP.md)**

---

## 15 分鐘快速入門

> **安裝注意事項**：從 v2.1.113 開始，Claude Code 以各作業系統的原生二進位檔形式提供（macOS／Linux／Windows）。`npm install -g @anthropic-ai/claude-code` 仍然可用——首次使用時，會透過選用相依套件下載原生執行檔。自 v2.1.116 起，下載來源改為 `https://downloads.claude.ai/claude-code-releases`——企業 Proxy 必須將此主機加入允許清單。

```bash
# 1. 複製本指南的儲存庫
git clone https://github.com/luongnv89/claude-howto.git
cd claude-howto

# 2. 複製你的第一個斜線指令
mkdir -p /path/to/your-project/.claude/commands
cp 01-slash-commands/optimize.md /path/to/your-project/.claude/commands/

# 3. 試著使用它——在 Claude Code 輸入：
# /optimize

# 4. 想進一步設定？加入專案記憶：
cp 02-memory/project-CLAUDE.md /path/to/your-project/CLAUDE.md

# 5. 安裝一個 Skill：
cp -r 03-skills/code-review-specialist ~/.claude/skills/
```

想完成完整設定嗎？這是**一小時的基本設定流程**：

```bash
# 斜線指令（15 分鐘）
cp 01-slash-commands/*.md .claude/commands/

# 專案記憶（15 分鐘）
cp 02-memory/project-CLAUDE.md ./CLAUDE.md

# 安裝 Skill（15 分鐘）
cp -r 03-skills/code-review-specialist ~/.claude/skills/

# 週末目標：加入 Hooks、Subagents、MCP 與 Plugins
# 按照學習路線逐步完成設定
```

**[查看完整安裝參考](#15-分鐘快速入門)**

---

## 你能用它打造什麼？

| 使用情境 | 組合使用的功能 |
|----------|----------------|
| **自動化程式碼審查** | 斜線指令 + Subagents + 記憶 + MCP |
| **團隊新人導入** | 記憶 + 斜線指令 + Plugins |
| **CI/CD 自動化** | CLI 參考 + Hooks + 背景任務 |
| **文件產生** | Skills + Subagents + Plugins |
| **安全性稽核** | Subagents + Skills + Hooks（唯讀模式） |
| **DevOps 流程** | Plugins + MCP + Hooks + 背景任務 |
| **複雜重構** | 檢查點 + 規劃模式 + Hooks |

---

## 常見問題

**這是免費的嗎？**
是的。採用 MIT 授權，永久免費。無論個人專案、工作或團隊內部皆可使用；只需要遵守保留授權聲明的要求。

**這份指南有持續維護嗎？**
有。指南會隨 Claude Code 各版本更新。目前版本：v2.1.296（2026 年 10 月），相容於 Claude Code 2.1 以上版本。

**這和官方文件有什麼不同？**
官方文件是功能參考資料；本指南則是結合圖表、可用於正式環境的範本，以及漸進式學習路線的教學。兩者相輔相成——先透過本指南學習，需要確認細節時再查閱官方文件。

**學完所有內容需要多久？**
完整路線約需 11–13 小時。不過，只要 15 分鐘，你就能複製一個斜線指令範本並實際試用，立即體驗其價值。

**可以搭配 Claude Sonnet／Haiku／Opus 使用嗎？**
可以。所有範本均適用於 Claude Fable 5.1、Claude Fable 5、Claude Opus 5.5、Claude Opus 5、Claude Sonnet 5、Claude Sonnet 4.6、Claude Opus 4.8、Claude Haiku 5.5 及 Claude Haiku 4.5。

**我可以參與貢獻嗎？**
當然可以。請參閱 [CONTRIBUTING.md](CONTRIBUTING.md) 的說明。我們歡迎新範例、錯誤修正、文件改進，以及社群範本。

**可以離線閱讀嗎？**
可以。執行 `uv run scripts/build_epub.py`，即可產生包含全部內容及已渲染圖表的 EPUB 電子書。

---

## 從今天開始掌握 Claude Code

你已經安裝 Claude Code。想讓生產力提升十倍，關鍵就在於知道該如何使用它。本指南提供結構化學習路線、視覺化說明，以及可直接複製貼上的範本，幫助你達成目標。

MIT 授權。永久免費。你可以複製、Fork，並依自己的需求使用。

**[開始學習路線 →](LEARNING-ROADMAP.md)** | **[瀏覽功能目錄](CATALOG.md)** | **[15 分鐘快速入門](#15-分鐘快速入門)**

---

<details>
<summary>Quick Navigation — All Features</summary>

| Feature | Description | Folder |
|---------|-------------|--------|
| **Feature Catalog** | Complete reference with installation commands | [CATALOG.md](CATALOG.md) |
| **Slash Commands** | User-invoked shortcuts | [01-slash-commands/](01-slash-commands/) |
| **Memory** | Persistent context | [02-memory/](02-memory/) |
| **Skills** | Reusable capabilities | [03-skills/](03-skills/) |
| **Subagents** | Specialized AI assistants | [04-subagents/](04-subagents/) |
| **MCP Protocol** | External tool access | [05-mcp/](05-mcp/) |
| **Hooks** | Event-driven automation | [06-hooks/](06-hooks/) |
| **Plugins** | Bundled features | [07-plugins/](07-plugins/) |
| **Checkpoints** | Session snapshots & rewind | [08-checkpoints/](08-checkpoints/) |
| **Advanced Features** | Planning, thinking, background tasks | [09-advanced-features/](09-advanced-features/) |
| **CLI Reference** | Commands, flags, and options | [10-cli/](10-cli/) |
| **Blog Posts** | Real-world usage examples | [Blog Posts](https://medium.com/@luongnv89) |

</details>

<details>
<summary>Feature Comparison</summary>

| Feature | Invocation | Persistence | Best For |
|---------|-----------|------------|----------|
| **Slash Commands** | Manual (`/cmd`) | Session only | Quick shortcuts |
| **Memory** | Auto-loaded | Cross-session | Long-term learning |
| **Skills** | Auto-invoked | Filesystem | Automated workflows |
| **Subagents** | Auto-delegated | Isolated context | Task distribution |
| **MCP Protocol** | Auto-queried | Real-time | Live data access |
| **Hooks** | Event-triggered | Configured | Automation & validation |
| **Plugins** | One command | All features | Complete solutions |
| **Checkpoints** | Manual/Auto | Session-based | Safe experimentation |
| **Planning Mode** | Manual/Auto | Plan phase | Complex implementations |
| **Background Tasks** | Manual | Task duration | Long-running operations |
| **CLI Reference** | Terminal commands | Session/Script | Automation & scripting |

</details>

<details>
<summary>Installation Quick Reference</summary>

```bash
# Slash Commands
cp 01-slash-commands/*.md .claude/commands/

# Memory
cp 02-memory/project-CLAUDE.md ./CLAUDE.md

# Skills
cp -r 03-skills/code-review-specialist ~/.claude/skills/

# Subagents
cp 04-subagents/*.md .claude/agents/

# MCP
export GITHUB_TOKEN="token"
claude mcp add github -- npx -y @modelcontextprotocol/server-github

# Hooks
mkdir -p ~/.claude/hooks
cp 06-hooks/*.sh ~/.claude/hooks/
chmod +x ~/.claude/hooks/*.sh

# Plugins
/plugin install pr-review

# Checkpoints (auto-enabled, configure in settings)
# See 08-checkpoints/README.md

# Advanced Features (configure in settings)
# See 09-advanced-features/config-examples.json

# CLI Reference (no installation needed)
# See 10-cli/README.md for usage examples
```

</details>

<details>
<summary>01. Slash Commands</summary>

**Location**: [01-slash-commands/](01-slash-commands/)

**What**: User-invoked shortcuts stored as Markdown files

**Examples**:
- `optimize.md` - Code optimization analysis
- `pr.md` - Pull request preparation
- `generate-api-docs.md` - API documentation generator

**Installation**:
```bash
cp 01-slash-commands/*.md /path/to/project/.claude/commands/
```

**Usage**:
```
/optimize
/pr
/generate-api-docs
```

**Learn More**: [Discovering Claude Code Slash Commands](https://medium.com/@luongnv89/discovering-claude-code-slash-commands-cdc17f0dfb29)

</details>

<details>
<summary>02. Memory</summary>

**Location**: [02-memory/](02-memory/)

**What**: Persistent context across sessions

**Examples**:
- `project-CLAUDE.md` - Team-wide project standards
- `directory-api-CLAUDE.md` - Directory-specific rules
- `personal-CLAUDE.md` - Personal preferences

**Installation**:
```bash
# Project memory
cp 02-memory/project-CLAUDE.md /path/to/project/CLAUDE.md

# Directory memory
cp 02-memory/directory-api-CLAUDE.md /path/to/project/src/api/CLAUDE.md

# Personal memory
cp 02-memory/personal-CLAUDE.md ~/.claude/CLAUDE.md
```

**Usage**: Automatically loaded by Claude

</details>

<details>
<summary>03. Skills</summary>

**Location**: [03-skills/](03-skills/)

**What**: Reusable, auto-invoked capabilities with instructions and scripts

**Examples**:
- `code-review-specialist/` - Comprehensive code review with scripts
- `brand-voice/` - Brand voice consistency checker
- `doc-generator/` - API documentation generator

**Installation**:
```bash
# Personal skills
cp -r 03-skills/code-review-specialist ~/.claude/skills/

# Project skills
cp -r 03-skills/code-review-specialist /path/to/project/.claude/skills/
```

**Usage**: Automatically invoked when relevant

</details>

<details>
<summary>04. Subagents</summary>

**Location**: [04-subagents/](04-subagents/)

**What**: Specialized AI assistants with isolated contexts and custom prompts

**Examples**:
- `code-reviewer.md` - Comprehensive code quality analysis
- `test-engineer.md` - Test strategy and coverage
- `documentation-writer.md` - Technical documentation
- `secure-reviewer.md` - Security-focused review (read-only)
- `implementation-agent.md` - Full feature implementation

**Installation**:
```bash
cp 04-subagents/*.md /path/to/project/.claude/agents/
```

**Usage**: Automatically delegated by main agent

</details>

<details>
<summary>05. MCP Protocol</summary>

**Location**: [05-mcp/](05-mcp/)

**What**: Model Context Protocol for accessing external tools and APIs

**Examples**:
- `github-mcp.json` - GitHub integration
- `database-mcp.json` - Database queries
- `filesystem-mcp.json` - File operations
- `multi-mcp.json` - Multiple MCP servers

**Installation**:
```bash
# Set environment variables
export GITHUB_TOKEN="your_token"
export DATABASE_URL="postgresql://..."

# Add MCP server via CLI
claude mcp add github -- npx -y @modelcontextprotocol/server-github

# Or add to project .mcp.json manually (see 05-mcp/ for examples)
```

**Usage**: MCP tools are automatically available to Claude once configured

</details>

<details>
<summary>06. Hooks</summary>

**Location**: [06-hooks/](06-hooks/)

**What**: Event-driven shell commands that execute automatically in response to Claude Code events

**Examples**:
- `format-code.sh` - Auto-format code before writing
- `pre-commit.sh` - Run tests before commits
- `security-scan.sh` - Scan for security issues
- `log-bash.sh` - Log all bash commands
- `validate-prompt.sh` - Validate user prompts
- `notify-team.sh` - Send notifications on events

**Installation**:
```bash
mkdir -p ~/.claude/hooks
cp 06-hooks/*.sh ~/.claude/hooks/
chmod +x ~/.claude/hooks/*.sh
```

Configure hooks in `~/.claude/settings.json`:
```json
{
  "hooks": {
    "PreToolUse": [{
      "matcher": "Write",
      "hooks": ["~/.claude/hooks/format-code.sh"]
    }],
    "PostToolUse": [{
      "matcher": "Write",
      "hooks": ["~/.claude/hooks/security-scan.sh"]
    }]
  }
}
```

**Usage**: Hooks execute automatically on events

**Hook Types** (5): `command`, `http`, `prompt`, `mcp_tool`, `agent` — how a hook runs.

**Hook Events** (33, in 4 categories) — when it runs:
- **Tool Hooks**: `PreToolUse`, `PostToolUse`, `PostToolUseFailure`, `PostToolBatch`, `PermissionRequest`, `PermissionDenied`
- **Session Hooks**: `SessionStart`, `Setup`, `SessionEnd`, `Stop`, `StopFailure`, `SubagentStart`, `SubagentStop`
- **Task Hooks**: `UserPromptSubmit`, `UserPromptExpansion`, `MessageDisplay`, `TaskCompleted`, `TaskCreated`, `TeammateIdle` — `TaskCompleted` and `TaskCreated` only fire when the todo tools are enabled, which is available by default only on Claude 3.x models, Opus 4 through 4.7, Sonnet 4 through 4.6, and Haiku 4.5 (`CLAUDE_CODE_ENABLE_TODO_TOOLS=1` restores them)
- **Lifecycle Hooks**: `ConfigChange`, `CwdChanged`, `DirectoryAdded`, `FileChanged`, `PreCompact`, `PostCompact`, `PreModelSwitch`, `PostModelSwitch`, `WorktreeCreate`, `WorktreeRemove`, `Notification`, `InstructionsLoaded`, `Elicitation`, `ElicitationResult`

</details>

<details>
<summary>07. Plugins</summary>

**Location**: [07-plugins/](07-plugins/)

**What**: Bundled collections of commands, agents, MCP, and hooks

**Examples**:
- `pr-review/` - Complete PR review workflow
- `devops-automation/` - Deployment and monitoring
- `documentation/` - Documentation generation

**Installation**:
```bash
/plugin install pr-review
/plugin install devops-automation
/plugin install documentation
```

**Usage**: Use bundled slash commands and features

</details>

<details>
<summary>08. Checkpoints and Rewind</summary>

**Location**: [08-checkpoints/](08-checkpoints/)

**What**: Save conversation state and rewind to previous points to explore different approaches

**Key Concepts**:
- **Checkpoint**: Snapshot of conversation state
- **Rewind**: Return to previous checkpoint
- **Branch Point**: Explore multiple approaches from same checkpoint

**Usage**:
```
# Checkpoints are created automatically with every user prompt
# To rewind, press Esc twice or use:
/rewind

# Then choose from five options:
# 1. Restore code and conversation
# 2. Restore conversation
# 3. Restore code
# 4. Summarize from here
# 5. Never mind
```

**Use Cases**:
- Try different implementation approaches
- Recover from mistakes
- Safe experimentation
- Compare alternative solutions
- A/B testing different designs

</details>

<details>
<summary>09. Advanced Features</summary>

**Location**: [09-advanced-features/](09-advanced-features/)

**What**: Advanced capabilities for complex workflows and automation

**Includes**:
- **Planning Mode** — Create detailed implementation plans before coding
- **Extended Thinking** — Deep reasoning for complex problems (toggle with `Alt+T` / `Option+T`)
- **Background Tasks** — Run long operations without blocking
- **Permission Modes** — `manual` (formerly `default`; `default` still accepted), `acceptEdits`, `plan`, `auto`, `dontAsk`, `bypassPermissions`
- **Headless Mode** — Run Claude Code in CI/CD: `claude -p "Run tests and generate report"`
- **Session Management** — `/resume`, `/rename`, `/fork`, `/branch`, `claude -c`, `claude -r`
- **Configuration** — Customize behavior in `~/.claude/settings.json`

See [config-examples.json](09-advanced-features/config-examples.json) for complete configurations.

</details>

<details>
<summary>10. CLI Reference</summary>

**Location**: [10-cli/](10-cli/)

**What**: Complete command-line interface reference for Claude Code

**Quick Examples**:
```bash
# Interactive mode
claude "explain this project"

# Print mode (non-interactive)
claude -p "review this code"

# Process file content
cat error.log | claude -p "explain this error"

# JSON output for scripts
claude -p --output-format json "list functions"

# Resume session
claude -r "feature-auth" "continue implementation"
```

**Use Cases**: CI/CD pipeline integration, script automation, batch processing, multi-session workflows, custom agent configurations

</details>

<details>
<summary>Example Workflows</summary>

### Complete Code Review Workflow

```markdown
# Uses: Slash Commands + Subagents + Memory + MCP

User: /review-pr

Claude:
1. Loads project memory (coding standards)
2. Fetches PR via GitHub MCP
3. Delegates to code-reviewer subagent
4. Delegates to test-engineer subagent
5. Synthesizes findings
6. Provides comprehensive review
```

### Automated Documentation

```markdown
# Uses: Skills + Subagents + Memory

User: "Generate API documentation for the auth module"

Claude:
1. Loads project memory (doc standards)
2. Detects doc generation request
3. Auto-invokes doc-generator skill
4. Delegates to api-documenter subagent
5. Creates comprehensive docs with examples
```

### DevOps Deployment

```markdown
# Uses: Plugins + MCP + Hooks

User: /deploy production

Claude:
1. Runs pre-deploy hook (validates environment)
2. Delegates to deployment-specialist subagent
3. Executes deployment via Kubernetes MCP
4. Monitors progress
5. Runs post-deploy hook (health checks)
6. Reports status
```

</details>

<details>
<summary>Directory Structure</summary>

```
├── 01-slash-commands/
│   ├── optimize.md
│   ├── pr.md
│   ├── generate-api-docs.md
│   └── README.md
├── 02-memory/
│   ├── project-CLAUDE.md
│   ├── directory-api-CLAUDE.md
│   ├── personal-CLAUDE.md
│   └── README.md
├── 03-skills/
│   ├── code-review-specialist/
│   │   ├── SKILL.md
│   │   ├── scripts/
│   │   └── templates/
│   ├── brand-voice/
│   │   ├── SKILL.md
│   │   └── templates/
│   ├── doc-generator/
│   │   ├── SKILL.md
│   │   └── generate-docs.py
│   └── README.md
├── 04-subagents/
│   ├── code-reviewer.md
│   ├── test-engineer.md
│   ├── documentation-writer.md
│   ├── secure-reviewer.md
│   ├── implementation-agent.md
│   └── README.md
├── 05-mcp/
│   ├── github-mcp.json
│   ├── database-mcp.json
│   ├── filesystem-mcp.json
│   ├── multi-mcp.json
│   └── README.md
├── 06-hooks/
│   ├── format-code.sh
│   ├── pre-commit.sh
│   ├── security-scan.sh
│   ├── log-bash.sh
│   ├── validate-prompt.sh
│   ├── notify-team.sh
│   └── README.md
├── 07-plugins/
│   ├── pr-review/
│   ├── devops-automation/
│   ├── documentation/
│   └── README.md
├── 08-checkpoints/
│   ├── checkpoint-examples.md
│   └── README.md
├── 09-advanced-features/
│   ├── config-examples.json
│   ├── planning-mode-examples.md
│   └── README.md
├── 10-cli/
│   └── README.md
└── README.md (this file)
```

</details>

<details>
<summary>Best Practices</summary>

### Do's
- Start simple with slash commands
- Add features incrementally
- Use memory for team standards
- Test configurations locally first
- Document custom implementations
- Version control project configurations
- Share plugins with team

### Don'ts
- Don't create redundant features
- Don't hardcode credentials
- Don't skip documentation
- Don't over-complicate simple tasks
- Don't ignore security best practices
- Don't commit sensitive data

</details>

<details>
<summary>Troubleshooting</summary>

### Feature Not Loading
1. Check file location and naming
2. Verify YAML frontmatter syntax
3. Check file permissions
4. Review Claude Code version compatibility

### MCP Connection Failed
1. Verify environment variables
2. Check MCP server installation
3. Test credentials
4. Review network connectivity

### Subagent Not Delegating
1. Check tool permissions
2. Verify agent description clarity
3. Review task complexity
4. Test agent independently

</details>

<details>
<summary>Testing</summary>

This project includes comprehensive automated testing:

- **Unit Tests**: Python tests using pytest (Python 3.10, 3.11, 3.12)
- **Code Quality**: Linting and formatting with Ruff
- **Security**: Vulnerability scanning with Bandit
- **Type Checking**: Static type analysis with mypy
- **Build Verification**: EPUB generation testing
- **Coverage Tracking**: Codecov integration

```bash
# Install development dependencies
uv pip install -r requirements-dev.txt

# Run all unit tests
pytest scripts/tests/ -v

# Run tests with coverage report
pytest scripts/tests/ -v --cov=scripts --cov-report=html

# Run code quality checks
ruff check scripts/
ruff format --check scripts/

# Run security scan
bandit -c pyproject.toml -r scripts/ --exclude scripts/tests/

# Run type checking
mypy scripts/ --ignore-missing-imports
```

Tests run automatically on every push to `main`/`develop` and every PR to `main`. See [TESTING.md](.github/TESTING.md) for detailed information.

</details>

<details>
<summary>EPUB Generation</summary>

Want to read this guide offline? Generate an EPUB ebook:

```bash
uv run scripts/build_epub.py
```

This creates `claude-howto-guide.epub` with all content, including rendered Mermaid diagrams.

See [scripts/README.md](scripts/README.md) for more options.

</details>

<details>
<summary>Contributing</summary>

Found an issue or want to contribute an example? We'd love your help!

**Please read [CONTRIBUTING.md](CONTRIBUTING.md) for detailed guidelines on:**
- Types of contributions (examples, docs, features, bugs, feedback)
- How to set up your development environment
- Directory structure and how to add content
- Writing guidelines and best practices
- Commit and PR process

**Our Community Standards:**
- [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) - How we treat each other
- [SECURITY.md](SECURITY.md) - Security policy and vulnerability reporting

### Reporting Security Issues

If you discover a security vulnerability, please report it responsibly:

1. **Use GitHub Private Vulnerability Reporting**: https://github.com/luongnv89/claude-howto/security/advisories
2. **Or read** [.github/SECURITY_REPORTING.md](.github/SECURITY_REPORTING.md) for detailed instructions
3. **Do NOT** open a public issue for security vulnerabilities

Quick start:
1. Fork and clone the repository
2. Create a descriptive branch (`add/feature-name`, `fix/bug`, `docs/improvement`)
3. Make your changes following the guidelines
4. Submit a pull request with a clear description

**Need help?** Open an issue or discussion, and we'll guide you through the process.

</details>

<details>
<summary>Additional Resources</summary>

- [Claude Code Documentation](https://code.claude.com/docs/en/overview)
- [MCP Protocol Specification](https://modelcontextprotocol.io)
- [Skills Repository](https://github.com/luongnv89/skills) - Collection of ready-to-use skills
- [Anthropic Cookbook](https://github.com/anthropics/anthropic-cookbook)
- [Boris Cherny's Claude Code Workflow](https://x.com/bcherny/status/2007179832300581177) - The creator of Claude Code shares his systematized workflow: parallel agents, shared CLAUDE.md, Plan mode, slash commands, subagents, and verification hooks for autonomous long-running sessions.

</details>

---

## Contributing

We welcome contributions! Please see our [Contributing Guide](CONTRIBUTING.md) for details on how to get started.

---

## License

MIT License - see [LICENSE](LICENSE). Free to use, modify, and distribute. The only requirement is including the license notice.

---

**Last Updated**: October 10, 2026
**Claude Code Version**: 2.1.296
**Sources**:
- https://code.claude.com/docs/en/tools-reference#task-tool-availability
- https://code.claude.com/docs/en/hooks
- https://code.claude.com/docs/en/overview
- https://code.claude.com/docs/en/changelog
- https://code.claude.com/docs/en/permission-modes
- https://platform.claude.com/docs/en/about-claude/models/overview
- https://github.com/anthropics/claude-code/releases
- https://github.com/anthropics/claude-code/releases/tag/v2.1.154
- https://code.claude.com/docs/en/model-config
- https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md
- https://github.com/anthropics/claude-code/releases/tag/v2.1.296
**Compatible Models**: Claude Fable 5.1, Claude Fable 5, Claude Opus 5, Claude Sonnet 5, Claude Sonnet 4.6, Claude Opus 4.8, Claude Haiku 4.5
