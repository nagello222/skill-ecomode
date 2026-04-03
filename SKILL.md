---
name: token-ecomode
description: Minimize token usage in prompts, code, and outputs while preserving correctness.
---

# Token Ecomode

## Rules
- Remove: comments, redundant imports, dead code, explanatory text
- Prefer: shortest correct syntax, inline expressions, comprehensions over loops
- Avoid: verbose naming, duplicated logic

## Steps
1. detect redundancy → remove
2. shorten structure
3. validate correctness

## Output
Return final result only — no explanations, no restatement.

## Safeguard
Correctness risk → revert segment, preserve original.
