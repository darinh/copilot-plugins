# copilot-plugins

A [GitHub Copilot CLI](https://docs.github.com/en/copilot/how-tos/copilot-cli) plugin
marketplace. It collects skill packs from different authors, written for other AI coding agents
such as Cursor, and converted so that Copilot CLI can load them.

A marketplace is a GitHub repository with a catalog at `.github/plugin/marketplace.json`. After you
add the marketplace to Copilot CLI once, you can install, update and remove its plugins by name.
Each plugin in `plugins/` is a complete Copilot CLI plugin: its skills, its custom agents, and the
license files of the project it came from.

These are unofficial conversions. The upstream authors did not write or review them. A bug in a
converted plugin belongs here, not upstream.

## Plugins

| Plugin | What it is | Converted from | License |
| --- | --- | --- | --- |
| `pstack` | 47 skills and 2 agents for rigorous, verified agent workflows: playbooks for features, bug fixes and reviews, design principles, and multi-model review. | [`pstack` in cursor/plugins](https://github.com/cursor/plugins/tree/main/pstack) | MIT, Copyright (c) 2026 Lauren Tan. See [`plugins/pstack/LICENSE`](plugins/pstack/LICENSE). |

Copilot CLI puts the plugin's name in front of a plugin agent's name. For example, the `pstack`
agents are `pstack:poteto-agent` and `pstack:comment-sicko`. Skills keep their own names, as in
`/poteto-mode`.

## Licenses

Each plugin keeps the license of the project it came from, and that license covers only that
plugin. The license files are in the plugin's own folder under `plugins/`, and the table above
names each one. No single license covers this repository as a whole.

## Install

You need Copilot CLI. Add the marketplace once on each computer, then install the plugins you want
by name:

```shell
copilot plugin marketplace add darinh/copilot-plugins
copilot plugin install <plugin>@darinh
```

For example, `copilot plugin install pstack@darinh`. `darinh` is the marketplace's name, taken from
its catalog, and `copilot plugin marketplace browse darinh` lists every plugin in it. Start a new
Copilot CLI session afterwards. `copilot plugin list` shows what you installed.

To remove a plugin, run `copilot plugin uninstall <plugin>@darinh`.

## Update

Copilot CLI copies a plugin when it installs it, so a new version here does not reach your computer
on its own. To get it, run:

```shell
copilot plugin update <plugin>@darinh
```

`copilot plugin update --all` updates every installed plugin. To update at the start of every
session instead, set `"autoUpdate": true` on the `darinh` entry under `extraKnownMarketplaces` in
`~/.copilot/settings.json`.

## How the plugins are made

Nothing in `plugins/` is edited by hand. `convert-skills`, a command-line tool by the owner of this
repository, generates it:

- `convert-skills` reads an upstream repository and converts each skill and agent into the form
  Copilot CLI expects. Frontmatter, tool names, agent references and file layout all change.
- `convert-skills sync` pulls later upstream changes and merges them into the converted copy.
- `convert-skills publish` writes the plugin into `plugins/<plugin>/` and its entry into the
  catalog. It copies that upstream's own license files into the plugin, and leaves every other
  plugin alone.

To publish a new version of a plugin, on the computer that holds the `convert-skills` workspace:

```shell
convert-skills sync <plugin>
convert-skills publish <plugin> --out <path to this repository>
git -C <path to this repository> commit -m "feat: publish <plugin> <version>"
git -C <path to this repository> push
```

`publish` stages what it writes, so git records the executable bit on each plugin's scripts.
