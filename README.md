<div align="center">

<img src="https://raw.githubusercontent.com/sumitsingh4411/repo-agent/main/media/icon.png" width="112" alt="Free Repo Agent — free AI coding agent for VS Code" />

<h1>Free Repo Agent</h1>

<h3>Free AI Coding Agent &amp; GitHub Copilot · Cursor · Claude Alternative for VS Code</h3>

<p><b>Repo-aware chat</b> · <b>autonomous multi-file edits</b> · <b>terminal commands</b> · <b>vision (screenshot → code)</b> · <b>MCP plugins</b> · <b>staff-engineer code review</b> — powered by <b>DeepSeek</b>, with <b>no subscription</b>.</p>

[![VS Code Marketplace Version](https://img.shields.io/visual-studio-marketplace/v/SUMITKUMARSINGH.free-repo-agent?label=Marketplace&color=0b6cff&logo=visualstudiocode)](https://marketplace.visualstudio.com/items?itemName=SUMITKUMARSINGH.free-repo-agent)
[![Installs](https://img.shields.io/visual-studio-marketplace/i/SUMITKUMARSINGH.free-repo-agent?color=0b6cff&label=installs)](https://marketplace.visualstudio.com/items?itemName=SUMITKUMARSINGH.free-repo-agent)
[![Rating](https://img.shields.io/visual-studio-marketplace/r/SUMITKUMARSINGH.free-repo-agent?color=ffb020)](https://marketplace.visualstudio.com/items?itemName=SUMITKUMARSINGH.free-repo-agent&ssr=false#review-details)
[![Price: Free](https://img.shields.io/badge/price-free-2ea44f)](https://marketplace.visualstudio.com/items?itemName=SUMITKUMARSINGH.free-repo-agent)
[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

<p>
<a href="https://marketplace.visualstudio.com/items?itemName=SUMITKUMARSINGH.free-repo-agent"><b>⬇️ Install</b></a> &nbsp;·&nbsp;
<a href="#-features"><b>✨ Features</b></a> &nbsp;·&nbsp;
<a href="#-getting-started"><b>🚀 Get started</b></a> &nbsp;·&nbsp;
<a href="https://github.com/sumitsingh4411/repo-agent/issues/new"><b>🐞 Report a bug</b></a>
</p>

</div>

> **A free AI coding agent and a free GitHub Copilot, Cursor & Claude alternative for VS Code** — repository-aware chat, autonomous code editing, terminal command running, vision (screenshot → component), and pre-commit code review, powered by **DeepSeek**.

**Free Repo Agent** is a free, open AI coding assistant that brings a Claude/Cursor/Cline-style **agent** experience into VS Code. It understands your whole repository, **writes and edits code** with inline **Keep / Undo** review, **runs terminal commands** with your approval, **auto-verifies its own work** (runs your typecheck/build and fixes errors before finishing), tracks progress on a **live Claude-style task checklist**, extends itself with **plugins (MCP)** — GitHub, web search, Postgres, filesystem and more — shows its **thinking**, supports **`@` file mentions**, **vision (paste a screenshot/UI → build the component)**, **image OCR** and **PDF uploads**, keeps **chat history/sessions**, and runs a **staff-engineer-grade pre-commit code review** of your staged git changes — all on the affordable DeepSeek API.

Looking for a **free Copilot alternative**, **free Cursor alternative**, **Cline / Continue alternative**, or a **free Claude / ChatGPT coding agent**? This is a lightweight, bring-your-own-key option with no subscription.

## 🐞 Report a bug / request a feature

Hit a bug or have an idea? **[Open an issue →](https://github.com/sumitsingh4411/repo-agent/issues/new)**

To help us fix it fast, please include:
- Your **VS Code version** and **extension version** (e.g. 0.7.15)
- **Steps to reproduce** and what you expected vs. what happened
- Any error text from **View → Output → "Repo Agent"**

Browse or search existing reports on the **[Issues page](https://github.com/sumitsingh4411/repo-agent/issues)**.

---

## 🚀 Getting started

### 1. Get a DeepSeek API key

Repo Agent needs a DeepSeek API key to talk to the model.

1. Go to **https://platform.deepseek.com/api_keys**
2. Sign in (or create a free account).
3. Click **Create new API key**, give it a name, and **copy** the key (starts with `sk-…`). You won’t be able to see it again, so save it somewhere safe.
4. DeepSeek is **pay-as-you-go** and very low cost — add a small amount of credit under **Billing** on the same dashboard. A few dollars goes a long way.

> 💡 Models: `deepseek-chat` (fast, general) and `deepseek-reasoner` (shows reasoning / “thinking”). You can switch in settings.

### 2. Add your key to VS Code

Open the Command Palette (`Cmd/Ctrl+Shift+P`) and run:

```
Agent: Set DeepSeek API Key
```

Paste your key and press Enter. It’s stored securely in VS Code **SecretStorage** — never written to your code or settings.

> Alternative: set the `DEEPSEEK_API_KEY` environment variable before launching VS Code.

### 3. Start using it

Open the chat any of these ways:

- Click the **Repo Agent `</>` icon in the top-right** of the editor toolbar (when a file is open) — this opens chat **beside your code**, on the right, like Cursor/Claude.
- Press **`Cmd/Ctrl+Shift+A`**.
- Click the **Repo Agent icon** in the Activity Bar (left sidebar).

The status bar shows when indexing is done and the key is set.

> 💡 **Prefer it docked on the right?** Show the Secondary Side Bar (`Cmd/Ctrl+Alt+B`), then **drag the Repo Agent icon** from the left Activity Bar into the right side bar. VS Code remembers the position.

---

## ✨ Features

| | Feature | What it does |
|---|---|---|
| 💬 | **Repo-aware chat** | Ask anything about your codebase. It indexes your project and injects the most relevant files into every answer. |
| ✍️ | **Code generation** | Describe what you want; it generates files that match your architecture, with a diff preview before writing. |
| 🤖 | **Autonomous agent** | Give it a task — it reads files, edits code, and runs commands step-by-step. Every change is reviewed **inline** with **Keep / Undo**. |
| ✅ | **Auto-verify & self-fix** | After editing, it automatically runs your project's typecheck/build, reads the errors, and **fixes them before finishing** — no more "done" on code that doesn't compile. |
| ☑️ | **Live task checklist** | A Claude-style checklist that ticks each step from pending → in-progress → ✓ done as the agent works, so you always see what it's doing now. |
| 🔍 | **Staff-engineer code review** | Reviews staged changes / current file / branch — reading the **full files**, then doing a **second audit pass** to drop false positives — and reports **Critical · Quality · Architecture · Testing** findings in the Problems panel and a sidebar. Add a **`system-design.md`** with your own rules and it enforces them too. |
| 🧩 | **Plugins (MCP)** | Add tools the agent can use — GitHub, web search, Postgres, filesystem, Puppeteer and more — one click from the **🧩 Plugins** panel. Backed by the **Model Context Protocol** (the same plugin system Claude uses); add any custom MCP server too. |
| 🧠 | **Visible thinking** | With the reasoning model, it streams its chain-of-thought in a collapsible **Thinking** block, like Claude. |
| 👁️ | **Vision (image → code)** | Flip the **👁️ Vision** toggle, paste or attach a UI screenshot/mockup, and ask it to build the component. A vision model turns the image into a precise spec, then the agent builds it. **Free by default** (Google Gemini free tier; or local Ollama, no key); falls back to OCR when off. |
| 📎 | **@ mentions & uploads** | Type `@` to reference any file, or attach files and **PDFs** (text is extracted automatically). |
| ⏹ | **Full control** | Inline command approval, a **Stop** button to interrupt, and per-change Keep/Undo or Keep-all/Undo-all. |

---

## 🧑‍💻 How to use

### Chat & generate
Type a question and **Send**. Toggle **Generate code** to produce files (you’ll get an **Apply** button with a diff preview before anything is written). Keep **Think** on to see the model reason through the answer.

- **`@` to reference files:** type `@` and pick a file from the dropdown — its contents are added to the context.
- **📎 to attach:** click the paperclip to attach text files or **PDFs**.

### Agent mode (autonomous)
Check **Agent (run & edit)** and describe a task, e.g.:

> _“Add a `/health` route and a test for it, then run the tests.”_

The agent will:
1. Read relevant files, then propose edits — each shows **inline in the file** with green highlights and **✓ Keep / ✗ Undo** buttons.
2. Ask to **Run** any terminal command (inline, in the chat) — commands run in a visible **Repo Agent** terminal.
3. When done, you get **Keep all / Undo all** to accept or revert the whole batch.

Use the **Stop** button anytime to interrupt.

### Code review
Stage some changes (`git add …`), then run **Agent: Review Staged Changes** (also available from the Source Control title bar). Findings appear in the **Problems** panel, the **Review Results** sidebar, and inline — each with **Fix with AI**, **Ignore**, and **Commit Anyway**.

You can also review the **current file** or have it run automatically on save (see settings).

**Custom review rules.** Want the reviewer to enforce *your* team's standards? Run **Agent: Create Review Guidelines** (or click the link in the empty Review Results panel) to scaffold a `system-design.md` at your repo root. Fill it with your intended system design and concrete rules — naming, error handling, "no `console.log`", required tests, layering, no secrets, etc. The reviewer reads it before every review and flags any change that breaks a rule, quoting it. Configure the filename with `repoAgent.review.guidelinesFile`; remove the file to fall back to the default rubric.

### Vision — paste an image, build the component (free)
DeepSeek is text-only, so image *understanding* uses a separate vision model — but it's **free by default**: it uses **Google Gemini's free tier** (no credit card). One‑time setup:

1. Click the **👁️ Vision** button in the chat footer (or run **Agent: Choose Vision Provider**) and pick a backend:
   - **Google Gemini — free** (default, recommended): it opens the free‑key page; paste the key.
   - **Ollama / LM Studio — local, no key**: 100% free & private (needs a local vision model like `llava`).
   - **OpenRouter (free models)**, **OpenAI (paid)**, or **Custom**.
2. With Vision on, **paste** a screenshot/mockup into the input (or attach with **+**), type e.g. *"build this as a React component"*, and send.

Behind the scenes the vision model turns the image into a precise implementation spec, then the agent builds the files from it. With Vision **off** (or no key set), attached images fall back to **OCR** — great for screenshots of code or error messages, and needs no key at all.

### Project conventions
Drop a `.agent.md` or `.claude.md` file in your repo root with conventions, architecture notes, or rules — Repo Agent reads it and follows it. For **code review specifically**, add a `system-design.md` with rules the reviewer must enforce (see *Custom review rules* above).

---

## ⚙️ Commands

Open the Command Palette and type **“Agent:”** to see all of them:

| Command | Description |
|---|---|
| `Agent: Chat` | Open the chat panel |
| `Agent: Generate Code` | Describe code to generate |
| `Agent: Run Agent (autonomous)` | Run a task that can edit files & run commands |
| `Agent: Review Staged Changes` | Pre-commit review of staged diff |
| `Agent: Review Current File` | Review the active file |
| `Agent: Create Review Guidelines` | Scaffold a `system-design.md` of project review rules |
| `Agent: Choose Vision Provider` | Pick a vision backend (Gemini free / Ollama / OpenRouter / OpenAI) for reading images |
| `Agent: Reindex Repository` | Rebuild the code index |
| `Agent: Explain Architecture` | Generate an architecture overview |
| `Agent: Set DeepSeek API Key` / `Clear DeepSeek API Key` | Manage your key |

---

## 🔧 Settings

All under `repoAgent.*` (Settings → search “Repo Agent”):

| Setting | Default | Description |
|---|---|---|
| `deepseek.model` | `deepseek-chat` | Model for generation & review |
| `deepseek.reasoningModel` | `deepseek-reasoner` | Model used when **Think** is on |
| `deepseek.showThinking` | `true` | Show reasoning by default |
| `deepseek.baseUrl` | `https://api.deepseek.com` | API base URL (OpenAI-compatible) |
| `deepseek.temperature` | `0.2` | Sampling temperature |
| `deepseek.maxTokens` | `4096` | Max tokens per response |
| `indexing.include` / `exclude` | _globs_ | Which files to index |
| `indexing.maxFiles` | `1500` | Index size cap |
| `indexing.generateSummaries` | `true` | AI per-file summaries (set `false` for zero API cost indexing) |
| `retrieval.maxFiles` | `8` | Relevant files injected per prompt |
| `review.autoOnSave` | `false` | Auto-review files on save |

---

## 🔒 Privacy

- Your code is only sent to **DeepSeek’s API** when you make a request (chat, generate, review, or run the agent), using the base URL you configure.
- Your API key lives in VS Code **SecretStorage**, never in your repo.
- The local index is cached under `.agent-cache/` (add it to `.gitignore`).
- Review the [DeepSeek privacy policy](https://platform.deepseek.com) for how the API handles data.

---

## ❓ Troubleshooting

- **“Set your DeepSeek API key first.”** Run **Agent: Set DeepSeek API Key** (see [step 3](#3-add-your-key-to-vs-code)).
- **`401 Unauthorized`** Your key is wrong/revoked, or you’re out of credit — check https://platform.deepseek.com/api_keys and **Billing**.
- **Agent says a command’s output “could not be captured.”** That’s VS Code shell integration not being active — the command still ran in the terminal. It’s on by default for zsh/bash/pwsh in recent VS Code.
- **No reasoning shown.** “Thinking” requires `deepseek-reasoner`; it doesn’t apply to autonomous Agent mode (which uses tools).

---

## 🆚 A free alternative to GitHub Copilot, Cursor & Claude

Free Repo Agent gives you the agentic coding workflow people love in **GitHub Copilot Chat**, **Cursor**, **Cline**, **Codex**, and **Claude** — autonomous multi-file edits, terminal commands, codebase-aware answers, a live task checklist, self-verifying edits, MCP plugins, and inline diff review — **without a monthly subscription**. You bring your own **DeepSeek API key** (pay-as-you-go, typically a few cents of usage), and everything runs inside VS Code. It’s ideal if you want a **free AI pair programmer**, a **free Copilot alternative**, or a **cheaper Cursor / Claude alternative** for everyday coding and code review. If you’ve looked at **Cline**, **Continue**, **Codeium**, **Windsurf**, **Tabnine**, **Cody**, **Aider**, or **Roo Code** and want a simple, bring-your-own-key agent that edits code, self-verifies, and reviews diffs inside VS Code, Free Repo Agent is a lightweight alternative to all of them.

## ❓ FAQ

**Is Free Repo Agent really free?**
Yes — the extension is free and open. You only pay DeepSeek’s low pay-as-you-go API usage (you bring your own key).

**Is it a good GitHub Copilot / Cursor / Claude alternative?**
Yes. You get repo-aware chat, an autonomous coding agent that edits files and runs commands, visible reasoning, and pre-commit code review — the same core workflow, with no subscription.

**Is it a free Cline / Continue / Aider alternative?**
Yes. Like Cline and Continue, it's an in-editor agent that reads your repo, edits multiple files, and runs commands — bring-your-own-key with DeepSeek, so there's no subscription. It adds a live task checklist, auto-verify/self-fix, and a staff-engineer code reviewer on top.

**Does it fix its own mistakes?**
Yes — after editing it automatically runs your project's typecheck/build, reads the errors, and fixes them before finishing, so you don't get code that fails to compile.

**Can I add plugins / MCP servers?**
Yes. Open the **🧩 Plugins** panel in chat and add tools the agent can use — GitHub, web search, Postgres, filesystem, Puppeteer and more — with one click, or add any custom MCP server. Plugins use the **Model Context Protocol** (the same plugin system Claude uses), so the huge MCP ecosystem works here. (Requires Node/npx on your PATH.)

**Do I need an API key?**
Yes — a DeepSeek API key from <https://platform.deepseek.com/api_keys>. Set it via **Agent: Set DeepSeek API Key**. It’s stored securely in VS Code SecretStorage.

**Which models does it use?**
`deepseek-chat` for fast coding and `deepseek-reasoner` for visible step-by-step “thinking”.

**Can it edit my code and run commands automatically?**
It proposes edits inline with **Keep / Undo** and asks before running any terminal command — you stay in control.

**Does it work like an AI code reviewer?**
Yes — it reviews your **staged git changes** and reports Critical / Quality / Architecture / Testing findings, like a senior engineer. You can also give it **custom review rules** in a `system-design.md` file and it enforces your project's standards on every review.

**Does my code leave my machine?**
Only the context needed for a request is sent to the DeepSeek API when you ask. Your key never leaves SecretStorage. See **Privacy** above.

---

## License

MIT — see the bundled `LICENSE` file.

---

<sub>Keywords: free AI coding agent, AI coding assistant, GitHub Copilot alternative, free Copilot, Cursor alternative, Claude alternative, Codex alternative, OpenAI Codex alternative, Cline alternative, Continue alternative, Codeium alternative, Windsurf alternative, Tabnine alternative, Cody alternative, Aider alternative, Roo Code alternative, ChatGPT for VS Code, DeepSeek VS Code extension, DeepSeek Coder, MCP, Model Context Protocol, MCP client for VS Code, MCP plugins, AI code review, AI code reviewer, custom code review rules, project review guidelines, vision AI coding, screenshot to code, image to code, UI to code, AI pair programming, agent mode, autonomous coding agent, self-verifying AI agent, AI refactoring, AI code generation, repo-aware AI assistant, bring your own key AI.</sub>
