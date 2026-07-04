# Wire Framework — Gemini CLI Extension

This extension provides the **Wire Framework**, an AI-accelerated delivery system for data platform engagements. It encodes 20+ years of analytics engineering methodology as executable workflow specifications, enabling an AI agent to produce production-grade artifacts across the full project lifecycle.

## Usage

All commands are available immediately — no install step required:

```
/dp start              — See all projects and available commands
/dp new                — Create a new project
/dp guide [new|resume|explain] — Interactive co-pilot: orients new users and surfaces the right next action
/dp autopilot <sow>    — Autonomous end-to-end execution from SOW
/dp status <project>   — Check project status
```

### Delivery commands

```
/dp requirements generate <project>   — Extract requirements from SOW
/dp requirements validate <project>   — Validate requirements
/dp requirements review <project>     — Stakeholder review

/dp conceptual_model generate <project>
/dp data_model generate <project>
/dp dbt generate <project>
/dp semantic_layer generate <project>
/dp dashboards generate <project>
... (and validate/review for each)
```

### Project data

Project data is stored in `.wire/` in the current repository. This directory is created automatically when you run `/dp new` or `/dp autopilot`.

## MCP Integrations

This extension configures optional MCP servers for:
- **Atlassian** — Jira issue tracking and Confluence document search
- **Fathom** — Meeting transcript context for reviews
- **Context7** — Library documentation lookups

## Tool Mapping

When following workflow specifications, use these Gemini CLI equivalents:

| Workflow Reference | Gemini CLI Tool |
|---|---|
| Read tool | Read files directly |
| Glob tool | Use `find` or `ls` commands |
| Grep tool | Use `grep` or `rg` commands |
| Write tool | Write files directly |
| Edit tool | Edit files directly |
| Bash tool | Run shell commands |
