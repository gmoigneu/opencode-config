# OpenCode Configuration

Personal [OpenCode](https://opencode.ai) configuration with custom agents, skills, and provider models.

## Features

- **Granular Permissions**: Pre-configured access to `~/psh`, `~/projects`, and `~/.config/opencode`
- **Custom Agents**: Specialized agents including SaaS designer
- **Skills**: Upsun PaaS management and browser automation
- **Provider Models**: Antigravity-hosted Gemini 3 and Claude models

## Structure

```
~/.config/opencode/
├── opencode.json      # Main configuration
├── agents/            # Custom agent definitions
│   └── saas-designer.md
└── skills/            # Agent skills
    ├── agent-browser/
    └── upsun/
```

## Permissions

| Tool   | Default | Allowed Paths                                      |
|--------|---------|---------------------------------------------------|
| read   | ask     | ~/psh/*, ~/projects/*, ~/.config/opencode/*       |
| edit   | ask     | ~/psh/*, ~/projects/*, ~/.config/opencode/*       |
| glob   | ask     | ~/psh/*, ~/projects/*, ~/.config/opencode/*       |
| list   | ask     | ~/psh/*, ~/projects/*, ~/.config/opencode/*       |
| bash   | ask     | git, npm, pnpm, node, symfony, upsun, agent-browser |

## Models

Custom Antigravity-hosted models available:

- Gemini 3 Pro / Flash
- Claude Sonnet 4.5 (standard + thinking)
- Claude Opus 4.5 (thinking)

## MCP Servers

- **Context7**: Documentation lookup via `https://mcp.context7.com/mcp`

## License

Apache License 2.0 - see [LICENSE](LICENSE)
