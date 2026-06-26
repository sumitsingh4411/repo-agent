<div align="center">

<img src="https://raw.githubusercontent.com/sumitsingh4411/repo-agent/main/media/icon.png" width="120" alt="Free Repo Agent logo" />

# Free Repo Agent

### The free AI coding agent for VS Code

A no-subscription **GitHub Copilot · Cursor · Claude alternative** — repo-aware chat, an autonomous agent that **edits files & runs commands**, **vision (screenshot → component)**, **MCP plugins**, and **staff-engineer code review**. Powered by **DeepSeek** (bring your own key, pay-as-you-go).

<br/>

[![VS Code Marketplace](https://img.shields.io/visual-studio-marketplace/v/SUMITKUMARSINGH.free-repo-agent?label=Marketplace&color=0b6cff&logo=visualstudiocode)](https://marketplace.visualstudio.com/items?itemName=SUMITKUMARSINGH.free-repo-agent)
[![Installs](https://img.shields.io/visual-studio-marketplace/i/SUMITKUMARSINGH.free-repo-agent?color=0b6cff&label=installs)](https://marketplace.visualstudio.com/items?itemName=SUMITKUMARSINGH.free-repo-agent)
[![Rating](https://img.shields.io/visual-studio-marketplace/r/SUMITKUMARSINGH.free-repo-agent?color=ffb020)](https://marketplace.visualstudio.com/items?itemName=SUMITKUMARSINGH.free-repo-agent&ssr=false#review-details)
[![Price: Free](https://img.shields.io/badge/price-free-2ea44f)](https://marketplace.visualstudio.com/items?itemName=SUMITKUMARSINGH.free-repo-agent)
[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

**[⬇️ Install](https://marketplace.visualstudio.com/items?itemName=SUMITKUMARSINGH.free-repo-agent) · [🚀 Get started](#-getting-started) · [✨ Features](#-features) · [🐞 Report a bug](https://github.com/sumitsingh4411/repo-agent/issues/new)**

</div>

---

**Free Repo Agent** brings a Claude/Cursor/Cline-style **agent** into VS Code. It understands your whole repository, writes and edits code with inline **Keep / Undo**, runs terminal commands with your approval, **verifies its own work** (typecheck/build, then fixes errors), reads **images** (paste a UI → build the component), extends itself with **MCP plugins**, and runs a **staff-engineer pre-commit code review** — all on the affordable DeepSeek API, with **no monthly subscription**.

## Contents

- [Features](#-features)
- [Getting started](#-getting-started)
- [How to use](#-how-to-use)
- [Commands](#%EF%B8%8F-commands)
- [Settings](#-settings)
- [Privacy](#-privacy)
- [Troubleshooting](#-troubleshooting)
- [vs. Copilot, Cursor & Claude](#-vs-copilot-cursor--claude)
- [FAQ](#-faq)
- [Report a bug](#-report-a-bug--request-a-feature)

## ✨ Features

| | Feature | What it does |
|---|---|---|
| 💬 | **Repo-aware chat** | Ask anything about your codebase — it indexes your project and injects the most relevant files into every answer. |
| ✍️ | **Code generation** | Describe what you want; it generates files that match your architecture, with a diff preview before writing. |
| 🤖 | **Autonomous agent** | Give it a task — it reads files, edits code, and runs commands step-by-step. Every change is reviewed **inline** with **Keep / Undo**. |
| ✅ | **Auto-verify & self-fix** | After editing, it runs your typecheck/build, reads the errors, and **fixes them before finishing** — no "done" on code that doesn't compile. |
| ☑️ | **Live task checklist** | A Claude-style checklist that ticks each step pending → in-progress → ✓ done as the agent works. |
| 🔍 | **Staff-engineer code review** | Reviews staged changes / current file / branch — reads the **full files**, runs a **second audit pass** to drop false positives, reports **Critical · Quality · Architecture · Testing**. Add a `system-design.md` with your own rules and it enforces them. |
| 🧩 | **Plugins (MCP)** | One-click tools the agent can use — GitHub, web search, Postgres, Playwright, filesystem and more — via the **Model Context Protocol**. Add any custom MCP server too. |
| 👁️ | **Vision (image → code)** | Paste a UI screenshot/mockup and ask it to build the component. **Free by default** (Google Gemini free tier, or local Ollama — no key); falls back to OCR. |
| 🧠 | **Project memory** | A `memory.md` injected into every prompt so the agent remembers your stack, conventions, and rules. |
| 📎 | **@ mentions & uploads** | Reference any file with `@`, or attach files and **PDFs** (text extracted automatically). |

## 🚀 Getting started

### 1. Get a DeepSeek API key

1. Go to **https://platform.deepseek.com/api_keys** and sign in (free account).
2. Click **Create new API key** and **copy** it (starts with `sk-…`).
3. DeepSeek is **pay-as-you-go** and very cheap — add a few dollars of credit under **Billing**.

### 2. Add your key to VS Code

Open the Command Palette (`Cmd/Ctrl+Shift+P`) and run **`Agent: Set DeepSeek API Key`**. It's stored securely in VS Code **SecretStorage** — never written to your code or settings.

> Alternative: set the `DEEPSEEK_API_KEY` environment variable before launching VS Code.

### 3. Start using it

- Press **`Cmd/Ctrl+Shift+A`**, or
- Click the **Repo Agent `</>` icon** in the editor's top-right to open chat **beside your code**, or
- Click the **Repo Agent icon** in the Activity Bar.

## 🧑‍💻 How to use

<details open>
<summary><b>Chat & generate</b></summary>

Type a question and **Send**. Toggle **Generate code** to produce files (you get an **Apply** button with a diff preview first). Keep **Think** on to watch the model reason. Type `@` to reference a file; click **+** to attach text files or **PDFs**.
</details>

<details>
<summary><b>Agent mode (autonomous)</b></summary>

Describe a task, e.g. *"Add a `/health` route and a test, then run the tests."* The agent:
1. Reads relevant files and proposes edits — each shows **inline** with **✓ Keep / ✗ Undo**.
2. Asks to **Run** any terminal command (in a visible Repo Agent terminal).
3. Ends with **Keep all / Undo all**. Hit **Stop** anytime.
</details>

<details>
<summary><b>Code review (with your own rules)</b></summary>

Stage changes (`git add …`), then run **Agent: Review Staged Changes** (also in the Source Control title bar). Findings land in the **Problems** panel, the **Review Results** sidebar, and inline — each with **Fix with AI**, **Ignore**, **Commit Anyway**. Run **Agent: Create Review Guidelines** to scaffold a `system-design.md` of your team's rules that the reviewer enforces every time.
</details>

<details>
<summary><b>Vision — paste an image, build the component (free)</b></summary>

DeepSeek is text-only, so image understanding uses a separate vision model — **free by default** via **Google Gemini's free tier** (no credit card). Click the **👁️ Vision** entry (`/` menu) → choose **Gemini (free)**, **Ollama (local, no key)**, **OpenRouter**, **OpenAI**, or **Custom** → paste a screenshot and ask *"build this as a React component."* Off (or no key) → images fall back to OCR.
</details>

<details>
<summary><b>Project memory & conventions</b></summary>

Type `/` → **Memory** to create a `memory.md` whose contents are injected into **every** prompt (stack, conventions, "always/never" rules). You can also drop a `.agent.md` or `.claude.md` in your repo root — Repo Agent reads and follows it.
</details>

## ⚙️ Commands

Open the Command Palette and type **"Agent:"**.

| Command | Description |
|---|---|
| `Agent: Chat` / `Open Chat (beside editor)` | Open the chat panel |
| `Agent: Generate Code` | Describe code to generate |
| `Agent: Run Agent (autonomous)` | Run a task that can edit files & run commands |
| `Agent: Review Staged Changes` / `Review Current File` | Pre-commit / file review |
| `Agent: Create Review Guidelines` | Scaffold a `system-design.md` of review rules |
| `Agent: Edit Memory` | Edit the always-on `memory.md` |
| `Agent: Choose Vision Provider` | Pick a vision backend (Gemini free / Ollama / …) |
| `Agent: Reindex Repository` / `Explain Architecture` | Index & architecture tools |
| `Agent: Set / Clear DeepSeek API Key` | Manage your key |

## 🔧 Settings

<details>
<summary>All settings live under <code>repoAgent.*</code> (Settings → "Repo Agent")</summary>

| Setting | Default | Description |
|---|---|---|
| `deepseek.model` | `deepseek-chat` | Model for generation & review |
| `deepseek.reasoningModel` | `deepseek-reasoner` | Model used when **Think** is on |
| `deepseek.showThinking` | `true` | Show reasoning by default |
| `deepseek.baseUrl` | `https://api.deepseek.com` | API base URL (OpenAI-compatible) |
| `deepseek.maxTokens` | `4096` | Max tokens per response |
| `vision.baseUrl` / `vision.model` | Gemini free | OpenAI-compatible vision endpoint |
| `review.guidelinesFile` | `system-design.md` | Your custom review rules file |
| `indexing.maxFiles` | `1500` | Index size cap |
| `retrieval.maxFiles` | `8` | Relevant files injected per prompt |
| `review.autoOnSave` | `false` | Auto-review files on save |

</details>

## 🔒 Privacy

- Your code is sent to **DeepSeek's API** only when you make a request, using the base URL you configure.
- Your API key lives in VS Code **SecretStorage**, never in your repo.
- The local index is cached under `.agent-cache/` (add it to `.gitignore`).

## ❓ Troubleshooting

<details>
<summary>Common issues</summary>

- **"Set your DeepSeek API key first."** → run **Agent: Set DeepSeek API Key**.
- **`401 Unauthorized`** → key wrong/revoked or out of credit; check the DeepSeek dashboard + Billing.
- **Vision failed** → open **View → Output → "Repo Agent"** for the real reason (bad key / wrong model / quota), then `/` → **Vision API key** to re-add it.
- **No reasoning shown** → "Thinking" needs `deepseek-reasoner`; it doesn't apply to autonomous Agent mode.
</details>

## 🆚 vs. Copilot, Cursor & Claude

| | Free Repo Agent | Copilot | Cursor | Claude / Cline |
|---|:---:|:---:|:---:|:---:|
| Price | **Free** (BYO key) | Subscription | Subscription | Subscription / BYO |
| Repo-aware agent (multi-file edits) | ✅ | ✅ | ✅ | ✅ |
| Runs terminal commands | ✅ | ✅ | ✅ | ✅ |
| Self-verifies (build/typecheck) | ✅ | — | partial | — |
| Vision: screenshot → code | ✅ (free) | — | ✅ | ✅ |
| MCP plugins | ✅ | — | ✅ | ✅ |
| Pre-commit code review + custom rules | ✅ | partial | — | — |

A free alternative to **GitHub Copilot, Cursor, Claude, Codex, Cline, Continue, Codeium, Windsurf, Tabnine, Cody, Aider & Roo Code** — a lightweight, bring-your-own-key agent that edits code, self-verifies, and reviews diffs inside VS Code.

## ❓ FAQ

<details>
<summary><b>Is it really free?</b></summary>

Yes — the extension is free and open. You only pay DeepSeek's low pay-as-you-go API usage (your own key).
</details>

<details>
<summary><b>Is it a good Copilot / Cursor / Claude / Cline alternative?</b></summary>

Yes — repo-aware chat, an autonomous agent that edits files and runs commands, visible reasoning, vision, MCP plugins, and pre-commit code review — the same core workflow, no subscription.
</details>

<details>
<summary><b>Does it fix its own mistakes?</b></summary>

Yes — after editing it runs your typecheck/build, reads the errors, and fixes them before finishing.
</details>

<details>
<summary><b>Can I add plugins / MCP servers?</b></summary>

Yes — open the **🧩 Plugins** panel and add GitHub, web search, Postgres, Playwright, and more with one click, or any custom MCP server (needs Node/npx).
</details>

<details>
<summary><b>Does my code leave my machine?</b></summary>

Only the context needed for a request is sent to the DeepSeek API when you ask. Your key never leaves SecretStorage.
</details>

## 🐞 Report a bug / request a feature

Found a bug or have an idea? **[Open an issue →](https://github.com/sumitsingh4411/repo-agent/issues/new)** — you'll get a quick form for a **bug report** or **feature request**. Please include your extension version, VS Code version, steps to reproduce, and any error from **View → Output → "Repo Agent"**.

Browse existing reports on the **[Issues page](https://github.com/sumitsingh4411/repo-agent/issues)**.

## License

MIT.

---

<sub>Free AI coding agent · AI coding assistant · GitHub Copilot alternative · free Copilot · Cursor alternative · Claude alternative · Codex alternative · Cline / Continue / Codeium / Windsurf / Tabnine / Cody / Aider / Roo Code alternative · ChatGPT for VS Code · DeepSeek VS Code extension · DeepSeek Coder · MCP · Model Context Protocol · MCP client · AI code review · AI code reviewer · custom review rules · vision AI coding · screenshot to code · image to code · UI to code · AI pair programming · agent mode · autonomous coding agent · self-verifying AI agent · AI refactoring · AI code generation · repo-aware AI assistant · bring your own key AI.</sub>
