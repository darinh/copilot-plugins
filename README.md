# pstack

GitHub Copilot CLI artifacts converted from [cursor/plugins](https://github.com/cursor/plugins/tree/6dbbdd50cef1bdbfb540f80df8b598d0a546e3aa/pstack) (a Cursor plugin) at commit `6dbbdd50cef1`, by convert-skills 0.1.0.
Converted: 2 agent, 44 skill.

## Source

| | |
| --- | --- |
| Repository | [https://github.com/cursor/plugins](https://github.com/cursor/plugins/tree/6dbbdd50cef1bdbfb540f80df8b598d0a546e3aa) |
| Path | `pstack` |
| Tracking | `6dbbdd50cef1bdbfb540f80df8b598d0a546e3aa` |
| Commit | [`6dbbdd50cef1`](https://github.com/cursor/plugins/tree/6dbbdd50cef1bdbfb540f80df8b598d0a546e3aa) |
| Read as | Cursor plugin (reader `cursor-plugin`) |
| License | MIT, see [LICENSE](LICENSE) |

## Install

```
convert-skills install pstack
```

That registers `skills/` with Copilot CLI, the same as `copilot skill add <this directory>/skills`. Add `--target agents,instructions` for the rest, and `convert-skills uninstall pstack` reverses every target.

## Update

```
convert-skills sync pstack
```

Sync converts the new upstream commit and three-way merges it into these files, so hand edits survive. An edit that collides with an upstream change stops the sync with conflict markers. `--regenerate` discards local edits instead.

## Contents

| Name | Kind | Path | Fidelity |
| --- | --- | --- | --- |
| comment-sicko | agent | `agents/comment-sicko.agent.md` | approximated |
| poteto-agent | agent | `agents/poteto-agent.agent.md` | approximated |
| architect | skill | `skills/architect/SKILL.md` | exact |
| arena | skill | `skills/arena/SKILL.md` | approximated |
| automate-me | skill | `skills/automate-me/SKILL.md` | exact |
| blast-radius | skill | `skills/blast-radius/SKILL.md` | exact |
| bro | skill | `skills/bro/SKILL.md` | exact |
| create-verification-skill | skill | `skills/create-verification-skill/SKILL.md` | exact |
| figure-it-out | skill | `skills/figure-it-out/SKILL.md` | exact |
| how | skill | `skills/how/SKILL.md` | exact |
| interrogate | skill | `skills/interrogate/SKILL.md` | exact |
| maintain-verification-skill | skill | `skills/maintain-verification-skill/SKILL.md` | exact |
| no-comments | skill | `skills/no-comments/SKILL.md` | exact |
| poteto-mode | skill | `skills/poteto-mode/SKILL.md` | unsupported |
| principle-boundary-discipline | skill | `skills/principle-boundary-discipline/SKILL.md` | exact |
| principle-build-the-lever | skill | `skills/principle-build-the-lever/SKILL.md` | exact |
| principle-encode-lessons-in-structure | skill | `skills/principle-encode-lessons-in-structure/SKILL.md` | exact |
| principle-exhaust-the-design-space | skill | `skills/principle-exhaust-the-design-space/SKILL.md` | exact |
| principle-experience-first | skill | `skills/principle-experience-first/SKILL.md` | exact |
| principle-fix-root-causes | skill | `skills/principle-fix-root-causes/SKILL.md` | exact |
| principle-foundational-thinking | skill | `skills/principle-foundational-thinking/SKILL.md` | exact |
| principle-guard-the-context-window | skill | `skills/principle-guard-the-context-window/SKILL.md` | exact |
| principle-laziness-protocol | skill | `skills/principle-laziness-protocol/SKILL.md` | exact |
| principle-make-operations-idempotent | skill | `skills/principle-make-operations-idempotent/SKILL.md` | exact |
| principle-migrate-callers-then-delete-legacy-apis | skill | `skills/principle-migrate-callers-then-delete-legacy-apis/SKILL.md` | exact |
| principle-minimize-reader-load | skill | `skills/principle-minimize-reader-load/SKILL.md` | exact |
| principle-model-the-domain | skill | `skills/principle-model-the-domain/SKILL.md` | exact |
| principle-never-block-on-the-human | skill | `skills/principle-never-block-on-the-human/SKILL.md` | exact |
| principle-outcome-oriented-execution | skill | `skills/principle-outcome-oriented-execution/SKILL.md` | exact |
| principle-prove-it-works | skill | `skills/principle-prove-it-works/SKILL.md` | exact |
| principle-redesign-from-first-principles | skill | `skills/principle-redesign-from-first-principles/SKILL.md` | exact |
| principle-separate-before-serializing-shared-state | skill | `skills/principle-separate-before-serializing-shared-state/SKILL.md` | exact |
| principle-sequence-verifiable-units | skill | `skills/principle-sequence-verifiable-units/SKILL.md` | exact |
| principle-subtract-before-you-add | skill | `skills/principle-subtract-before-you-add/SKILL.md` | exact |
| principle-type-system-discipline | skill | `skills/principle-type-system-discipline/SKILL.md` | exact |
| recall | skill | `skills/recall/SKILL.md` | exact |
| reflect | skill | `skills/reflect/SKILL.md` | exact |
| setup-pstack | skill | `skills/setup-pstack/SKILL.md` | exact |
| show-me-your-work | skill | `skills/show-me-your-work/SKILL.md` | exact |
| swarm | skill | `skills/swarm/SKILL.md` | approximated |
| tdd | skill | `skills/tdd/SKILL.md` | exact |
| teach | skill | `skills/teach/SKILL.md` | exact |
| technical-writing | skill | `skills/technical-writing/SKILL.md` | exact |
| typescript-best-practices | skill | `skills/typescript-best-practices/SKILL.md` | unsupported |
| unslop | skill | `skills/unslop/SKILL.md` | exact |
| why | skill | `skills/why/SKILL.md` | approximated |

## Needs a human

The converter does these deterministically only as far as it can. Each item below is text that still reads as written for the source harness, or a feature it could not carry. `manifest.json` lists every item.

| Kind | Count |
| --- | --- |
| command-substitution | 2 |
| dropped-link | 1 |
| foreign-token | 9 |
| runtime-mention | 23 |

### command-substitution

| Where | Detail |
| --- | --- |
| `skills/typescript-best-practices/SKILL.md:15` | !`, a cast, or a "should never happen" throw. \| \| ` was executed by the source harness and is inert here |
| `skills/typescript-best-practices/references/patterns.md:94` | !`, ` was executed by the source harness and is inert here |

### dropped-link

| Where | Detail |
| --- | --- |
| `skills/why/references/synthesizer-prompt.md:65` | \[PR #123\](url) pointed at url, which is not in the converted package |

### foreign-token

| Where | Detail |
| --- | --- |
| `skills/poteto-mode/SKILL.md:32` | matches /(?<!\[\w/.\])\/loop\b/, use autopilot mode |
| `skills/poteto-mode/SKILL.md:129` | matches /(?<!\[\w/.\])\/loop\b/, use autopilot mode |
| `skills/poteto-mode/playbooks/autonomous-run.md:3` | matches /(?<!\[\w/.\])\/loop\b/, use autopilot mode |
| `skills/poteto-mode/playbooks/autonomous-run.md:6` | matches /(?<!\[\w/.\])\/loop\b/, use autopilot mode |
| `skills/poteto-mode/playbooks/babysit.md:14` | matches /(?<!\[\w/.\])\/loop\b/, use autopilot mode |
| `skills/poteto-mode/playbooks/bug-fix.md:8` | matches /(?<!\[\w/.\])\/loop\b/, use autopilot mode |
| `skills/poteto-mode/playbooks/orchestrate.md:73` | matches /\bloop skill\b/, use autopilot mode |
| `skills/poteto-mode/playbooks/shipping.md:17` | matches /(?<!\[\w/.\])\/loop\b/, use autopilot mode |
| `skills/poteto-mode/playbooks/visual-parity.md:8` | matches /(?<!\[\w/.\])\/loop\b/, use autopilot mode |

### runtime-mention

| Where | Detail |
| --- | --- |
| `skills/automate-me/SKILL.md:12` | names the source runtime: This skill orchestrates three others: an inline mining pass (see step 1), Cursor's built-in `create-skill` (authoring), and the **unslop** skill (prose discipline). It sequences them; it doesn't replace them. |
| `skills/automate-me/SKILL.md:68` | names the source runtime: Use Cursor's built-in `create-skill` skill to author the skill. Placement: |
| `skills/automate-me/SKILL.md:110` | names the source runtime: - Cursor's built-in `create-skill` skill: skill authoring process and writing guidelines. |
| `skills/poteto-mode/SKILL.md:23` | names the source runtime: - Any prose surface → the **unslop** skill. Your reply is a prose surface; write it per **Writing the reply**. Agent-facing prose also follows the **create-skill** skill (Cursor's built-in for authoring SKILL.md files). |
| `skills/poteto-mode/SKILL.md:28` | names the source runtime: - Any PR-status request → the **Babysit** playbook (`playbooks/babysit.md`), and not Cursor's built-in babysit skill, whose description matches the same words. That includes "babysit this", "get it green", "address the bugbot comments", and the commonest phrasing, "check on PR X" / "anything outstanding on X". Never triggered by merely opening a PR. Declare its mode before polling; the playbook's step 1 owns the request-to-mode mapping. Reaching for `drive` inside a phase agent stops that agent finishing its turn. |
| `skills/poteto-mode/SKILL.md:134` | names the source runtime: - **Pause safely.** Suspending in-flight work cleanly so it can be resumed, on an explicit pause, going offline, a Cursor restart, or imminent context compaction. The complement to Session pickup. Full steps: `playbooks/pause-safely.md`. |
| `skills/poteto-mode/playbooks/authoring-a-skill.md:5` | names the source runtime: 1. Use the **create-skill** skill (Cursor's built-in for authoring SKILL.md files). |
| `skills/poteto-mode/playbooks/autonomous-run.md:6` | names the source runtime: 2. Pick the wake mechanism using Cursor's `/loop` command (a built-in, not a pstack skill). An event to watch (CI, a merge, a ref advancing) gets a watcher subagent that wakes you on the event, with a long time-based heartbeat as fallback. No event gets a fixed-interval heartbeat sized to when the result is worth re-checking. |
| `skills/poteto-mode/playbooks/autopilot-full.md:6` | names the source runtime: 2. **Spawn one owner per PR with the full lifecycle.** One Cursor cloud agent per PR owns build, gt registration, self-proof on the real artifact (the **prove-it-works** principle skill), skeptical Bugbot triage per `../references/bugbot-triage.md`, a slop-strip (the `deslop` skill from the `cursor-team-kit` plugin (`/deslop`)), `/no-comments` (the **no-comments** skill), a restack onto current trunk, the babysit loop to green (`playbooks/babysit.md`), and the merge itself. The restack always precedes babysit and never waits for drift or conflicts. Every owner keeps a decisions.tsv trail per the **show-me-your-work** skill, never committed, returned with its reports. The merge is the one step an owner may not take alone; step 4 gates it. |
| `skills/poteto-mode/playbooks/autopilot-stack.md:5` | names the source runtime: 1. **Run the owner loop unchanged.** One Cursor cloud agent per PR owns its change end to end: build, `gt` registration of its own PR, self-proof (gates, CI, receipts), skeptical Bugbot triage per `../references/bugbot-triage.md`, a slop-strip (the `deslop` skill from the `cursor-team-kit` plugin (`/deslop`)), `/no-comments` (the **no-comments** skill), and babysit to green per `playbooks/babysit.md`. Owners parallelize when the work is self-contained. Every owner keeps a `decisions.tsv` trail per the **show-me-your-work** skill, never committed, returned in its report. |
| `skills/poteto-mode/playbooks/babysit.md:3` | names the source runtime: **You own the merge frontier. Declare a mode, clear one PR at a time, stop where the human's call begins.** For "babysit this", "get it green", "all green", "merge-ready", "watch CI", "address the bugbot comments", or "check on PR X". Step 1 owns the request-to-mode mapping. This playbook replaces Cursor's built-in babysit skill for these requests, so do not route there even though its description matches the same words. A request to land or ship is `playbooks/shipping.md`, which begins where this playbook ends. |
| `skills/poteto-mode/playbooks/bug-fix.md:8` | names the source runtime: 2. Binary-search the cause. Form the candidate hypotheses, then rule them out until one survives. Seed them with `how` over the affected subsystem and the **why** skill for regression history. Each pass, take the split that cuts the most remaining problem space, get runtime evidence, eliminate. When program state is unclear, add instrumentation or logging and read it as the code runs. Don't guess. Drive a long or stubborn hunt with Cursor's `/loop` command. Confirm the surviving *mechanism* with runtime evidence before the step-3 architect/interrogate fan-out; a design grounded on a plausible-but-unconfirmed cause can be unanimously wrong while the real cause sits one subsystem over. |
| `skills/poteto-mode/playbooks/opening-a-pr.md:9` | names the source runtime: **PRs.** `/deslop` the diff before commit; `/no-comments` the diff before review; apply the **unslop** skill to the PR description and commit bodies. Small PRs, 5 narrow over 1 fat; stack follow-ups, branch off main only for genuinely independent work. For stacked PRs, use whatever stacking tool your team uses; the principle is small, ordered slices with the stack visible to reviewers. `gh pr view <number>` before referencing PR status. Rebase on `main` before substantial stack work. No `## Summary` / `## Test plan` boilerplate on small PRs; commit bodies don't restate the subject. After opening, run Cursor's built-in **babysit** skill; push back when feedback drifts from intent. |
| `skills/poteto-mode/playbooks/orchestrate.md:97` | names the source runtime: - Never resume an agent to check on it; a resume restarts an idle agent. Probe read-only: the ledger, `units.tsv`, `gh`, pushed branches, the cloud agent's status in the Cursor dashboard. Transcript mtime is not liveness. |
| `skills/poteto-mode/playbooks/orchestrate.md:103` | names the source runtime: - After a Cursor restart: local agents are dead, cloud work is not. Re-read the standing orders and `units.tsv`, recompute the frontier, reattach cloud work by PR and branch rather than agent id, respawn one sub-coordinator per track from its stored brief plus current state, drain, resume. The dead session's store lock clears itself on the next write; `orch` replaces a lock whose holder pid is gone. |
| `skills/poteto-mode/playbooks/pause-safely.md:3` | names the source runtime: **You own a clean stop. Leave a checkpoint a cold-start agent can resume from.** For "pause safely", "I need to go offline", "restart Cursor", or "board my flight", and when context is about to compact or summarize. This is explicit only. On "keep going", "going to bed, keep going", or "don't stop", do not pause. Those mean continue, and Autonomous run already checkpoints per iteration. |
| `skills/poteto-mode/playbooks/shipping.md:7` | names the source runtime: 1. **Verify every PR independently before arming anything.** One subagent per PR, not batched, each a Cursor cloud agent, each exercising the real surface (`control-ui` or `control-cli` from `cursor-team-kit` as the change demands) against parent versus head. Each returns `PASS`, `PASS+NOTES` or `FAIL` and posts that verdict on its own PR so the record outlives the chat. Safe means a verdict from an agent that did not write the code. CI green is not a verdict, and an approving bot review is not a verdict. |
| `skills/poteto-mode/playbooks/worktree-cleanup.md:10` | names the source runtime: 6. Simulators and other reclaimers. Simulators are usually the next-biggest win. `xcrun simctl --set testing delete all` (XCTestDevices clones), `xcrun simctl delete unavailable`, and `xcrun simctl runtime list` then `runtime delete <id>` for old runtimes. More when needed: Xcode `DerivedData` and `iOS DeviceSupport`; `~/Library/Application Support/Cursor` (`state.vscdb.backup`, and `snapshots/roots/<root>` where a `<root>` named for a folder you opened as a workspace balloons); package caches (pnpm, uv, brew, yarn). Clear only caches the user has not said to keep. |
| `skills/poteto-mode/references/plan.md:76` | names the source runtime: If a phase creates or edits a skill, the phase instructs the implementer to use the **create-skill** skill (Cursor's built-in for authoring SKILL.md files). |
| `skills/poteto-mode/references/plan.md:101` | names the source runtime: - Cursor's built-in **babysit** skill after opening the PR. |
| `skills/reflect/SKILL.md:65` | names the source runtime: - Substantive existing-skill edit (a new section, a new pattern table, more than ~10 lines): hand to Cursor's built-in `create-skill` skill and run its draft / test / iterate loop. |
| `skills/setup-pstack/SKILL.md:15` | names the source runtime: Enumerate the model slugs you can pass to a `task` subagent in this session; that is the dependable source. If Cursor also exposes a models API or CLI that lists the user's entitled models, prefer it for completeness. If you cannot detect any, ask the user to paste the slugs they have access to. Never write a real slug you have not confirmed is available. The aliases `inherit-parent` and `auto` are always valid even though they are not detected slugs. |
| `skills/why/SKILL.md:101` | names the source runtime: Before spawning investigators, list the available MCPs from the Cursor environment. Use the available-tools map when present. Otherwise inspect the `mcps/` directory Cursor exposes for enabled MCP servers. |

## Fidelity

One row per feature the converter decided on.

| Fidelity | Features | Meaning |
| --- | --- | --- |
| exact | 165 | behaves the same in Copilot CLI |
| approximated | 7 | converted, with a known difference noted in manifest.json |
| unsupported | 5 | no Copilot equivalent; dropped or not converted |
| unverified | 0 | converted to a Copilot feature whose behaviour no primary source confirms |
