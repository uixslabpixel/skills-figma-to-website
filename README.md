# uix

Claude Code skills for UI/UX → code workflows.

## Skills

| Skill | What it does |
|---|---|
| [`figma-to-website`](skills/figma-to-website/SKILL.md) | Turns a Figma website design into a running, responsive prototype (localhost or Claude artifact). Desktop-first with human checkpoints, placeholder-first layout, semantic renaming of messy Figma layers, a Figma-vs-normalized typescale switch (`Cmd + \`), and token-budget rules. |

## Install

Requires [Claude Code](https://claude.com/claude-code) and the Figma MCP server.

Personal (all projects):

```bash
git clone https://github.com/vickyfikri90-cloud/uix.git
mkdir -p ~/.claude/skills && cp -R uix/skills/figma-to-website ~/.claude/skills/
```

Per project: copy `skills/figma-to-website` into your project's `.claude/skills/`.

## Use

In Claude Code, share a Figma link and ask for a website prototype, e.g.:

> Build this as a website on localhost: https://www.figma.com/design/...

The skill walks through: plan → ⛔ plan OK → desktop layout with placeholders → ⛔ layout confirmed → assets & polish → ⛔ desktop confirmed → mobile/tablet → final QA.

