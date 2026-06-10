# Evidence Gate

Use this file when checking literature, claims, citations, data claims, or implementation claims.

## Evidence Grades

- **A: Direct support**  
  The source directly supports the exact claim.
- **B: Partial support**  
  The source supports a narrower or adjacent claim. The prose must be careful.
- **C: Background only**  
  The source gives context but should not be used as proof.
- **D: Reject**  
  The source is irrelevant, contradictory, too vague, or only found through a weak summary.

Only A and carefully worded B evidence should enter manuscript claims.

## Literature Checks

For every important citation:

- What exact sentence will it support?
- Is the cited source high relevance?
- Did the agent inspect enough of the source to avoid summary drift?
- Is the wording narrower than the evidence?

If a search tool returns a vague answer, re-query. If still vague, inspect the paper. If the paper cannot support the claim, reject the citation or weaken the claim.

## Implementation Checks

For data/code/figure claims:

- Does the artifact exist?
- Does the file or script produce the stated output?
- Are figure labels, units, and captions consistent with the text?
- Is the result final, placeholder, or future work?
- Does the manuscript distinguish completed work from planned work?

Do not write "the framework supports X" unless the current artifact actually supports X. If only an interface exists, say that an interface is provided.

