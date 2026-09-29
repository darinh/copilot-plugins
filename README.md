# copilot-plugins

A [GitHub Copilot CLI](https://docs.github.com/en/copilot/how-tos/copilot-cli) plugin
marketplace. It holds skill packs written for other AI coding agents, such as Cursor, converted so
that Copilot CLI can load them.

A marketplace is a GitHub repository with a catalog at `.github/plugin/marketplace.json`. After you
add the marketplace to Copilot CLI once, you can install, update and remove its plugins by name.
Each plugin in `plugins/` is a complete Copilot CLI plugin: its skills, its custom agents, and its
upstream license.

These are unofficial conversions. The upstream authors did not write or review them. A bug in a
converted plugin belongs here, not upstream.

## Plugins

| Plugin | What it is | Converted from | License |
| --- | --- | --- | --- |
| `pstack` | 47 skills and 2 agents for rigorous, verified agent workflows: playbooks for features, bug fixes and reviews, design principles, and multi-model review. | [`pstack` in cursor/plugins](https://github.com/cursor/plugins/tree/main/pstack) | MIT, Copyright (c) 2026 Lauren Tan. See [`plugins/pstack/LICENSE`](plugins/pstack/LICENSE). |

Copilot CLI puts the plugin's name in front of a plugin agent's name. So the `pstack` agents are
`pstack:poteto-agent` and `pstack:comment-sicko`, as in `copilot --agent pstack:poteto-agent`.
Skills keep their own names, as in `/poteto-mode`.

## Install

You need Copilot CLI. Run these once on each computer:

```shell
copilot plugin marketplace add darinh/copilot-plugins
copilot plugin install pstack@darinh
```

`darinh` is the marketplace's name, taken from its catalog. Start a new Copilot CLI session
afterwards. `copilot plugin list` shows the plugin, and `copilot skill list` shows its skills.

To remove it, run `copilot plugin uninstall pstack@darinh`.

## Update

Copilot CLI copies a plugin when it installs it, so a new version here does not reach your computer
on its own. To get it, run:

```shell
copilot plugin update pstack@darinh
```

`copilot plugin update --all` updates every installed plugin. To update at the start of every
session instead, set `"autoUpdate": true` on the `darinh` entry under `extraKnownMarketplaces` in
`~/.copilot/settings.json`.

## How the plugins are made

Nothing in `plugins/` is edited by hand. `convert-skills`, a command-line tool by the owner of this
repository, generates it:

- `convert-skills` reads the upstream repository and converts each skill and agent into the form
  Copilot CLI expects. Frontmatter, tool names, agent references and file layout all change.
- `convert-skills sync` pulls later upstream changes and merges them into the converted copy.
- `convert-skills publish` writes the plugin into `plugins/<name>/` and its entry into the catalog.

To publish a new version, on the computer that holds the `convert-skills` workspace:

```shell
convert-skills sync pstack
convert-skills publish pstack --out <path to this repository>
git -C <path to this repository> commit -m "feat: publish pstack <version>"
git -C <path to this repository> push
```

`publish` stages what it writes, so git records the executable bit on the plugin's scripts.
