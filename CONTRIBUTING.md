# Contributing

This repo hosts integration guides and skill files for the [Ejentum Logic API](https://ejentum.com). Contributions welcome.

## What belongs here

- Integration guides for agent frameworks (LangChain, CrewAI, LlamaIndex, AutoGen, Cursor, Windsurf, Codex, etc.)
- Skill files for agentic IDEs (Claude Code, Cursor rules, etc.)
- Workflow templates for no-code platforms (n8n, Make.com, Zapier)
- Example integrations and reference implementations

## What doesn't

- The Ejentum Logic API core (closed source)
- The ability corpus (internal)
- Benchmarks (lives in [ejentum/benchmarks](https://github.com/ejentum/benchmarks))
- Anything requiring API key secrets in committed files

## Adding a new integration

1. Open an issue first, tag it `new-integration`. Say which framework and link a reference to the framework's tool/plugin conventions.
2. After acknowledgment, fork and work in a branch named `integration/<framework-name>`.
3. Structure: create a top-level folder for the framework (`/langchain`, `/crewai`, etc.) with a README following the pattern of `/n8n` and `/claude-code`.
4. Open PR referencing the issue.

## Fixes to existing integrations

- Screenshot updates, typos, broken links: PR directly, no issue needed.
- Breaking changes to install steps: open an issue first, tag `breaking-change`.

## Scope of reviews

- Small docs fixes: usually merged within a few days.
- New integrations: reviewed for technical correctness, scope fit, and maintenance burden. Some integrations may be declined if the framework has a conflicting official path.
- PRs that add nothing operational (pure prose rewrites without new information) are usually closed with a note.

## Testing locally

- n8n workflows: import the JSON into a test n8n instance and run the sample prompt.
- Skill files: drop into `~/.claude/skills/<name>/SKILL.md` and verify the agent auto-invokes on a matching task.
- For the API itself, use a free-tier key from [ejentum.com/dashboard](https://ejentum.com/dashboard).

## Questions about the API

Not contribution questions: email info@ejentum.com.

Contribution questions or integration design discussions: open an issue on this repo.
