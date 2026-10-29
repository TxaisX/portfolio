# Kolux

**Personal project** · Sept 2026 – present · v0.15.4 (Oct 2026) · [Installers](https://github.com/TxaisX/kolux-releases) (source is private)

## The problem

AI coding agents (Claude Code, Codex, Gemini CLI and others) are most useful when several run at once, each on its own task. Run them in the same folder, though, and they overwrite each other's work. Juggling a terminal per agent also makes it hard to see which one is waiting on you.

## What I built

A Windows desktop app that puts a whole team of agents in one window:

| Area | What the user gets |
|---|---|
| Isolated sessions | Each agent works in its own copy of the project (a git worktree), so parallel agents never collide |
| Launching | A menu of the agents actually installed on the PC; one click opens a preset team (Solo, Pair, Workbench, Swarm) with a role for each |
| Live status | Each agent shows as working, waiting on you, or done, with a notification when one finishes |
| Orchestration | A command-line tool that lets one agent start workers and pass messages between them |
| Automations | Prompts that run on a schedule or when an event happens |
| Plan review | When an agent proposes a plan, you comment on it section by section, then approve it or send it back |
| Also built in | Terminals, an editor, a browser, diff review, dictation, session resume after restart, automatic updates |

Kolux bundles no AI models or keys. It launches the tools the user already pays for.

## How I built it

I planned it, wrote the specs and acceptance checks, and directed AI agents to write the code, often several at a time inside Kolux itself. I tested every release on my own machine and shipped through numbered versions with installers and an auto-update feed.

## What I learned

- **The bottleneck was the machine, not the app.** When several agents ran their test suites at once, RAM and CPU maxed out. Capping test workers fixed it. The lesson was to measure before blaming the code.
