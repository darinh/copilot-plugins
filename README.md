# pstack

GitHub Copilot CLI artifacts converted from [cursor/plugins](https://github.com/cursor/plugins/tree/adf3218ca2f5b9971eedc07a76bef22df7701539/pstack) (a Cursor plugin) at commit `adf3218ca2f5`, by convert-skills 0.1.0.
Converted: 2 agents, 47 skills.

## Source

| | |
| --- | --- |
| Repository | [https://github.com/cursor/plugins](https://github.com/cursor/plugins/tree/adf3218ca2f5b9971eedc07a76bef22df7701539) |
| Path | `pstack` |
| Tracking | `main` |
| Commit | [`adf3218ca2f5`](https://github.com/cursor/plugins/tree/adf3218ca2f5b9971eedc07a76bef22df7701539) |
| Read as | Cursor plugin (reader `cursor-plugin`) |
| License | MIT, see [LICENSE](LICENSE) |

## Install

```
convert-skills install pstack
```

That installs the package as the `pstack` Copilot CLI plugin. Its agents answer to `pstack:<name>`, and `copilot plugin list` shows it. `convert-skills uninstall pstack` removes it and puts `settings.json` back as it was.

## Update

```
convert-skills sync pstack
convert-skills install pstack
```

Sync converts the new upstream commit and three-way merges it into these files, so hand edits survive. An edit that collides with an upstream change stops the sync with conflict markers. A file upstream deletes stays until `--prune`, and manifest.json lists it under `retained`. `--regenerate` discards local edits instead. Copilot CLI loads the plugin from its own copy, so run `install` again after a sync to update it.

## Contents

Each artifact's fidelity is the worst of its features, so one dropped key makes it `unsupported` even when the rest converted exactly. `manifest.json` lists every feature.

| Name | Kind | Path | Fidelity |
| --- | --- | --- | --- |
| comment-sicko | agent | `agents/comment-sicko.agent.md` | approximated |
| poteto-agent | agent | `agents/poteto-agent.agent.md` | approximated |
| architect | skill | `skills/architect/SKILL.md` | approximated |
| arena | skill | `skills/arena/SKILL.md` | approximated |
| automate-me | skill | `skills/automate-me/SKILL.md` | approximated |
| blast-radius | skill | `skills/blast-radius/SKILL.md` | exact |
| bro | skill | `skills/bro/SKILL.md` | exact |
| create-verification-skill | skill | `skills/create-verification-skill/SKILL.md` | approximated |
| figure-it-out | skill | `skills/figure-it-out/SKILL.md` | approximated |
| how | skill | `skills/how/SKILL.md` | approximated |
| interrogate | skill | `skills/interrogate/SKILL.md` | approximated |
| maintain-verification-skill | skill | `skills/maintain-verification-skill/SKILL.md` | approximated |
| make-bot-ui | skill | `skills/make-bot-ui/SKILL.md` | approximated |
| no-comments | skill | `skills/no-comments/SKILL.md` | approximated |
| poteto-mode | skill | `skills/poteto-mode/SKILL.md` | unsupported |
| principle-attack-the-premise | skill | `skills/principle-attack-the-premise/SKILL.md` | approximated |
| principle-boundary-discipline | skill | `skills/principle-boundary-discipline/SKILL.md` | approximated |
| principle-build-the-lever | skill | `skills/principle-build-the-lever/SKILL.md` | approximated |
| principle-encode-lessons-in-structure | skill | `skills/principle-encode-lessons-in-structure/SKILL.md` | approximated |
| principle-exhaust-the-design-space | skill | `skills/principle-exhaust-the-design-space/SKILL.md` | approximated |
| principle-experience-first | skill | `skills/principle-experience-first/SKILL.md` | approximated |
| principle-fix-root-causes | skill | `skills/principle-fix-root-causes/SKILL.md` | approximated |
| principle-foundational-thinking | skill | `skills/principle-foundational-thinking/SKILL.md` | approximated |
| principle-guard-the-context-window | skill | `skills/principle-guard-the-context-window/SKILL.md` | approximated |
| principle-laziness-protocol | skill | `skills/principle-laziness-protocol/SKILL.md` | approximated |
| principle-make-operations-idempotent | skill | `skills/principle-make-operations-idempotent/SKILL.md` | approximated |
| principle-migrate-callers-then-delete-legacy-apis | skill | `skills/principle-migrate-callers-then-delete-legacy-apis/SKILL.md` | approximated |
| principle-minimize-reader-load | skill | `skills/principle-minimize-reader-load/SKILL.md` | approximated |
| principle-model-the-domain | skill | `skills/principle-model-the-domain/SKILL.md` | approximated |
| principle-never-block-on-the-human | skill | `skills/principle-never-block-on-the-human/SKILL.md` | approximated |
| principle-outcome-oriented-execution | skill | `skills/principle-outcome-oriented-execution/SKILL.md` | approximated |
| principle-prove-it-works | skill | `skills/principle-prove-it-works/SKILL.md` | approximated |
| principle-redesign-from-first-principles | skill | `skills/principle-redesign-from-first-principles/SKILL.md` | approximated |
| principle-separate-before-serializing-shared-state | skill | `skills/principle-separate-before-serializing-shared-state/SKILL.md` | approximated |
| principle-sequence-verifiable-units | skill | `skills/principle-sequence-verifiable-units/SKILL.md` | approximated |
| principle-subtract-before-you-add | skill | `skills/principle-subtract-before-you-add/SKILL.md` | approximated |
| principle-test-behavior-not-implementation | skill | `skills/principle-test-behavior-not-implementation/SKILL.md` | approximated |
| principle-type-system-discipline | skill | `skills/principle-type-system-discipline/SKILL.md` | approximated |
| recall | skill | `skills/recall/SKILL.md` | exact |
| reflect | skill | `skills/reflect/SKILL.md` | approximated |
| setup-pstack | skill | `skills/setup-pstack/SKILL.md` | exact |
| show-me-your-work | skill | `skills/show-me-your-work/SKILL.md` | approximated |
| swarm | skill | `skills/swarm/SKILL.md` | approximated |
| tdd | skill | `skills/tdd/SKILL.md` | approximated |
| teach | skill | `skills/teach/SKILL.md` | exact |
| technical-writing | skill | `skills/technical-writing/SKILL.md` | approximated |
| typescript-best-practices | skill | `skills/typescript-best-practices/SKILL.md` | unsupported |
| unslop | skill | `skills/unslop/SKILL.md` | approximated |
| why | skill | `skills/why/SKILL.md` | approximated |

## Not carried

These source files have no Copilot CLI equivalent in this package and are listed in `manifest.json` under `notCarried`.

| Path | Files | Examples |
| --- | --- | --- |
| `.cursor-plugin/` | 1 | `.cursor-plugin/plugin.json` |
| `.gitignore` | 1 | |
| `README.md` | 1 | |
| `assets/` | 1 | `assets/logo.png` |
| `automations/` | 12 | `automations/benny/FOR_AGENTS.md`, `automations/benny/README.md`, `automations/benny/skills/reproduce-and-fix-issues/SKILL.md` |
| `docs/` | 17 | `docs/guide/01-setup.md`, `docs/guide/02-poteto-mode.md`, `docs/guide/03-understand.md` |

## Needs a human

The converter does these deterministically only as far as it can. Each item below is text that still reads as written for the source harness, or a feature it could not carry. `manifest.json` lists every item.

| Kind | Count |
| --- | --- |
| command-substitution | 2 |
| dropped-link | 1 |
| foreign-token | 65 |
| runtime-mention | 18 |
| unsupported-artifact | 1 |

### command-substitution

| Where | Detail |
| --- | --- |
| `skills/typescript-best-practices/SKILL.md:17` | !`, a cast, or a "should never happen" throw. \| \| ` was executed by the source harness and is inert here |
| `skills/typescript-best-practices/references/patterns.md:94` | !`, ` was executed by the source harness and is inert here |

### dropped-link

| Where | Detail |
| --- | --- |
| `skills/why/references/synthesizer-prompt.md:65` | \[PR #123\](url) pointed at url, which is not in the converted package |

### foreign-token

| Where | Detail |
| --- | --- |
| `skills/architect/SKILL.md:33` | matches /\.mdc\b/, use a Copilot .instructions.md file |
| `skills/architect/SKILL.md:33` | matches /`(?:gpt\|claude\|grok\|gemini\|composer)-\[\w.-\]*-(?:max\|xhigh\|high\|medium\|low)(?:-fast)?`/, use the same model with reasoning_effort as its own task field (`gpt-5.6-sol-max` becomes `model: "gpt-5.6-sol"` with `reasoning_effort: "max"`) |
| `skills/arena/SKILL.md:28` | matches /`(?:gpt\|claude\|grok\|gemini\|composer)-\[\w.-\]*-(?:max\|xhigh\|high\|medium\|low)(?:-fast)?`/, use the same model with reasoning_effort as its own task field (`gpt-5.6-sol-max` becomes `model: "gpt-5.6-sol"` with `reasoning_effort: "max"`) |
| `skills/arena/SKILL.md:41` | matches /`(?:gpt\|claude\|grok\|gemini\|composer)-\[\w.-\]*-(?:max\|xhigh\|high\|medium\|low)(?:-fast)?`/, use the same model with reasoning_effort as its own task field (`gpt-5.6-sol-max` becomes `model: "gpt-5.6-sol"` with `reasoning_effort: "max"`) |
| `skills/automate-me/SKILL.md:29` | matches /~\/\.cursor\//, use the Copilot counterpart under ~/.copilot, if there is one |
| `skills/automate-me/SKILL.md:29` | matches /\bagent-transcripts\//, use the session's events.jsonl under ~/.copilot/session-state/<session-id>/, the folder the system prompt names |
| `skills/how/SKILL.md:11` | matches /\.mdc\b/, use a Copilot .instructions.md file |
| `skills/how/SKILL.md:27` | matches /`(?:gpt\|claude\|grok\|gemini\|composer)-\[\w.-\]*-(?:max\|xhigh\|high\|medium\|low)(?:-fast)?`/, use the same model with reasoning_effort as its own task field (`gpt-5.6-sol-max` becomes `model: "gpt-5.6-sol"` with `reasoning_effort: "max"`) |
| `skills/how/SKILL.md:28` | matches /`readonly`/, use agent_type "explore" for pure reads, or a prompt that forbids writes |
| `skills/how/SKILL.md:37` | matches /`(?:gpt\|claude\|grok\|gemini\|composer)-\[\w.-\]*-(?:max\|xhigh\|high\|medium\|low)(?:-fast)?`/, use the same model with reasoning_effort as its own task field (`gpt-5.6-sol-max` becomes `model: "gpt-5.6-sol"` with `reasoning_effort: "max"`) |
| `skills/how/SKILL.md:38` | matches /`readonly`/, use agent_type "explore" for pure reads, or a prompt that forbids writes |
| `skills/how/SKILL.md:47` | matches /`(?:gpt\|claude\|grok\|gemini\|composer)-\[\w.-\]*-(?:max\|xhigh\|high\|medium\|low)(?:-fast)?`/, use the same model with reasoning_effort as its own task field (`gpt-5.6-sol-max` becomes `model: "gpt-5.6-sol"` with `reasoning_effort: "max"`) |
| `skills/how/SKILL.md:48` | matches /`readonly`/, use agent_type "explore" for pure reads, or a prompt that forbids writes |
| `skills/interrogate/SKILL.md:40` | matches /`(?:gpt\|claude\|grok\|gemini\|composer)-\[\w.-\]*-(?:max\|xhigh\|high\|medium\|low)(?:-fast)?`/, use the same model with reasoning_effort as its own task field (`gpt-5.6-sol-max` becomes `model: "gpt-5.6-sol"` with `reasoning_effort: "max"`) |
| `skills/interrogate/SKILL.md:41` | matches /`(?:gpt\|claude\|grok\|gemini\|composer)-\[\w.-\]*-(?:max\|xhigh\|high\|medium\|low)(?:-fast)?`/, use the same model with reasoning_effort as its own task field (`gpt-5.6-sol-max` becomes `model: "gpt-5.6-sol"` with `reasoning_effort: "max"`) |
| `skills/interrogate/SKILL.md:42` | matches /`(?:gpt\|claude\|grok\|gemini\|composer)-\[\w.-\]*-(?:max\|xhigh\|high\|medium\|low)(?:-fast)?`/, use the same model with reasoning_effort as its own task field (`gpt-5.6-sol-max` becomes `model: "gpt-5.6-sol"` with `reasoning_effort: "max"`) |
| `skills/interrogate/SKILL.md:47` | matches /`readonly`/, use agent_type "explore" for pure reads, or a prompt that forbids writes |
| `skills/poteto-mode/SKILL.md:31` | matches /(?<!\[\w/.\])\/loop\b/, use autopilot mode |
| `skills/poteto-mode/SKILL.md:89` | matches /`(?:gpt\|claude\|grok\|gemini\|composer)-\[\w.-\]*-(?:max\|xhigh\|high\|medium\|low)(?:-fast)?`/, use the same model with reasoning_effort as its own task field (`gpt-5.6-sol-max` becomes `model: "gpt-5.6-sol"` with `reasoning_effort: "max"`) |
| `skills/poteto-mode/SKILL.md:131` | matches /(?<!\[\w/.\])\/loop\b/, use autopilot mode |
| `skills/poteto-mode/playbooks/autonomous-run.md:6` | matches /(?<!\[\w/.\])\/loop\b/, use autopilot mode |
| `skills/poteto-mode/playbooks/autopilot-full.md:10` | matches /(?<!\[\w/.\])\/loop\b/, use autopilot mode |
| `skills/poteto-mode/playbooks/autopilot-stack.md:6` | matches /(?<!\[\w/.\])\/loop\b/, use autopilot mode |
| `skills/poteto-mode/playbooks/babysit.md:12` | matches /(?<!\[\w/.\])\/loop\b/, use autopilot mode |
| `skills/poteto-mode/playbooks/bug-fix.md:8` | matches /(?<!\[\w/.\])\/loop\b/, use autopilot mode |
| | and 40 more in `manifest.json` |

### runtime-mention

| Where | Detail |
| --- | --- |
| `skills/automate-me/SKILL.md:11` | names the source runtime: This skill orchestrates three others: an inline mining pass (see step 1), Cursor's built-in `create-skill` (authoring), and the **unslop** skill (prose discipline). It sequences them. It doesn't replace them. |
| `skills/automate-me/SKILL.md:67` | names the source runtime: Use Cursor's built-in `create-skill` skill to author the skill. Placement: |
| `skills/poteto-mode/SKILL.md:22` | names the source runtime: - Any prose surface → the **unslop** skill. Your reply is a prose surface. Write it per **Writing the reply**. Agent-facing prose also follows the **create-skill** skill (Cursor's built-in for authoring SKILL.md files). |
| `skills/poteto-mode/SKILL.md:27` | names the source runtime: - Any PR-status request → the **Babysit** playbook (`playbooks/babysit.md`), and not Cursor's built-in babysit skill, whose description matches the same words. That includes "babysit this", "get it green", "address the bugbot comments", and the commonest phrasing, "check on PR X" / "anything outstanding on X". Never triggered by merely opening a PR. Declare its mode before polling. The playbook's step 1 owns the request-to-mode mapping. Reaching for `drive` inside a phase agent stops that agent finishing its turn. |
| `skills/poteto-mode/SKILL.md:136` | names the source runtime: - **Pause safely.** Suspending in-flight work cleanly so it can be resumed, on an explicit pause, going offline, a Cursor restart, or imminent context compaction. The complement to Session pickup. Full steps: `playbooks/pause-safely.md`. |
| `skills/poteto-mode/playbooks/authoring-a-skill.md:5` | names the source runtime: 1. Use the **create-skill** skill (Cursor's built-in for authoring SKILL.md files). |
| `skills/poteto-mode/playbooks/autonomous-run.md:6` | names the source runtime: 2. Pick the wake mechanism using Cursor's `/loop` command (a built-in, not a pstack skill). An event to watch (CI, a merge, a ref advancing) gets a watcher subagent that wakes you on the event, with a long time-based heartbeat as fallback. No event gets a fixed-interval heartbeat sized to when the result is worth re-checking. |
| `skills/poteto-mode/playbooks/autopilot-full.md:6` | names the source runtime: 2. **Spawn one owner per PR with the full lifecycle and an early trail.** Resolve the forge once for the program. GitHub CLI (`gh`) is the default. If `command -v origin` succeeds and Origin can resolve the repository, use `origin pr ...` for PR create, edit, view, watch, and merge operations. Otherwise stay on `gh` and record the fallback. Never require Graphite (`gt`). One Cursor cloud agent per PR owns build, the first push, a ready PR, self-proof on the real artifact (the **prove-it-works** principle skill), skeptical Bugbot triage per `../references/bugbot-triage.md`, a slop-strip (the `deslop` skill from the `cursor-team-kit` plugin (`/deslop`)), `/no-comments` (the **no-comments** skill), a rebase onto current trunk, the babysit loop to green (`playbooks/babysit.md`), and the merge itself. Within about 15 minutes, every owner starts a `decisions.tsv` trail per the **show-me-your-work** skill, pushes its first branch snapshot, and opens the PR ready, never draft. Open the PR before self-proof so the URL, decisions, and checks form a durable trail. Keep `decisions.tsv` uncommitted and return it with the reports. As soon as a subagent starts, the owner adds its ID, expected runtime (at least the longest past run of that kind), and state to a `children.tsv` kept the same way. The owner does the first rebase before the code-ready report and babysit, whether or not trunk has drifted. In fix rounds, the owner keeps that merge base. The owner rebases again only at merge prep (step 5), on a `git merge-tree` conflict with trunk, or on a CI failure that comes from a change on trunk. When the shipped code is final, after the slop-strip and `/no-comments`, it reports the code-ready head SHA. It also reports the SHA of each later push that changes the patch. Self-proof, CI, and babysit then run in parallel with the swarm. The owner reports merge-ready with the head SHA when self-proof, CI, and babysit finish. Before a push that starts a round, run the pre-review checks that the repo's AGENTS.md files and rules name for the touched paths. Run them on the committed head. A hook pass is not proof. To publish each rebase, push the owner's own branch with `git push --force-with-lease` after an `ls-remote` check. Never force-push a shared branch. The merge is the one step an owner may not take alone. Step 4 gates it. |
| `skills/poteto-mode/playbooks/autopilot-stack.md:5` | names the source runtime: 1. **Run the owner loop unchanged.** Resolve the forge once for the program. GitHub CLI (`gh`) is the default. If `command -v origin` succeeds and Origin can resolve the repository, use `origin pr ...` for PR create, edit, view, watch, and merge operations. Otherwise stay on `gh` and record the fallback. Never require Graphite (`gt`). One Cursor cloud agent per PR owns its change end to end: build, first push, a ready PR opened before self-proof, self-proof (gates, CI, receipts), skeptical Bugbot triage per `../references/bugbot-triage.md`, a slop-strip (the `deslop` skill from the `cursor-team-kit` plugin (`/deslop`)), `/no-comments` (the **no-comments** skill), and babysit to green per `playbooks/babysit.md`. Owners parallelize when the work is self-contained. Within about 15 minutes, every owner starts a `decisions.tsv` trail per the **show-me-your-work** skill, pushes its first branch snapshot, and opens the PR ready, never draft. Keep the trail uncommitted and return it in the report. Owners also keep the `children.tsv` of Autopilot-full step 2. |
| `skills/poteto-mode/playbooks/babysit.md:3` | names the source runtime: **You own the merge frontier. Declare a mode, clear one PR at a time, stop where the human's call begins.** This playbook replaces Cursor's built-in babysit skill for these requests, so do not route there even though its description matches the same words. A request to land or ship is `playbooks/shipping.md`, which begins where this playbook ends. |
| `skills/poteto-mode/playbooks/bug-fix.md:8` | names the source runtime: 2. Binary-search the cause. Form the candidate hypotheses, then rule them out until one survives. Seed them with `how` over the affected subsystem and the **why** skill for regression history. Each pass, take the split that cuts the most remaining problem space, get runtime evidence, eliminate. When program state is unclear, add instrumentation or logging and read it as the code runs. Don't guess. Drive a long or stubborn hunt with Cursor's `/loop` command. Confirm the surviving *mechanism* with runtime evidence before the step-3 architect/interrogate fan-out. |
| `skills/poteto-mode/playbooks/orchestrate.md:95` | names the source runtime: - Never resume an agent to check on it. A resume restarts an idle agent. Probe read-only: the ledger, `units.tsv`, `gh`, pushed branches, the cloud agent's status in the Cursor dashboard. Transcript mtime is not liveness. |
| `skills/poteto-mode/playbooks/orchestrate.md:101` | names the source runtime: - After a Cursor restart: local agents are dead, cloud work is not. Re-read the standing orders and `units.tsv`, recompute the frontier, reattach cloud work by PR and branch rather than agent id, respawn one sub-coordinator per track from its stored brief plus current state, drain, resume. The dead session's store lock clears itself on the next write. `orch` replaces a lock whose holder pid is gone. |
| `skills/poteto-mode/playbooks/shipping.md:7` | names the source runtime: 1. **Resolve the forge, then verify every PR independently.** GitHub CLI (`gh`) is the default. If `command -v origin` succeeds and Origin can resolve the repository, use `origin pr ...` for PR view, watch, edit, and merge operations. Otherwise stay on `gh` and record the fallback. Never require Graphite (`gt`). One subagent per PR, not batched, each a Cursor cloud agent, each exercising the real surface with the matching control skill (such as `control-ui` or `control-cli` from `cursor-team-kit`) against parent versus head. Each returns `PASS`, `PASS+NOTES` or `FAIL` and posts that verdict on its own PR. Safe means a verdict from an agent that did not write the code. CI green is not a verdict, and an approving bot review is not a verdict. |
| `skills/poteto-mode/playbooks/worktree-cleanup.md:10` | names the source runtime: 6. Simulators and other reclaimers. Simulators are usually the next-biggest win. `xcrun simctl --set testing delete all` (XCTestDevices clones), `xcrun simctl delete unavailable`, and `xcrun simctl runtime list` then `runtime delete <id>` for old runtimes. More when needed: Xcode `DerivedData` and `iOS DeviceSupport`, `~/Library/Application Support/Cursor` (`state.vscdb.backup`, and `snapshots/roots/<root>` where a `<root>` named for a folder you opened as a workspace balloons), package caches (pnpm, uv, brew, yarn). Clear only caches the user has not said to keep. |
| `skills/reflect/SKILL.md:60` | names the source runtime: - Substantive existing-skill edit (a new section, a new pattern table, more than ~10 lines): hand to Cursor's built-in `create-skill` skill and run its draft / test / iterate loop. |
| `skills/setup-pstack/SKILL.md:15` | names the source runtime: Enumerate the model slugs you can pass to a `task` subagent in this session. That is the dependable source. If Cursor also exposes a models API or CLI that lists the user's entitled models, prefer it for completeness. If you cannot detect any, ask the user to paste the slugs they have access to. Never write a real slug you have not confirmed is available. The aliases `inherit-parent` and `auto` are always valid even though they are not detected slugs. |
| `skills/why/SKILL.md:64` | names the source runtime: Before spawning investigators, list the available MCPs from the Cursor environment. Use the available-tools map when present. Otherwise inspect the `mcps/` directory Cursor exposes for enabled MCP servers. |

### unsupported-artifact

| Where | Detail |
| --- | --- |
| `skills/typescript-best-practices/SKILL.md` | path filter not carried: **/*.ts, **/*.tsx |

## Fidelity

One row per feature the converter decided on.

| Fidelity | Features | Meaning |
| --- | --- | --- |
| exact | 136 | behaves the same in Copilot CLI |
| approximated | 50 | converted, with a known difference noted in manifest.json |
| unsupported | 5 | no Copilot equivalent; dropped or not converted |
| unverified | 0 | converted to a Copilot feature whose behaviour no primary source confirms |
