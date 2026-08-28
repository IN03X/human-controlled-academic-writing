# Claim And Evidence Gate

## Trigger

Load for literature search, citations, factual claims, related work, evidence audits, or any manuscript wording attributed to a source.

## Evidence Grades

- **A: Direct support.** The inspected source supports the exact claim.
- **B: Partial support.** The source supports a narrower or adjacent claim; narrow the prose accordingly.
- **C: Background only.** The source provides context but cannot prove the claim.
- **D: Reject.** The source is irrelevant, contradictory, too vague, or known only through an unreliable summary.

Only A evidence and carefully worded B evidence may support manuscript claims.

## Required Checks

For each important citation:

1. Identify the exact manuscript sentence or claim it supports.
2. Confirm that the source is directly relevant.
3. Inspect enough of the original source to avoid title, abstract, or search-summary drift.
4. Keep the wording no broader or more certain than the evidence.

If retrieval is vague, re-query or inspect the source. If support remains insufficient, weaken the claim, replace the source, or reject the citation.

## Output Rule

Do not expose internal evidence grades in manuscript prose. Report rejected or uncertain evidence to the user when it affects the requested claim.
