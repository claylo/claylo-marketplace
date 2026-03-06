# claylo-marketplace

Claude Code plugins I build and maintain. If it's listed here, it works and I use it.

## Install

```
/plugin marketplace add claylo/claylo-marketplace
```

Then install individual plugins:

```
/plugin install <plugin-name>@claylo-marketplace
```

## Plugins

### [actionista](https://github.com/claylo/actionista) `v0.2.0`

GitHub Actions assistant — helps create, review, and optimize workflows with up-to-date action versions, migration guidance, and best practices.

- Tracks 118 GitHub Actions with current versions and migration diffs
- MCP server with `lookup_action`, `list_actions`, and `check_workflow` tools
- Skill content covering patterns, security, and workflow syntax
- Daily automated index updates via Claude Code Action

```
/plugin install actionista@claylo-marketplace
```

## Adding plugins

Each plugin entry in `.claude-plugin/marketplace.json` points to a standalone git repo. Plugins are self-contained — install one or all, they don't depend on each other unless noted.

```json
{
  "name": "plugin-name",
  "source": {
    "source": "url",
    "url": "https://github.com/claylo/plugin-name.git"
  },
  "description": "What it does",
  "version": "1.0.0",
  "strict": true
}
```

## License

MIT
