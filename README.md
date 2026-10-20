<div align="center">

<img src="https://raw.githubusercontent.com/sumitsingh4411/repo-agent/main/media/icon.png" width="128" alt="Free Repo Agent — free AI coding agent for VS Code" />

# Free Repo Agent

### 🚀 The free DeepSeek AI coding agent for VS Code

**A no-subscription [GitHub Copilot](#-vs-copilot-cursor--claude) · Cursor · Claude Code alternative** — repo-aware chat, an autonomous agent that **edits files & runs commands**, a **DeepSeek V4.1 Flash / V4 Pro model switcher with thinking mode**, a **terminal CLI**, **vision (screenshot → component)**, **MCP plugins**, **project memory**, and **staff-engineer code review**. Bring your own key, pay only cents — or plug in **GPT / Claude / any model** via an OpenAI-compatible URL.

<br/>

![Agent mode](https://img.shields.io/badge/🤖_Autonomous_agent-0b6cff?style=for-the-badge)
![Models](https://img.shields.io/badge/🧠_DeepSeek_V4.1_+_thinking-4d6bfe?style=for-the-badge)
![Vision](https://img.shields.io/badge/👁️_Screenshot_→_code-7c4dff?style=for-the-badge)
![MCP](https://img.shields.io/badge/🧩_MCP_plugins-1aa260?style=for-the-badge)
![Review](https://img.shields.io/badge/🔍_AI_code_review-ff6d00?style=for-the-badge)
![CLI](https://img.shields.io/badge/⌨️_Terminal_CLI-222222?style=for-the-badge)

<br/>

[![VS Code Marketplace](https://img.shields.io/visual-studio-marketplace/v/SUMITKUMARSINGH.free-repo-agent?label=Marketplace&color=0b6cff&logo=visualstudiocode)](https://marketplace.visualstudio.com/items?itemName=SUMITKUMARSINGH.free-repo-agent)
[![Installs](https://img.shields.io/visual-studio-marketplace/i/SUMITKUMARSINGH.free-repo-agent?color=0b6cff&label=installs)](https://marketplace.visualstudio.com/items?itemName=SUMITKUMARSINGH.free-repo-agent)
[![Rating](https://img.shields.io/visual-studio-marketplace/r/SUMITKUMARSINGH.free-repo-agent?color=ffb020)](https://marketplace.visualstudio.com/items?itemName=SUMITKUMARSINGH.free-repo-agent&ssr=false#review-details)
[![Price: Free](https://img.shields.io/badge/price-free-2ea44f)](https://marketplace.visualstudio.com/items?itemName=SUMITKUMARSINGH.free-repo-agent)
[![GitHub stars](https://img.shields.io/github/stars/sumitsingh4411/repo-agent?style=social)](https://github.com/sumitsingh4411/repo-agent)

<br/>

[![Install in VS Code](https://img.shields.io/badge/⬇️_Install_in_VS_Code-0b6cff?style=for-the-badge&logo=visualstudiocode&logoColor=white)](https://marketplace.visualstudio.com/items?itemName=SUMITKUMARSINGH.free-repo-agent)
[![Install from Open VSX](https://img.shields.io/badge/⬇️_Cursor_·_Windsurf_·_VSCodium-Open_VSX-a60ee5?style=for-the-badge)](https://open-vsx.org/extension/SUMITKUMARSINGH/free-repo-agent)

<sub>

Built with [![VS Code](https://img.shields.io/badge/-VS_Code-007ACC?logo=visualstudiocode&logoColor=white)](https://code.visualstudio.com) [![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?logo=typescript&logoColor=white)](https://www.typescriptlang.org) [![DeepSeek](https://img.shields.io/badge/-DeepSeek-4d6bfe)](https://platform.deepseek.com) [![MCP](https://img.shields.io/badge/-MCP-1aa260)](https://modelcontextprotocol.io) [![MIT](https://img.shields.io/badge/-MIT-blue)](LICENSE)

</sub>

**[🚀 Get started](#-get-started-in-60-seconds) &nbsp;•&nbsp; [✨ Features](#-everything-it-does) &nbsp;•&nbsp; [🧩 Plugins](#-plugins-mcp--give-the-agent-superpowers) &nbsp;•&nbsp; [🐞 Report a bug](https://github.com/sumitsingh4411/repo-agent/issues/new)**

</div>

---

> **Free Repo Agent** brings a Claude/Cursor/Cline-style **agent** into VS Code. It indexes your whole repository, writes and edits code with inline **Keep / Undo**, runs terminal commands with your approval, **verifies its own work** (typecheck/build → then fixes the errors), lets you **switch models** (DeepSeek **V4 Pro / V4 Flash** with **thinking mode**, or any OpenAI-compatible model), tunes **effort** (fast → max reasoning), **reads images** (paste a UI → build the component), extends itself with **MCP plugins (local & remote)**, learns your codebase, remembers your project, and runs a **staff-engineer pre-commit code review** — all on the affordable DeepSeek API with **no monthly subscription**.

<div align="center">

**Looking for a free Copilot alternative · Cursor alternative · Claude Code alternative · Cline / Roo Code / Kilo Code / Continue / Aider alternative · or the best DeepSeek extension for VS Code?** This is the lightweight, bring-your-own-key one.

</div>

## 📚 Contents

<table>
<tr>
<td>

- [✨ What's new in 0.12](#-whats-new-in-012)
- [⚡ Everything it does](#-everything-it-does)
- [🚀 Get started in 60 seconds](#-get-started-in-60-seconds)
- [🧠 Models & thinking mode](#-models--thinking-mode--generate-the-best-code)
- [📖 Learn this codebase](#-learn-this-codebase)
- [👁️ Vision — image → code](#%EF%B8%8F-vision--paste-an-image-build-the-component)

</td>
<td>

- [🧩 Plugins (MCP)](#-plugins-mcp--give-the-agent-superpowers)
- [🧠 Project memory](#-project-memory--memorymd)
- [🔍 Code review + custom rules](#-staff-engineer-code-review--your-own-rules)
- [🧭 Repo indexing](#-repo-aware-indexing--retrieval)

</td>
<td>

- [🛠️ In your editor](#%EF%B8%8F-in-your-editor--power-tools)
- [⌨️ Terminal CLI](#%EF%B8%8F-terminal-cli--the-agent-in-your-shell)
- [⚙️ Commands](#%EF%B8%8F-commands)
- [🔧 Settings](#-settings)
- [🆚 vs Copilot/Cursor/Claude](#-vs-copilot-cursor--claude)
- [❓ FAQ](#-faq) · [🐞 Report a bug](#-report-a-bug--request-a-feature)

</td>
</tr>
</table>

## ✨ What's new in 0.12

The biggest update yet — the features people compare coding agents on:

- **📋 Plan mode** — the agent investigates read-only and proposes a step-by-step plan; click **▶ Execute plan** to run it.
- **↺ Checkpoints** — hover any message and click **↺ Restore** to undo every file the agent changed since then and rewind the chat.
- **✍️ Inline autocomplete** — grey suggestions as you type, **Tab** to accept (DeepSeek fill-in-the-middle). Off by default — turn it on from the status bar.
- **💡 Quick Fix & right-click** — **✨ Fix with Repo Agent** on any red squiggle; right-click code → Explain · Fix · Refactor · Write tests · Add docs.
- **✨ AI commit messages** — a sparkle button in Source Control writes the message from your staged changes.
- **🔎 Sharper agent** — exact **grep**, the **Problems** panel, **go-to-definition / find-references**, **web fetch**, and **parallel research subagents**. A loop guard stops it repeating itself.
- **⧉ Multiple chat tabs**, **`AGENTS.md`** support, new mentions **`@problems` `@diff` `@terminal` `@https://…`**, **custom `/commands`**, **hooks**, and **long-chat memory**.
- **⌨️ CLI:** plugins (MCP, `.mcp.json`), `--image`, saved sessions (`--continue` / `--resume`), auto-verify and `--plan`.

[Full changelog →](https://marketplace.visualstudio.com/items/SUMITKUMARSINGH.free-repo-agent/changelog)

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
Paste a **UI screenshot/mockup** and say *"build this component."* **Zero setup** — the default DeepSeek V4.1 Flash reads images with your existing key. Falls back to OCR for code/error screenshots.

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

### 🧠 Model switcher + thinking mode
Switch models from the footer, Claude-style: **DeepSeek V4.1 Flash / V4 Pro** with **thinking mode** (deep reasoning that works *with* tool calls), or point at **OpenAI / OpenRouter / Gemini** for GPT/Claude/Llama.

</td>
<td width="50%" valign="top">

### ⚡ Effort control
A dial from **fast & cheap → max reasoning**. Higher effort = more tool steps, longer answers, more context, and deeper V4 thinking — you decide speed vs. quality per task.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🧩 Plugins (MCP) — local & remote
One-click tools — **GitHub, web search, Postgres, Playwright, filesystem** & 20+ more — via the **Model Context Protocol**. Install from **npm/GitHub**, a custom command, or a **remote URL**.

</td>
<td width="50%" valign="top">

### ⌨️ Terminal CLI (like Claude Code)
Prefer the shell? Run the **same autonomous agent in your terminal** — live checklist, file edits, command running, approvals — with no VS Code open. Ships with the extension.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 📖 Learn this codebase + 🧠 memory
One click generates a **knowledge brief** of your project (architecture, conventions, key files) that's injected into every prompt — plus a `memory.md` for your own always-on rules.

</td>
<td width="50%" valign="top">

### 👍 Learns from your feedback
Every reply has **Copy · 👍 · 👎**. A 👎 saves *what was wrong* as a rule the agent follows from then on — and offers a one-click **Retry**. Works with **no folder open** too.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 📋 Plan mode
Before a big change, the agent **investigates read-only** and returns what it found, a numbered plan naming every file, and open questions. Nothing changes until you click **▶ Execute plan**.

</td>
<td width="50%" valign="top">

### ↺ Checkpoints & rewind
Every message is a checkpoint. Click **↺ Restore** to put back every file the agent changed since then — files it created are deleted — and rewind the chat to that point.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### ✍️ Inline autocomplete
**Copilot-style grey suggestions** as you type, **Tab** to accept — DeepSeek fill-in-the-middle using the code before *and* after your cursor. Off by default; one click in the status bar.

</td>
<td width="50%" valign="top">

### 💡 Quick Fix, right-click & commits
**✨ Fix with Repo Agent** on any red squiggle, right-click code → **Explain · Fix · Refactor · Tests · Docs**, and an **AI commit message** button in Source Control.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🔎 Precise search + subagents
The agent **greps** exact text, reads the **Problems** panel, uses the language server for **definitions & references**, fetches docs pages, and fans out **parallel research subagents**.

</td>
<td width="50%" valign="top">

### ⧉ Tabs, commands & hooks
Run **several chats side by side**, save prompts as **custom `/commands`**, and run your own scripts before/after tool calls with **hooks**. Reads **`AGENTS.md`**.

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

- **📋 Plan first** — click the **📋 Plan** chip (or type `/plan`): it only reads and investigates, then proposes a plan. **▶ Execute plan** carries it out.
- **↺ Rewind** — hover a message you sent → **↺ Restore** reverts every file the agent changed since then and puts your message back in the input. (Effects of shell commands, like installs, aren't undone.)
- **⧉ Several at once** — **⧉ Tab** opens another independent chat, each with its own terminal.
- **🧠 Long chats keep their memory** — older messages are summarized automatically; `/compact` does it now.

## 🛠️ In your editor & power tools

| | |
|---|---|
| **💡 Quick Fix** | Cursor on a red/yellow squiggle → lightbulb → **✨ Fix with Repo Agent** or **Explain** |
| **Right-click** | Select code → **Repo Agent** → Explain · Find & fix bugs · Refactor · Write tests · Add docs |
| **✨ Commit message** | The sparkle in the Source Control title bar writes it from your staged diff, in your repo's style |
| **✍️ Autocomplete** | Click **Autocomplete** in the status bar → grey suggestions, **Tab** to accept (each pause is a small API call) |
| **@-mentions** | `@file` · `@problems` · `@diff` (uncommitted changes) · `@terminal` · `@https://…` (a web page) |
| **Custom `/commands`** | Save a prompt as `.repo-agent/commands/review-pr.md` (share via git) or `~/.repo-agent/commands/`, then type `/review-pr …`. `$ARGUMENTS` = what you type after it |
| **`AGENTS.md`** | The shared agent-instructions standard (Codex, Cursor, Claude Code) — read into every prompt, alongside `.claude.md` and `memory.md` |

**Hooks** — run your own scripts around the agent's tool calls with `.repo-agent/hooks.json`:

```json
{ "preToolUse": [{ "matcher": "write_file|edit_file", "command": "./scripts/guard-migrations.sh" }] }
```

Each hook gets the event as JSON on stdin; **exit code 2** blocks the call (stderr is told to the agent). Project hooks only run in a trusted workspace, after you approve that exact file.

## ⌨️ Terminal CLI — the agent in your shell

Prefer working in the terminal, like **Claude Code**? The same agent runs as a CLI — **no VS Code needed**. It plans a live checklist, reads and edits files, and runs commands in your current directory, **asking before anything that changes them**.

```
◆ Repo Agent v0.11.0 · deepseek-flash · medium effort

› add a /health route and a test for it

  ▶ Add the /health route
  ○ Add a test
  ○ Run the tests

● Read  src/server.ts
● Edit  src/server.ts
  ✎ Edit src/server.ts
    Approve? [y]es / [n]o / [a]lways:
```

**Setup** — the CLI ships **inside the extension** (v0.10.0 or later), so once Repo Agent is installed just point an alias at it:

```bash
# add to ~/.zshrc (or ~/.bashrc), then restart your terminal
alias repo-agent='node "$(ls -dt ~/.vscode/extensions/sumitkumarsingh.free-repo-agent-*/dist/cli.js | head -1)"'
```

```bash
export DEEPSEEK_API_KEY=sk-...      # or just run it and paste your key when asked

repo-agent                          # interactive session in the current folder
repo-agent "add a /health route"    # run one task, then keep going
```

| | |
|---|---|
| **Options** | `-m, --model <id>` · `-e, --effort low\|medium\|high\|max` · `-C, --cwd <dir>` · `--base-url <url>` (any OpenAI-compatible provider) · `-y, --yes` (auto-approve) · `--login` (re-enter your key) · `--plan` · `-i, --image <file>` · `-c, --continue` · `-r, --resume` · `--no-verify` |
| **In-session** | `/plan` · `/image <file>` · `/resume` · `/mcp` · `/login` · `/model <id>` · `/effort <lvl>` · `/clear` · `/cwd` · `/help` · `/exit` |
| **Plugins** | Add `"mcpServers"` to `~/.repo-agent.json` or a project `.mcp.json` — the same format as Claude Code & Cursor. Project servers are approved once; each plugin call is confirmed |
| **Controls** | Approve each change with `y` / `n` / `a`lways · **Ctrl-C** stops a run, again quits |

> Your key comes from `DEEPSEEK_API_KEY` or `~/.repo-agent.json` (written `chmod 600`, only if you opt in). Pasted the wrong one? `repo-agent --login`.
>
> The CLI keeps its **own** key store — the extension's key lives in VS Code SecretStorage, which a program outside VS Code can't read.

## 🧠 Models & thinking mode — generate the best code

Switch the model from the **🧠 chip in the chat footer** (or the ⚙︎ Options menu), just like Claude:

| Model | Best for |
|---|---|
| **DeepSeek V4.1 Flash** (`deepseek-flash`) | **Newest & the default** — fast, cheap, 1M context, 384K output, and **reads images natively** |
| **DeepSeek V4 Pro** (`deepseek-v4-pro`) | Hardest code & reasoning — top quality (text only) |
| **R1 / V3** (`deepseek-reasoner` / `deepseek-chat`) | Legacy models |

- **Thinking mode** — on the V4 models the agent uses DeepSeek's built-in **deep reasoning that works *with* tool calls**, so it thinks before it edits. It's wired to the **⚡ Effort** dial: off at *Low* (fast/cheap), then *low → high → max* reasoning at *Medium → High → Max*.
- **Not just DeepSeek** — the extension speaks an **OpenAI-compatible API**, so set a custom model id + point `repoAgent.deepseek.baseUrl` at **OpenAI, OpenRouter, Gemini, or any provider** to run the agent on **GPT-4o, Claude, Llama, Qwen** and more.

## 📖 Learn this codebase

Run **Agent: Learn This Codebase** (or `/` → *Learn this codebase*) and it indexes your repo and writes a thorough **knowledge brief** — purpose, stack, architecture, key files, data models, conventions, build/run/test — to `.repo-agent/knowledge.md`. That brief is injected into **every** prompt, so the agent knows your project instantly. Re-run anytime to refresh.

## 👁️ Vision — paste an image, build the component

**Zero setup.** The default model — **DeepSeek V4.1 Flash** — is **natively multimodal**, so it reads images with the DeepSeek key you already have. One model, one key, nothing to configure.

Just **paste a screenshot/mockup** into the chat and ask *"build this as a React component."* The image becomes a precise implementation spec, and the agent builds the files.

```text
/  →  👁️ Vision  →  switch provider (optional):
     • DeepSeek V4.1 Flash — same key, no setup   ← default
     • Google Gemini — FREE (no credit card)
     • Ollama / LM Studio — local, no key
     • OpenRouter (free models) · OpenAI · Custom
```

Vision off, or no key? Images fall back to **OCR** — perfect for screenshots of errors or code.

## 🧩 Plugins (MCP) — give the agent superpowers

Open the **🧩 Plugins** panel (or type <kbd>/</kbd> → **Plugins**) and add tools with one click. Built on the **Model Context Protocol** — the same plugin standard Claude uses — so the entire MCP ecosystem works here. Add from the built-in catalog, **npm/GitHub**, a **custom command**, or a **remote URL**.

📖 **[Full guide: how to use plugins →](docs/PLUGINS.md)**

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

> ➕ **Add any MCP server** — from **npm/GitHub** (paste `@scope/server` or `owner/repo`), a **custom command**, or a **remote URL** (hosted servers over Streamable HTTP, with an optional bearer token). Keys are stored securely in VS Code SecretStorage. **[Full guide → docs/PLUGINS.md](docs/PLUGINS.md)**

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
| `Agent: Learn This Codebase` | Generate a persistent project knowledge brief |
| `Agent: Edit Memory` | Edit the always-on `memory.md` |
| `Agent: Choose Vision Provider` | Pick a vision backend (Gemini free / Ollama / …) |
| `Agent: Reindex Repository` / `Explain Architecture` | Index & architecture tools |
| `Agent: Set / Clear DeepSeek API Key` | Manage your key |
| `Agent: New Chat Tab` | Open another independent chat |
| `Agent: Generate Commit Message` | Commit message from your staged changes (also ✨ in Source Control) |
| `Agent: Toggle Inline Autocomplete` | Grey as-you-type suggestions on/off |
| Right-click → **Repo Agent** → … | Explain / Fix / Refactor / Write tests / Add docs for the selection |

## 🔧 Settings

<details>
<summary>All settings live under <code>repoAgent.*</code> — click to expand</summary>

| Setting | Default | Description |
|---|---|---|
| `deepseek.model` | `deepseek-flash` | Active model (switch it from the 🧠 footer chip) |
| `effort` | `medium` | Speed vs. reasoning depth: low · medium · high · max |
| `deepseek.baseUrl` | `https://api.deepseek.com` | API base URL — point at any OpenAI-compatible provider |
| `deepseek.maxTokens` | `4096` | Max tokens per response (auto-raised for V4) |
| `vision.baseUrl` / `vision.model` | DeepSeek `deepseek-flash` | OpenAI-compatible vision endpoint (reuses your DeepSeek key) |
| `review.guidelinesFile` | `system-design.md` | Your custom review-rules file |
| `review.deepAudit` | `true` | Second audit pass for fewer false positives |
| `indexing.maxFiles` | `1500` | Index size cap |
| `indexing.generateSummaries` | `true` | AI per-file summaries (set `false` for $0 indexing) |
| `retrieval.maxFiles` | `8` | Relevant files injected per prompt |
| `plugins.autoRun` | `false` | Run plugin tools without a confirm prompt (off = you confirm each third-party tool call) |
| `autocomplete.enabled` | `false` | Inline autocomplete — each typing pause is a small API call |
| `autocomplete.delayMs` | `350` | Typing pause before a suggestion is requested |
| `review.autoOnSave` | `false` | Auto-review files on save |

</details>

## 🔒 Privacy & security

- **Your keys stay secret.** DeepSeek/vision keys and any plugin or remote‑MCP tokens live in VS Code **SecretStorage** — never in your code, settings, or the extension's storage, and never logged.
- **No telemetry.** Zero analytics/tracking. The only network calls go to endpoints **you** configure — your AI provider, your vision provider, and any MCP servers you add. Your code/context is sent to *your* AI provider only when you make a request.
- **The agent stays in your project.** File edits are blocked from absolute paths and `..` traversal; commands run in a **visible terminal with your approval**; edits show inline with **Keep / Undo**.
- **Plugins run third‑party code** — add only servers you trust. Plugin tools **ask before running** by default (`plugins.autoRun` is off); enable it only for trusted plugins.
- **Sensitive generated files?** `memory.md` and `.repo-agent/knowledge.md` are injected into prompts and committed by default — add them to `.gitignore` if private:
  ```gitignore
  .agent-cache/
  .repo-agent/
  memory.md
  ```

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
<details><summary><b>Does it have inline autocomplete like Copilot?</b></summary><br/>Yes — since 0.12. Grey suggestions appear as you pause typing and <b>Tab</b> accepts them, using DeepSeek's fill-in-the-middle model with the code before and after your cursor. It's off by default (each pause is a small API call); click <b>Autocomplete</b> in the status bar to turn it on.</details>
<details><summary><b>Can I undo what the agent did?</b></summary><br/>Yes. Each edit shows inline with <b>Keep / Undo</b>, and every message is a checkpoint: click <b>↺ Restore</b> on it to revert all files the agent changed since then and rewind the chat. You can also use <b>📋 Plan mode</b> to review a plan before anything changes.</details>
<details><summary><b>Is it a good Copilot / Cursor / Claude / Cline alternative?</b></summary><br/>Yes — repo-aware chat, an autonomous agent that edits files and runs commands, visible reasoning, vision, MCP plugins, and pre-commit code review — the same core workflow, no subscription.</details>
<details><summary><b>Is there a free DeepSeek extension / DeepSeek agent for VS Code?</b></summary><br/>Yes — this is one. It's a full <b>DeepSeek coding agent</b> (not just chat): it edits files, runs commands, reads screenshots and reviews code, using your own DeepSeek API key.</details>
<details><summary><b>How do I use DeepSeek V4.1 Flash in VS Code?</b></summary><br/>Install Free Repo Agent and run <b>Agent: Set DeepSeek API Key</b> — <b>DeepSeek V4.1 Flash (<code>deepseek-flash</code>) is the default</b>. Switch to <b>V4 Pro</b> from the 🧠 footer chip. Thinking mode is built in and follows the ⚡ Effort dial.</details>
<details><summary><b>Is there a free Claude Code alternative that runs in the terminal?</b></summary><br/>Yes — the <b>terminal CLI</b> (<code>repo-agent</code>) runs the same autonomous agent in your shell: live checklist, file edits, commands, with approval before every change. See <a href="#️-terminal-cli--the-agent-in-your-shell">Terminal CLI</a>. It doubles as a lightweight <b>Aider alternative</b>.</details>
<details><summary><b>Is it a Roo Code / Kilo Code / Cline alternative?</b></summary><br/>Yes — like them it's an in-editor agent that reads your repo, edits multiple files and runs commands, bring-your-own-key with no subscription, plus a live checklist, auto-verify/self-fix and a staff-engineer code reviewer.</details>
<details><summary><b>Can I use it in Cursor, Windsurf or VSCodium?</b></summary><br/>It's published on <b><a href="https://open-vsx.org/extension/SUMITKUMARSINGH/free-repo-agent">Open VSX</a></b>, the registry Cursor, Windsurf and VSCodium install from — search <i>“Free Repo Agent”</i> in their Extensions view.</details>
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

<sub>Free DeepSeek AI coding agent · free AI autocomplete · Copilot autocomplete alternative · AI plan mode · AI coding checkpoints · AI commit message generator · AGENTS.md · DeepSeek extension for VS Code · DeepSeek agent · DeepSeek V4.1 Flash · DeepSeek V4 Pro · DeepSeek in Cursor · Open VSX AI agent · Claude Code alternative · Roo Code alternative · Kilo Code alternative · terminal AI coding agent · Free AI coding agent · AI coding assistant · AI agent for VS Code · agentic coding · vibe coding · GitHub Copilot alternative · free Copilot · Copilot Chat alternative · Cursor alternative · Claude alternative · Claude Code alternative · Codex alternative · Cline / Continue / Codeium / Windsurf / Tabnine / Cody / Aider / Roo Code / Kilo Code alternative · ChatGPT for VS Code · DeepSeek VS Code extension · DeepSeek Coder · DeepSeek V4 · DeepSeek V4 Pro · DeepSeek V4 Flash · thinking mode · reasoning model · AI model switcher · switch AI model · OpenRouter · GPT-4o · use Claude in VS Code · MCP · Model Context Protocol · MCP client · remote MCP server · MCP plugins · AI code review · AI code reviewer · custom review rules · vision AI coding · screenshot to code · image to code · UI to code · AI pair programming · agent mode · autonomous coding agent · self-verifying AI agent · learn codebase · project memory · repo indexing · AI refactoring · AI code generation · repo-aware AI assistant · bring your own key AI.</sub>

</div>
