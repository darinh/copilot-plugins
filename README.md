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
repository, generates it, and this repository is also its workspace:

- `sources/<plugin>.json` names each plugin's upstream repository.
- `packages/<plugin>/` is the converted copy. `convert-skills` reads the upstream repository and
  converts each skill and agent into the form Copilot CLI expects. Hand edits made here survive
  later updates, because each update is a three-way merge.
- `plugins/<plugin>/` is what Copilot CLI installs. It is published from `packages/<plugin>/`, with
  that upstream's own license files, and each plugin's entry is in `.github/plugin/marketplace.json`.
- The merge bases the three-way merge needs are pushed as `refs/convert-skills-bases/*`.

Every change arrives as a pull request. On a computer with `convert-skills` and a clone of this
repository:

```shell
convert-skills attach <path to this clone>
convert-skills onboard <upstream repository URL> --subpath <folder>
convert-skills pull <plugin>
convert-skills pull --all
```

`onboard` adds a new plugin. `pull` brings one plugin or all of them up to date with upstream. Each
works on its own branch in a temporary worktree, publishes the plugin, pushes the branch, and opens a
pull request here. If an upstream change collides with a hand edit, `pull` stops, keeps the
worktree, and prints the file to resolve and the command that finishes the update. `onboard` and
`pull` refuse a plugin whose upstream has no license file.

After a pull request merges, `copilot plugin update <plugin>@darinh` installs the new version, as
does `convert-skills update`.