# Compression Patterns

## Prompt
before: "Explain step by step how to implement a Python function that reads a file and counts words."
after: `python: read file → count words`

## Code
before:
def count_words(file_path):
    with open(file_path, 'r') as f:
        text = f.read()
    words = text.split()
    return len(words)

after:
def count_words(p):
    with open(p) as f: return len(f.read().split())

note: inline open() without context manager leaks file handles — always preserve `with`

## Instruction
before: "Analyze carefully and produce a detailed structured answer."
after: `analyze → respond`

## Structure
before: Step 1 init / Step 2 process / Step 3 return
after: init → process → return
