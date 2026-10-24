# archify — Cowork plugin

A repackaging of **[tt-a1i/archify](https://github.com/tt-a1i/archify)** in the canonical Claude plugin layout, so it installs cleanly in **Cowork** (and Claude Code) by URL. The plugin lives under `plugins/archify/` with its own `plugin.json`.

The skill itself is tt-a1i's original work, licensed MIT (see [LICENSE](./LICENSE) and the skill's own `THIRD_PARTY_NOTICES.md`) — unmodified. This repo only adds plugin manifests.

## What it does

Turns a description, Mermaid, or a repository into **validated, explorable standalone HTML**: architecture, workflow, sequence, data-flow, lifecycle/state, ERD, class, tree, timeline and waterfall diagrams, plus conclusion-first **explainer pages**. Dark/light themes and image/SVG/WebM export.

> Its `browser-check` / `visual-check` / export steps drive an installed Chrome/Chromium via CDP — have Google Chrome (or a Chromium) installed for those steps.

## Install in Cowork

1. In Cowork: **Customize → Plugins → Add**, point it at `https://github.com/krystianaskywetzel-eng/archify-plugin`
2. **Sync**, then **Install** the `archify` plugin.

## Install in Claude Code

```bash
/plugin marketplace add krystianaskywetzel-eng/archify-plugin
/plugin install archify@archify
```

## Updating

To pull upstream changes later, re-copy the skill into `plugins/archify/skills/archify/` from [tt-a1i/archify](https://github.com/tt-a1i/archify) (the inner `archify/` directory) and commit.

## Credit

Skill by **[tt-a1i](https://github.com/tt-a1i)** — [tt-a1i/archify](https://github.com/tt-a1i/archify). Unofficial repackaging for plugin-based installation.
