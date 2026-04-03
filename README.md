# token-ecomode

A Claude Code skill that minimizes token usage in prompts, code, and outputs while preserving correctness.

## What it does

- **Prompts** — strips narrative, converts to directive blocks
- **Code** — collapses logic, inlines variables, prefers comprehensions over loops
- **Outputs** — returns final result only, no commentary

## Files

| File | Purpose |
|---|---|
| `SKILL.md` | Core rules, compression steps, output policy, safeguard |
| `examples.md` | Before/after compression patterns for prompts, code, and instructions |

## Usage

Invoke with `/token-ecomode` in Claude Code.

## Install

Copy this skill into your Claude skills directory:

```
~/.claude/skills/token-ecomode/
```
