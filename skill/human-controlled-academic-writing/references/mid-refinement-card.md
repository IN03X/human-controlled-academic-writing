# Mid-Refinement Card

Use this card for advisor comments, paragraph repair, sentence tightening, and section-to-section alignment.

## Default Sequence

1. Restate the user's concern in concrete terms.
2. Identify the local claim the passage should serve.
3. Show the problem in the current text.
4. Propose a small revision target.
5. When asked, show before/after text.
6. Edit only after the user accepts the direction.

## Revision Gates

Every revised sentence must pass:

- Does it serve the local claim?
- Is it necessary for the paragraph?
- Does it use the shortest wording that preserves the information?
- Does it name the concrete object, action, variable, comparison, or result?
- Does it avoid report voice, workflow voice, and agent-thinking voice?

## Advisor Comment Handling

When the advisor says "main line is unclear":

- Do not add a slogan.
- Inspect whether section order, paragraph claims, and contribution statements make the main object obvious.
- Separate primary contribution from downstream tasks.
- If a dataset is the main contribution, downstream benchmark/modeling tasks should read as uses of the dataset, not equal co-main claims unless the human confirms otherwise.

When the advisor says "long sentences":

- Split only when a sentence combines multiple centers.
- Keep necessary technical definitions intact.
- Prefer one sentence per relation: prior work did X; it did not cover Y; the current paper addresses Z.

## Related Work Refinement

Related work should make readers understand what prior work did and what coverage remains. It should not repeatedly say "our work is different".

For each cited paragraph:

- Name the prior work's relevant object, variable, or output.
- State only the aspect needed for the local claim.
- Avoid listing every feature of the cited paper.
- End with a specific coverage boundary, not a broad self-promotion sentence.

