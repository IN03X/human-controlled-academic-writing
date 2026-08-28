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

When paragraph or section structure is disputed, show the concrete rhetorical
path before polished prose. Use a sequence such as A -> B -> C -> D in which
each step names the idea introduced and how it leads to the next. Diagnosis or
an allowed-content list alone is not a revision direction.

## Advisor Comments

Turn advisor feedback into a small action list before revising. Separate
claim/structure/prose issues from figure/data/code issues so that an artifact
problem is not disguised as a text-only fix. For consequential changes, propose
the smallest coherent batch with before/after text or a paragraph contract and
wait for approval. Low-risk edits inside accepted meaning still follow the
decision boundary above.

For "the main line is unclear", inspect section responsibilities, paragraph claims, and contribution statements. Do not add a slogan. Separate the primary contribution from downstream uses. When a dataset is primary, benchmarks or models should remain downstream uses unless the human promotes them to co-primary contributions.

For "sentences are too long", split by semantic relation rather than punctuation. Preserve compact technical definitions and formulas.

For "too detailed" or "put this in the main text", preserve useful technical
content but move it to the section where readers need it: problem and value in
the introduction, input-output definitions in the system description, data and
hyperparameters in experimental setup, and metrics and outcomes in results.
Replace premature internals with a compact statement of the component's input,
output, and purpose. Do not add words solely to make a section longer.

## Related Work

- Each paragraph must serve one local comparison or coverage claim.
- Name only the cited work's object, variable, method, or output needed for that claim.
- Do not summarize every feature of a related paper.
- End with a specific coverage boundary when one is supported; do not repeatedly advertise the current work.

## Required Output

Deliver the revised manuscript content or a concrete proposed direction, depending on the approval boundary. Keep process commentary outside manuscript prose.

## Stop Conditions

Stop when the local claim is unknown, evidence cannot support the intended wording, or preserving the user's meaning conflicts with the requested edit.
