---
name: human-controlled-academic-writing
description: Use when planning, drafting, revising, strictly reviewing, or manually synchronizing an academic paper under human control. Covers LaTeX and Overleaf paper work, including Dropbox or rclone pull/push workflows, plus evidence-gated writing with PaperQA2, Zotero, folder corpora, or manual source inspection.
metadata:
  version: "0.2.0"
  source_attribution: "Adapted from project writing protocols and ideas from Imbad0202/academic-research-skills for a human-controlled academic writing workflow."
---

# Human-Controlled Academic Writing

This skill is for slow, human-controlled academic paper writing. The agent is not an autopilot. It is a research partner that asks questions, checks evidence, drafts only after alignment, reviews harshly, and revises only after the human accepts a concrete plan.

## First Step

Open `references/stage-router.md` before acting. Classify the current stage and read only the card named by the router.

Do not load all references by default. The workflow relies on progressive disclosure so the active rules stay small enough to follow.

If the paper uses LaTeX, Overleaf, Dropbox, rclone, or separate local and synchronized copies, also open `references/manual-overleaf-sync.md` before editing or synchronizing files.

## Non-Negotiable Rules

1. The human controls the thesis, contribution, scope, and final judgment.
2. Do not draft unless the current section or paragraph claim is known.
3. If no claim or contract exists, create a proposed contract or ask the human before writing.
4. Literature writing must serve a local argument. Do not summarize papers just because they are related.
5. Weak evidence cannot become strong prose. Re-query, inspect the source, weaken the claim, or reject the evidence.
6. Preserve the user's intended meaning. Improve wording and logic, but do not delete a core claim the user explicitly wants.
7. Academic prose must be compact. Remove filler, report-like narration, inflated wording, and multi-center long sentences.
8. Manuscript prose addresses readers as authors. Do not expose the agent's thinking process or evidence-management workflow.
9. Strict review comes before polishing. Diagnose claim, evidence, structure, and terminology problems before touching style.
10. Implementation claims must match actual data, scripts, figures, tables, and experiment status.
11. Paper synchronization is a separate, manually authorized boundary. Work in the local copy by default; do not pull from or push to an Overleaf, Dropbox, or rclone sync location without explicit user instruction.

## Reference Map

- Topic discovery, novelty stress test, first structure: `references/early-writing-card.md`
- Chapter and paragraph contracts: `references/outline-contract-card.md`
- Advisor comments, sentence-level refinement, paragraph repair: `references/mid-refinement-card.md`
- Harsh manuscript review and consistency audit: `references/strict-review-card.md`
- Evidence grading and citation use: `references/evidence-gate.md`
- Paragraph contract schema: `references/paragraph-contract.md`
- Chinese/English prose gates: `references/prose-style-gates.md`
- Positive and negative examples: `references/examples-good-bad.md`
- Local-first Overleaf, Dropbox, and rclone pull/push safeguards: `references/manual-overleaf-sync.md`

## Working Files

For a paper project, keep lightweight working files in the project workspace:

- `project_passport.yaml`
- `decision_log.md`
- `novelty_matrix.md`
- `outline_contract.md`
- `chapter_contract.md`
- `paragraph_contract.md`
- `claim_evidence_table.yaml`
- `rejected_evidence_log.md`

Templates live outside the skill in this repository's `templates/` directory.

