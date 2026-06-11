# Ejentum Integrations

Official integration guides and skill files for the [Ejentum API](https://ejentum.com), the Reasoning Harness for Agentic AI.

Your agent POSTs a task description and a mode. The API returns a structured cognitive injection (failure pattern to avoid, procedure to follow, verification criterion, suppress/amplify signals). Your agent absorbs the injection and writes from it. 679 engineered abilities across four modes: reasoning, code, anti-deception, memory.

## What's here

| Folder | What it is | Install time |
|---|---|---|
| [`/n8n`](./n8n) | One HTTP Request tool + pre-built workflow JSON. Agent auto-routes to the right mode via `$fromAI()`. | 3 min |
| [`/claude-code`](./claude-code) | Five native Claude Code skill files (`ejentum-unified`, `ejentum-reasoning`, `ejentum-code`, `ejentum-anti-deception`, `ejentum-memory`). Drop into `~/.claude/skills/`, set one env var, done. | 5 min |

Each subfolder has a README with picture-by-picture install walkthrough and downloadable assets.

## Native packages

Standalone packages on PyPI and npm, one per host framework. Each speaks its host's native idiom; pick the one that matches your stack.

### Python (PyPI)

| Framework | Install | Repo |
|---|---|---|
| CrewAI | `pip install crewai-ejentum` | [crewai-ejentum](https://github.com/ejentum/crewai-ejentum) |
| Agno | `pip install agno-ejentum` | [agno-ejentum](https://github.com/ejentum/agno-ejentum) |
| PydanticAI | `pip install pydantic-ai-ejentum` | [pydantic-ai-ejentum](https://github.com/ejentum/pydantic-ai-ejentum) |
| HuggingFace smolagents | `pip install smolagents-ejentum` | [smolagents-ejentum](https://github.com/ejentum/smolagents-ejentum) |
| LangChain | `pip install langchain-ejentum` | [langchain-ejentum](https://github.com/ejentum/langchain-ejentum) |
| Letta | `pip install letta-ejentum` | [letta-ejentum](https://github.com/ejentum/letta-ejentum) |
| Microsoft AutoGen | `pip install autogen-ejentum` | [autogen-ejentum](https://github.com/ejentum/autogen-ejentum) |
| LlamaIndex | (PyPI registration pending) | [llama-index-tools-ejentum](https://github.com/ejentum/llama-index-tools-ejentum) |

### TypeScript / JavaScript (npm)

| Framework | Install | Repo |
|---|---|---|
| Vercel AI SDK | `npm install ejentum-ai` | [ejentum-ai](https://github.com/ejentum/ejentum-ai) |
| Mastra | `npm install ejentum-mastra` | [ejentum-mastra](https://github.com/ejentum/ejentum-mastra) |
| LangGraph.js | `npm install ejentum-langgraph` | [ejentum-langgraph](https://github.com/ejentum/ejentum-langgraph) |
| Firebase Genkit | `npm install ejentum-genkit` | [ejentum-genkit](https://github.com/ejentum/ejentum-genkit) |
| n8n (community node) | `npm install n8n-nodes-ejentum` | [n8n-nodes-ejentum](https://github.com/ejentum/n8n-nodes-ejentum) |

### Agentic IDEs and editors

| Tool | How |
|---|---|
| Cursor, Claude Code, Windsurf, Continue, Cline, n8n MCP Client | `npx -y ejentum-mcp` (also listed on Glama and mcp.so) |
| Anthropic Claude Code plugin directory | Install from the directory UI (Published 2026-05-22) |
| Zed editor | Install **Ejentum** from Zed Extensions |
| Cursor / Windsurf / Cline rules files | Adapters under [`ejentum-mcp/editors/`](https://github.com/ejentum/ejentum-mcp/tree/main/editors) |
| Codex CLI | `.codex-plugin/plugin.json` shipped with `ejentum-mcp` |

If you want an integration that isn't here yet, open an issue.

## Getting an API key

Free tier: 30-day trial, no card. Generate at [ejentum.com/dashboard](https://ejentum.com/dashboard).

Paid: Ki €19/mo (5,000 calls), Super €49/mo (10,000 calls + multi-mode). See [pricing](https://ejentum.com/pricing).

## Benchmarks and evidence

- Homepage: https://ejentum.com (five benchmark pills across all four harnesses)
- Full methodology: https://ejentum.com/docs/benchmarks
- "Under Pressure" research paper: [Zenodo](https://doi.org/10.5281/zenodo.19392715) · [SSRN](https://ssrn.com/abstract=6512038)

## License

MIT. See [LICENSE](./LICENSE).

## Contributing

PRs welcome on any integration folder. For additions (new framework), open an issue first so we can scope it together.

For questions about the Ejentum API itself: info@ejentum.com.
