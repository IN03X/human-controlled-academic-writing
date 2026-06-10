# PaperQA2 Integration

Use PaperQA2 as an evidence gate, not as an author.

## Query Pattern

Ask questions that can fail:

- Which papers in this corpus already do `<claim>`?
- Does any paper directly support this sentence: `<sentence>`?
- What is the strongest counterexample to `<novelty claim>`?
- For `<paper title>`, what exact result supports `<specific relation>`?

## Evidence Use

If PaperQA2 returns vague or partial support:

1. Re-query with a more specific question.
2. Inspect the original paper when available.
3. Grade the evidence.
4. Weaken or reject the manuscript claim if support remains weak.

## Wrapper Example

Adapt command names to your local wrapper:

```powershell
.\paperqa2.ps1 -Command ask -Index <index> -Question "<question>"
.\paperqa2.ps1 -Command search -Index <index> -Question "<query>"
```

