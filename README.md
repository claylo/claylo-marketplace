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

GitHub Actions assistant — helps create, review, and optimize workflows with up-to-date action versions, migration guidance, and best practices

```
/plugin install actionista@claylo-marketplace
```

### [building-in-the-open](https://github.com/claylo/building-in-the-open) `v1.0.0`

Personas, skills, and quality gates for producing professional, self-contained development artifacts — from internal handoffs to end-user documentation

```
/plugin install building-in-the-open@claylo-marketplace
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
