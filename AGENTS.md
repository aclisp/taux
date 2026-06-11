# Repository Instructions

## Scope

These instructions apply to the entire repository.

## Project Context

This project is a Tau mirror package for Pi. Treat files under `extensions/` as Pi extension code and files under `public/` as the browser UI served by the mirror extension.

## Pi Documentation

When working on Pi topics, read the relevant Pi documentation and examples before implementing or reviewing changes. This applies when the task concerns Pi itself, its SDK, extensions, themes, skills, prompt templates, TUI components, keybindings, custom providers, adding models, or Pi packages.

- Main documentation: `/opt/homebrew/lib/node_modules/@earendil-works/pi-coding-agent/README.md`
- Additional docs: `/opt/homebrew/lib/node_modules/@earendil-works/pi-coding-agent/docs`
- Examples: `/opt/homebrew/lib/node_modules/@earendil-works/pi-coding-agent/examples`

Resolve doc references relative to those roots:

- `docs/extensions.md` -> `/opt/homebrew/lib/node_modules/@earendil-works/pi-coding-agent/docs/extensions.md`
- `examples/extensions/` -> `/opt/homebrew/lib/node_modules/@earendil-works/pi-coding-agent/examples/extensions/`

Useful Pi topic entry points:

- Extensions: `docs/extensions.md`, `examples/extensions/`
- Themes: `docs/themes.md`
- Skills: `docs/skills.md`
- Prompt templates: `docs/prompt-templates.md`
- TUI components: `docs/tui.md`
- Keybindings: `docs/keybindings.md`
- SDK integrations: `docs/sdk.md`
- Custom providers: `docs/custom-provider.md`
- Adding models: `docs/models.md`
- Pi packages: `docs/packages.md`

Always read Pi `.md` files completely and follow relevant cross-references before implementing Pi-related changes. For example, follow `tui.md` when an extension uses TUI APIs.

## Checks

Use these commands for project validation:

```bash
npx tsc --noEmit
biome check --write
```

`biome` is installed globally for this project. Use `biome check --write` to format, lint, and organize imports for configured files.
