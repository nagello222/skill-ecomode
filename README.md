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

## Reference

This skill is informed by the findings of:

> Gao, Y., Li, Z., Yuan, Y., Ji, Z., Ma, P., & Wang, S. (2026).
> **SkillReducer: Optimizing LLM Agent Skills for Token Efficiency.**
> *arXiv:2603.29919v1* — [https://arxiv.org/abs/2603.29919](https://arxiv.org/abs/2603.29919)

Key findings applied here: 60%+ of skill body content is non-actionable; removing it reduces attention dilution and improves functional quality by 2.8% (less-is-more effect).
