# Ejentum Integrations

Official integration guides and skill files for the [Ejentum Logic API](https://ejentum.com) — a runtime reasoning harness for AI agents.

Your agent POSTs a task description and a mode. The API returns a structured cognitive injection (failure pattern to avoid, procedure to follow, verification criterion, suppress/amplify signals). Your agent absorbs the injection and writes from it. 679 engineered abilities across four modes: reasoning, code, anti-deception, memory.

## What's here

| Folder | What it is | Install time |
|---|---|---|
| [`/n8n`](./n8n) | One HTTP Request tool + pre-built workflow JSON. Agent auto-routes to the right mode via `$fromAI()`. | 3 min |
| [`/claude-code`](./claude-code) | Five native Claude Code skill files (`ejentum-unified`, `ejentum-reasoning`, `ejentum-code`, `ejentum-anti-deception`, `ejentum-memory`). Drop into `~/.claude/skills/`, set one env var, done. | 5 min |

Each subfolder has a README with picture-by-picture install walkthrough and downloadable assets.

### Standalone MCP server

For agentic IDEs that speak the Model Context Protocol (Claude Code, Cursor, Cline, Windsurf, Continue), there's also a packaged MCP server: [github.com/ejentum/ejentum-mcp](https://github.com/ejentum/ejentum-mcp). One-line install via `npx -y ejentum-mcp`, set `EJENTUM_API_KEY`, and the four harness modes appear as MCP tools the agent can call. Same `/skills/` files as `/claude-code` here, plus editor-rules adapters for Cursor/Windsurf/Cline at `/editors/`.

## Other frameworks

| Framework | Docs |
|---|---|
| LangChain / LangGraph | https://ejentum.com/docs/integrations#langchain |
| CrewAI | https://ejentum.com/docs/integrations#crewai |
| Cursor / Windsurf / Codex | https://ejentum.com/docs/integrations#agentic-ides |
| Make.com | https://ejentum.com/docs/integrations#makecom |
| Any framework (universal pattern) | https://ejentum.com/docs/integrations#universal-pattern |

If you want an integration that isn't here yet, open an issue.

## Getting an API key

Free tier: 100 calls, no card. Generate at [ejentum.com/dashboard](https://ejentum.com/dashboard).

Paid: Ki €19/mo (5,000 calls), Haki €49/mo (10,000 calls + multi-mode). See [pricing](https://ejentum.com/pricing).

## Benchmarks and evidence

- Homepage: https://ejentum.com (five benchmark pills across all four harnesses)
- Full methodology: https://ejentum.com/docs/benchmarks
- "Under Pressure" research paper: [Zenodo](https://doi.org/10.5281/zenodo.19392715) · [SSRN](https://ssrn.com/abstract=6512038)

## License

MIT. See [LICENSE](./LICENSE).

## Contributing

PRs welcome on any integration folder. For additions (new framework), open an issue first so we can scope it together.

For questions about the Ejentum API itself: info@ejentum.com.
