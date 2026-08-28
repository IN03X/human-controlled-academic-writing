# Draft And Revise

## Trigger

Use for manuscript drafting, advisor comments, paragraph repair, transitions, related-work revision, and sentence tightening.

## Decision Boundary

- If the requested change affects an accepted claim, contribution, section responsibility, evidence meaning, or conclusion, diagnose the issue and propose a small revision direction before editing.
- If the change stays inside accepted meaning, edit directly and verify the result.

## Actions

1. Identify the local claim and reader takeaway.
2. Diagnose what the current passage does that conflicts with them.
3. Make the smallest revision that resolves the problem.
4. Preserve the user's intended technical boundary and level of certainty.
5. Apply the evidence, prose, and artifact gates selected by the router.

Show before/after text when the user requests it or when approval is needed to expose a consequential change.

## Advisor Comments

For "the main line is unclear", inspect section responsibilities, paragraph claims, and contribution statements. Do not add a slogan. Separate the primary contribution from downstream uses. When a dataset is primary, benchmarks or models should remain downstream uses unless the human promotes them to co-primary contributions.

For "sentences are too long", split by semantic relation rather than punctuation. Preserve compact technical definitions and formulas.

## Related Work

- Each paragraph must serve one local comparison or coverage claim.
- Name only the cited work's object, variable, method, or output needed for that claim.
- Do not summarize every feature of a related paper.
- End with a specific coverage boundary when one is supported; do not repeatedly advertise the current work.

## Required Output

Deliver the revised manuscript content or a concrete proposed direction, depending on the approval boundary. Keep process commentary outside manuscript prose.

## Stop Conditions

Stop when the local claim is unknown, evidence cannot support the intended wording, or preserving the user's meaning conflicts with the requested edit.
