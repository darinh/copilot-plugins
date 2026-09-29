# copilot-plugins

A GitHub Copilot CLI plugin marketplace. Each plugin here is a skill pack from another agent
harness, converted for Copilot CLI by `convert-skills`.

## Install on a computer

You need Copilot CLI and access to this repository. The repository is private, so git has to be
signed in to GitHub, for example with `gh auth login`.

```powershell
copilot plugin marketplace add darinh/copilot-plugins
copilot plugin install pstack@darinh
```

Start a new Copilot CLI session afterwards. `copilot plugin list` shows the plugin, and
`copilot skill list` shows its skills.

## Get updates

Copilot CLI copies a plugin when it installs it, so a push here does not reach a computer on its
own. On each computer, run:

```powershell
copilot plugin marketplace update darinh
copilot plugin update pstack@darinh
```

To update at the start of every session instead, set `"autoUpdate": true` on the `darinh` entry
under `extraKnownMarketplaces` in `~/.copilot/settings.json`.

## Plugins

| Plugin | Converted from | License |
| --- | --- | --- |
| `pstack` | [cursor/plugins `pstack`](https://github.com/cursor/plugins/tree/main/pstack) | MIT, Copyright (c) 2026 Lauren Tan. The license text ships in `plugins/pstack/LICENSE`. |

The `pstack` plugin's agents answer to `pstack:<name>`, for example
`copilot --agent pstack:poteto-agent`.

## How this repository is updated

Nothing here is edited by hand. On the computer that holds the convert-skills workspace:

```powershell
convert-skills sync pstack
convert-skills publish pstack --out C:\path\to\copilot-plugins
git -C C:\path\to\copilot-plugins add -A
git -C C:\path\to\copilot-plugins commit -m "chore: publish pstack"
git -C C:\path\to\copilot-plugins push
```

`publish` rewrites `.github/plugin/marketplace.json` and `plugins/<slug>/`, and leaves other
plugins alone.
