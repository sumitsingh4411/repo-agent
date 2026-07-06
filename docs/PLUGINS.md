# 🧩 Plugins (MCP servers) — how to use

Plugins give the agent **extra tools** — GitHub, web search, databases, a browser, your design files, and hundreds more. They're **MCP servers** (Model Context Protocol — the same plugin standard Claude uses), so the whole MCP ecosystem works here.

Once a plugin is connected, you don't do anything special: just chat, and the agent uses its tools automatically (e.g. *"search the web for…"*, *"query the users table"*, *"open this URL and summarise it"*).

---

## Requirements

- **Local plugins** (the common kind) run via **`npx`**, so you need **Node.js** installed (which includes `npx`). Check with `node -v` in a terminal.
- **Remote plugins** just need a **URL** — no Node required.

---

## Open the Plugins panel

- Click **🧩 Plugins** in the chat's top bar, **or**
- Type **`/`** in the chat and pick **Plugins**.

At the top there's a **🔎 search box** (filter the list) and a **"Browse more →"** link to the full MCP registry.

---

## Four ways to add a plugin

### 1. From the catalog (one‑click) — easiest
The panel ships with 20 popular servers (GitHub, GitLab, Postgres, SQLite, Playwright, Brave/Tavily/Exa search, Firecrawl, Filesystem, Memory, Notion, Figma, and more).

1. Find it in the list (or search).
2. Click **Add**.
3. If it needs a key/token, a small form appears — fill it in and click **Connect**.

### 2. From npm or GitHub
For any published MCP server not in the catalog.

- Under **"➕ Install from npm or GitHub"**, paste one of:
  - an npm package: `mcp-server-foo` or `@scope/server`
  - a GitHub repo: `owner/repo` or `https://github.com/owner/repo`
- Click **Install**. It runs via `npx` under the hood.

### 3. Custom command
For a local script or any binary that speaks MCP over stdio.

- Under **"+ Add custom plugin (command)"**, enter the full command, e.g.:
  - `npx -y @modelcontextprotocol/server-github`
  - `python /path/to/my_server.py`
  - `node ./my-mcp-server.js`
- Click **Connect**.

### 4. Remote MCP server (URL)
For a **hosted** server you connect to over the network (Streamable HTTP).

- Under **"🌐 Add remote MCP server (URL)"**:
  - **Server URL** — e.g. `https://example.com/mcp`
  - **Name** *(optional)*
  - **Bearer token** *(optional)* — sent as `Authorization: Bearer …`
- Click **Connect**.

---

## Check it's working

Each plugin row shows a live status:

- `● connecting…` — starting up (first run may download the package).
- `● connected · N tools` — ready to use ✅
- `● error: …` — see [Troubleshooting](#troubleshooting).

---

## Approvals (auto‑run)

By default the agent runs plugin tools **without asking** (`repoAgent.plugins.autoRun = true`).
Prefer to approve each external tool call? Turn it **off** in Settings (search "Repo Agent") and you'll get a **Run / Reject** prompt for every plugin tool.

---

## Manage plugins

- **Remove** — click **Remove** on a plugin's row.
- **Status** — updates live in the panel.
- Removing a plugin also deletes its stored secrets.

---

## Secrets & security

- Keys, tokens, and connection strings are stored in **VS Code SecretStorage** — never written to your code, settings, or globalState.
- ⚠️ Plugins run real code (a local process via `npx`, or a network call). Only add servers you trust — the same as any MCP client, including Claude.

---

## Find more servers

- **Browse more →** in the panel opens the official registry: <https://github.com/modelcontextprotocol/servers>.
- Curated lists like *awesome-mcp-servers* are handy too — pick a server, then use **npm/GitHub** or **remote URL** to add it. (An "awesome list" repo itself isn't installable — it's just a directory of links.)

---

## Troubleshooting

- **`command not found` / nothing connects** → install **Node.js** (gives you `npx`) and reload the window.
- **A plugin shows `error`** → open **View → Output → "Repo Agent"** for the real message (bad key, wrong package name, network error…).
- **Wrong package name** → double‑check it on npmjs.com; some servers are Python‑only (`uvx …`) — use the **custom command** with `uvx` if you have it.
- **Remote server won't connect** → this build supports the **Streamable HTTP** transport with **no‑auth or a bearer token**. Legacy SSE‑only servers and servers requiring an **OAuth login** aren't supported yet.

---

## Examples

| Goal | How |
|---|---|
| GitHub issues/PRs | Catalog → **GitHub** → paste a token |
| Web search | Catalog → **Web Search (Tavily/Brave)** or **Exa** |
| Query a Postgres DB | Catalog → **Postgres** → paste the connection string |
| Drive a real browser | Catalog → **Playwright** |
| Any npm MCP server | **Install from npm or GitHub** → `@scope/server` |
| A GitHub‑hosted server | **Install from npm or GitHub** → `owner/repo` |
| Your local server | **Add custom plugin** → `python server.py` |
| A hosted server | **Add remote MCP server (URL)** → paste the URL |
