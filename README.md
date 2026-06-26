<div align="center">

<img src="https://raw.githubusercontent.com/sumitsingh4411/repo-agent/main/media/icon.png" width="128" alt="Free Repo Agent — free AI coding agent for VS Code" />

# Free Repo Agent

### 🚀 The free AI coding agent for VS Code

**A no-subscription [GitHub Copilot](#-vs-copilot-cursor--claude) · Cursor · Claude alternative** — repo-aware chat, an autonomous agent that **edits files & runs commands**, **vision (screenshot → component)**, **MCP plugins**, **project memory**, and **staff-engineer code review**. Powered by **DeepSeek** — bring your own key, pay only cents.

<br/>

![Agent mode](https://img.shields.io/badge/🤖_Autonomous_agent-0b6cff?style=for-the-badge)
![Vision](https://img.shields.io/badge/👁️_Screenshot_→_code-7c4dff?style=for-the-badge)
![MCP](https://img.shields.io/badge/🧩_MCP_plugins-1aa260?style=for-the-badge)
![Review](https://img.shields.io/badge/🔍_AI_code_review-ff6d00?style=for-the-badge)
![Memory](https://img.shields.io/badge/🧠_Project_memory-e91e63?style=for-the-badge)

<br/>

[![VS Code Marketplace](https://img.shields.io/visual-studio-marketplace/v/SUMITKUMARSINGH.free-repo-agent?label=Marketplace&color=0b6cff&logo=visualstudiocode)](https://marketplace.visualstudio.com/items?itemName=SUMITKUMARSINGH.free-repo-agent)
[![Installs](https://img.shields.io/visual-studio-marketplace/i/SUMITKUMARSINGH.free-repo-agent?color=0b6cff&label=installs)](https://marketplace.visualstudio.com/items?itemName=SUMITKUMARSINGH.free-repo-agent)
[![Rating](https://img.shields.io/visual-studio-marketplace/r/SUMITKUMARSINGH.free-repo-agent?color=ffb020)](https://marketplace.visualstudio.com/items?itemName=SUMITKUMARSINGH.free-repo-agent&ssr=false#review-details)
[![Price: Free](https://img.shields.io/badge/price-free-2ea44f)](https://marketplace.visualstudio.com/items?itemName=SUMITKUMARSINGH.free-repo-agent)
[![GitHub stars](https://img.shields.io/github/stars/sumitsingh4411/repo-agent?style=social)](https://github.com/sumitsingh4411/repo-agent)

<br/>

[![Install in VS Code](https://img.shields.io/badge/⬇️_Install_in_VS_Code-0b6cff?style=for-the-badge&logo=visualstudiocode&logoColor=white)](https://marketplace.visualstudio.com/items?itemName=SUMITKUMARSINGH.free-repo-agent)

<sub>

Built with [![VS Code](https://img.shields.io/badge/-VS_Code-007ACC?logo=visualstudiocode&logoColor=white)](https://code.visualstudio.com) [![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?logo=typescript&logoColor=white)](https://www.typescriptlang.org) [![DeepSeek](https://img.shields.io/badge/-DeepSeek-4d6bfe)](https://platform.deepseek.com) [![MCP](https://img.shields.io/badge/-MCP-1aa260)](https://modelcontextprotocol.io) [![MIT](https://img.shields.io/badge/-MIT-blue)](LICENSE)

</sub>

**[🚀 Get started](#-get-started-in-60-seconds) &nbsp;•&nbsp; [✨ Features](#-everything-it-does) &nbsp;•&nbsp; [🧩 Plugins](#-plugins-mcp--give-the-agent-superpowers) &nbsp;•&nbsp; [🐞 Report a bug](https://github.com/sumitsingh4411/repo-agent/issues/new)**

</div>

---

> **Free Repo Agent** brings a Claude/Cursor/Cline-style **agent** into VS Code. It indexes your whole repository, writes and edits code with inline **Keep / Undo**, runs terminal commands with your approval, **verifies its own work** (typecheck/build → then fixes the errors), **reads images** (paste a UI → build the component), extends itself with **MCP plugins**, remembers your project, and runs a **staff-engineer pre-commit code review** — all on the affordable DeepSeek API with **no monthly subscription**.

<div align="center">

**Looking for a free Copilot alternative · Cursor alternative · Claude / ChatGPT coding agent · Cline / Continue / Aider alternative?** This is the lightweight, bring-your-own-key one.

</div>

## 📚 Contents

<table>
<tr>
<td>

- [⚡ Everything it does](#-everything-it-does)
- [🚀 Get started in 60 seconds](#-get-started-in-60-seconds)
- [🤖 Autonomous agent](#-autonomous-agent--self-verifying)
- [👁️ Vision — image → code](#%EF%B8%8F-vision--paste-an-image-build-the-component)

</td>
<td>

- [🧩 Plugins (MCP)](#-plugins-mcp--give-the-agent-superpowers)
- [🧠 Project memory](#-project-memory--memorymd)
- [🔍 Code review + custom rules](#-staff-engineer-code-review--your-own-rules)
- [🧭 Repo indexing](#-repo-aware-indexing--retrieval)

</td>
<td>

- [⚙️ Commands](#%EF%B8%8F-commands)
- [🔧 Settings](#-settings)
- [🆚 vs Copilot/Cursor/Claude](#-vs-copilot-cursor--claude)
- [❓ FAQ](#-faq) · [🐞 Report a bug](#-report-a-bug--request-a-feature)

</td>
</tr>
</table>

## ⚡ Everything it does

<table>
<tr>
<td width="50%" valign="top">

### 💬 Repo-aware chat
Ask anything about your codebase. It **indexes your project** and injects the most relevant files into every answer — no copy-pasting context.

</td>
<td width="50%" valign="top">

### 🤖 Autonomous agent
Give it a task — it reads files, **edits across many files**, and **runs commands** step by step. Every change is reviewed **inline** with **✓ Keep / ✗ Undo**.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### ✅ Auto-verify & self-fix
After editing it runs your **typecheck/build**, reads the errors, and **fixes them before saying "done"** — no more code that doesn't compile.

</td>
<td width="50%" valign="top">

### 👁️ Vision (image → code)
Paste a **UI screenshot/mockup** and say *"build this component."* **Free by default** via Google Gemini (or local Ollama). Falls back to OCR for screenshots of code/errors.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🧩 Plugins (MCP)
One-click tools the agent can use — **GitHub, web search, Postgres, Playwright, filesystem** & more — via the **Model Context Protocol**. Add any custom server.

</td>
<td width="50%" valign="top">

### 🔍 Staff-engineer code review
Reviews staged changes / files / branches, reads the **full files**, runs a **second audit pass**, and reports **Critical · Quality · Architecture · Testing**. Enforces **your own rules**.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🧠 Project memory
A `memory.md` injected into **every** prompt so the agent always remembers your **stack, conventions, and rules**.

</td>
<td width="50%" valign="top">

### ☑️ Live task checklist · 🧠 Thinking · 📎 Uploads
A Claude-style **task checklist**, streamed **chain-of-thought**, `@`-mention any file, and attach **PDFs / images**.

</td>
</tr>
</table>

## 🚀 Get started in 60 seconds

**1. Get a DeepSeek API key** → [platform.deepseek.com/api_keys](https://platform.deepseek.com/api_keys) — pay-as-you-go, a few dollars lasts a long time.

**2. Add it to VS Code** → <kbd>Cmd/Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>P</kbd> → **`Agent: Set DeepSeek API Key`** (stored in VS Code SecretStorage, never in your repo).

**3. Open chat** → press <kbd>Cmd/Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>A</kbd>, or click the **Repo Agent `</>` icon** to dock it beside your code — and start.

> 💡 Type <kbd>/</kbd> in the chat for quick commands: **Plugins, Memory, Reindex, Auto-accept, Vision** and more.

## 🤖 Autonomous agent — self-verifying

Describe a task and watch it work end-to-end:

> *"Add a `/health` route and a test for it, then run the tests."*

1. 📖 Reads the relevant files (from the repo index).
2. ✍️ Proposes edits **inline in your files** with green highlights and **✓ Keep / ✗ Undo**.
3. ▶️ Asks to **Run** any terminal command in a visible *Repo Agent* terminal.
4. ✅ **Auto-verifies** — runs your typecheck/build and **fixes errors** before finishing.
5. ☑️ A **live checklist** ticks each step `pending → in-progress → ✓ done`. Hit **Stop** anytime.

## 👁️ Vision — paste an image, build the component

DeepSeek is text-only, so image understanding uses a **separate, free-by-default** vision model.

```text
/  →  👁️ Vision  →  choose a provider:
     • Google Gemini — FREE (no credit card)   ← default
     • Ollama / LM Studio — local, no key
     • OpenRouter (free models) · OpenAI · Custom
```

Then **paste a screenshot/mockup** into the chat and ask *"build this as a React component."* The vision model turns the image into a precise implementation spec, and the agent builds the files. No key? Images fall back to **OCR** — perfect for screenshots of errors or code.

## 🧩 Plugins (MCP) — give the agent superpowers

Open the **🧩 Plugins** panel (or type <kbd>/</kbd> → **Plugins**) and add tools with one click. Built on the **Model Context Protocol** — the same plugin standard Claude uses — so the entire MCP ecosystem works here.

| | Plugin | What the agent can do |
|---|---|---|
| 📁 | **Filesystem** | Read/write/search files in a folder you allow |
| 🐙 | **GitHub** | Search repos/issues, read files, open PRs & issues |
| 🦊 | **GitLab** | Repos, issues, merge requests |
| 🔎 | **Web Search** (Brave) | Search the web for up-to-date info |
| 🦅 | **Tavily** | AI-grade web search & page extraction |
| 🌐 | **Fetch** | Fetch a URL as clean text/markdown |
| 🎭 | **Playwright** | Drive a real browser: click, fill, scrape, screenshot |
| 🐘 | **Postgres** · 🗃️ **SQLite** | Query your databases |
| 🪜 | **Sequential Thinking** | Structured step-by-step reasoning |
| 📚 | **Context7** | Up-to-date docs & snippets for any library |
| 🧠 | **Memory** | A knowledge graph the agent reads/writes across tasks |
| 🗺️ | **Google Maps** · 💬 **Slack** | Places/directions · channels & messages |

> ➕ **Add any custom MCP server** from the same panel — just give it a command + args. Keys are stored securely in VS Code SecretStorage.

## 🧠 Project memory — `memory.md`

Type <kbd>/</kbd> → **Memory** to create a `memory.md` at your repo root. Its contents are injected into **every** chat and agent prompt, so the agent always remembers your project:

```markdown
# Project Memory

## Project
- Stack: React + TypeScript + Vite, Node/Express API, Postgres
- Run: `npm run dev` · Tests: `npm test`

## Conventions
- 2-space indent, single quotes, named exports.
- Always add types and a test. Never commit secrets or use `any`.
```

Delete the file to turn memory off. (You can also drop a `.agent.md` / `.claude.md` — it reads those too.)

## 🔍 Staff-engineer code review + your own rules

Stage changes (`git add …`) → **Agent: Review Staged Changes** (also in the Source Control title bar). Findings appear in the **Problems** panel, the **Review Results** sidebar, and **inline** — each with **Fix with AI**, **Ignore**, and **Commit Anyway**.

**Make it enforce YOUR standards.** Run **Agent: Create Review Guidelines** to scaffold a `system-design.md`. The reviewer reads it before every review and flags any change that breaks a rule — quoting the rule:

```markdown
# Review Guidelines & System Design

## Architecture
- UI → services → data access. UI must not import data-access directly.

## Review rules
- No `console.log` in committed code — use the logger.
- Every new exported function ships with a test.
- No secrets in source; read them from config/secret storage.
```

## 🧭 Repo-aware indexing & retrieval

On first run, Repo Agent **indexes your repository** — symbols, structure, and optional AI per-file summaries — into a local cache (`.agent-cache/`). Every question then pulls in the **most relevant files automatically**, so answers fit *your* codebase. Re-run anytime with **Agent: Reindex Repository**, and tune what's indexed via `repoAgent.indexing.*` and how many files are injected via `repoAgent.retrieval.maxFiles`.

## ⚙️ Commands

<kbd>Cmd/Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>P</kbd> → type **"Agent:"**

| Command | Description |
|---|---|
| `Agent: Chat` / `Open Chat (beside editor)` | Open the chat panel |
| `Agent: Generate Code` | Describe code to generate |
| `Agent: Run Agent (autonomous)` | Run a task that edits files & runs commands |
| `Agent: Review Staged Changes` / `Review Current File` | Pre-commit / file review |
| `Agent: Create Review Guidelines` | Scaffold a `system-design.md` of review rules |
| `Agent: Edit Memory` | Edit the always-on `memory.md` |
| `Agent: Choose Vision Provider` | Pick a vision backend (Gemini free / Ollama / …) |
| `Agent: Reindex Repository` / `Explain Architecture` | Index & architecture tools |
| `Agent: Set / Clear DeepSeek API Key` | Manage your key |

## 🔧 Settings

<details>
<summary>All settings live under <code>repoAgent.*</code> — click to expand</summary>

| Setting | Default | Description |
|---|---|---|
| `deepseek.model` | `deepseek-chat` | Model for generation & review |
| `deepseek.reasoningModel` | `deepseek-reasoner` | Model used when **Think** is on |
| `deepseek.showThinking` | `true` | Show reasoning by default |
| `deepseek.baseUrl` | `https://api.deepseek.com` | API base URL (OpenAI-compatible) |
| `deepseek.maxTokens` | `4096` | Max tokens per response |
| `vision.baseUrl` / `vision.model` | Gemini free | OpenAI-compatible vision endpoint |
| `review.guidelinesFile` | `system-design.md` | Your custom review-rules file |
| `review.deepAudit` | `true` | Second audit pass for fewer false positives |
| `indexing.maxFiles` | `1500` | Index size cap |
| `indexing.generateSummaries` | `true` | AI per-file summaries (set `false` for $0 indexing) |
| `retrieval.maxFiles` | `8` | Relevant files injected per prompt |
| `plugins.autoRun` | `true` | Run plugin tools without a confirm prompt |
| `review.autoOnSave` | `false` | Auto-review files on save |

</details>

## 🆚 vs Copilot, Cursor & Claude

| | **Free Repo Agent** | Copilot | Cursor | Claude / Cline |
|---|:---:|:---:|:---:|:---:|
| **Price** | 🟢 **Free** (BYO key) | 💲 Subscription | 💲 Subscription | 💲 Sub / BYO |
| Repo-aware multi-file agent | ✅ | ✅ | ✅ | ✅ |
| Runs terminal commands | ✅ | ✅ | ✅ | ✅ |
| **Self-verifies** (build/typecheck) | ✅ | — | ◐ | — |
| **Vision:** screenshot → code | ✅ free | — | ✅ | ✅ |
| **MCP plugins** | ✅ | — | ✅ | ✅ |
| **Code review + custom rules** | ✅ | ◐ | — | — |
| **Project memory file** | ✅ | ◐ | ◐ | ✅ |

A free alternative to **GitHub Copilot, Cursor, Claude, Codex, Cline, Continue, Codeium, Windsurf, Tabnine, Cody, Aider & Roo Code** — a lightweight, bring-your-own-key agent that edits code, self-verifies, and reviews diffs inside VS Code.

## ❓ FAQ

<details><summary><b>Is it really free?</b></summary><br/>Yes — the extension is free and open. You only pay DeepSeek's low pay-as-you-go API usage (your own key).</details>
<details><summary><b>Is it a good Copilot / Cursor / Claude / Cline alternative?</b></summary><br/>Yes — repo-aware chat, an autonomous agent that edits files and runs commands, visible reasoning, vision, MCP plugins, and pre-commit code review — the same core workflow, no subscription.</details>
<details><summary><b>Does it fix its own mistakes?</b></summary><br/>Yes — after editing it runs your typecheck/build, reads the errors, and fixes them before finishing.</details>
<details><summary><b>Can I add plugins / MCP servers?</b></summary><br/>Yes — open the 🧩 Plugins panel and add GitHub, web search, Postgres, Playwright and more with one click, or any custom MCP server (needs Node/npx).</details>
<details><summary><b>Does my code leave my machine?</b></summary><br/>Only the context needed for a request is sent to the DeepSeek API when you ask. Your key never leaves SecretStorage; the index is cached locally under <code>.agent-cache/</code>.</details>

## 🐞 Report a bug / request a feature

Found a bug or have an idea? **[Open an issue →](https://github.com/sumitsingh4411/repo-agent/issues/new)** — you'll get a guided **bug report** or **feature request** form. Please include your extension version, VS Code version, steps to reproduce, and any error from **View → Output → "Repo Agent"**. Browse existing reports on the **[Issues page](https://github.com/sumitsingh4411/repo-agent/issues)**.

## ⭐ Star history

<a href="https://star-history.com/#sumitsingh4411/repo-agent&Date">
  <img src="https://api.star-history.com/svg?repos=sumitsingh4411/repo-agent&type=Date" width="600" alt="Star history chart" />
</a>

<div align="center">

---

### ⭐ If Free Repo Agent saves you time, [star it](https://github.com/sumitsingh4411/repo-agent) and [leave a review](https://marketplace.visualstudio.com/items?itemName=SUMITKUMARSINGH.free-repo-agent&ssr=false#review-details) — it helps others find it.

**MIT licensed**

<sub>Free AI coding agent · AI coding assistant · GitHub Copilot alternative · free Copilot · Cursor alternative · Claude alternative · Codex alternative · Cline / Continue / Codeium / Windsurf / Tabnine / Cody / Aider / Roo Code alternative · ChatGPT for VS Code · DeepSeek VS Code extension · DeepSeek Coder · MCP · Model Context Protocol · MCP client · AI code review · AI code reviewer · custom review rules · vision AI coding · screenshot to code · image to code · UI to code · AI pair programming · agent mode · autonomous coding agent · self-verifying AI agent · project memory · repo indexing · AI refactoring · AI code generation · repo-aware AI assistant · bring your own key AI.</sub>

</div>
