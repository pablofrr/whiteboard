# whiteboard

A skill for coding agents: after finishing a task, it asks you whiteboard-style
questions about the code and logic to make sure you understand it and could explain it.

## Install

```sh
npx skills add pablofrr/whiteboard
```

Works with any agent that supports `SKILL.md` (Claude Code, Codex, Cursor, Gemini CLI…).
Use `-a <agent>` to target a specific agent and `-g` to install globally.

## Usage

When a task is done, ask your agent: "whiteboard me".

## Diagrams as images (optional)

The interview sketches flows as ASCII diagrams. In Claude Code on Ghostty or kitty,
install [mermaid-render](https://github.com/pablofrr/mermaid-render) to see them as
rendered Mermaid images instead.
