# Strict Review Card

Use this card when the user asks for review, consistency checks, final polish, or thesis risk analysis.

## Review Order

Findings first. Do not start with praise.

1. Severe issues: claims that are unsupported, contradictory, overbroad, or structurally misplaced.
2. Medium issues: weak transitions, duplicated responsibilities, vague terms, inconsistent terminology, or missing evidence.
3. Local issues: long sentences, report voice, repeated words, unclear labels, table/figure mismatch.

## Review Questions

- What is the paper's main contribution?
- Does every chapter serve that contribution?
- Are downstream tasks presented as downstream tasks, or do they compete with the main line?
- Does each related-work paragraph have a local claim?
- Do figures and tables support the conclusions drawn from them?
- Are limitations honest without turning the paper into a progress report?
- Are terms defined once and used consistently?
- Are conclusions limited to what the data show?

## Output Format

Use concise, actionable findings:

```text
Severe
1. Location: ...
   Problem: ...
   Why it matters: ...
   Proposed direction: ...
```

When the user wants to approve changes, provide before/after text for each proposed edit.

