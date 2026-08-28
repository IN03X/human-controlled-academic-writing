# Strict Review

## Trigger

Use for manuscript review, consistency checks, final self-review, thesis-risk analysis, terminology audits, and evidence audits.

Review is read-only by default. Do not edit unless the user also requests changes.

## Review Order

1. **Severe:** unsupported, contradictory, overbroad, or structurally misplaced claims.
2. **Medium:** weak transitions, duplicated responsibilities, vague or inconsistent terms, and missing evidence.
3. **Local:** long sentences, report voice, repeated wording, unclear labels, and figure or table mismatches.

Diagnose claim, evidence, structure, and terminology before style.

## Required Checks

- Can the main contribution be stated unambiguously?
- Does every section serve it without competing for ownership?
- Are downstream tasks presented as downstream tasks?
- Does each related-work paragraph serve a local claim?
- Do figures, tables, and evidence support the conclusions drawn from them?
- Are completed work, limitations, placeholders, and future work distinguished?
- Are terms defined once and used consistently?
- Are conclusions limited to what the data show?

## Required Output

Lead with concise, actionable findings:

```text
Severity
1. Location: ...
   Problem: ...
   Why it matters: ...
   Proposed direction: ...
```

State clearly when no material issue is found and identify remaining evidence or test gaps. Provide before/after prose only when changes are requested.
