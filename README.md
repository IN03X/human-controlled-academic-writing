# Human-Controlled Academic Writing

A reusable Codex skill for writing academic papers under human control.

This repository packages a writing workflow developed through real thesis and paper work. It treats the skill as a decision system: the human controls the argument, while the agent selects the relevant writing mode and verification gates for the current task.

## What This Workflow Emphasizes

- The human controls the thesis, contribution, scope, and final judgment.
- Every section and paragraph must serve a known local claim.
- Literature paragraphs must serve a specific argument, not become broad summaries.
- Language strength cannot exceed the available evidence or implementation status.
- High-risk argument changes require approval; low-risk wording edits may proceed.
- One primary writing mode can combine with multiple evidence, prose, artifact, and synchronization gates.
- Compact conference and challenge papers can load a dedicated structure and advisor-readiness gate without imposing that format on every manuscript.

## Repository Layout

```text
skill/
  human-controlled-academic-writing/
    SKILL.md
    agents/
      openai.yaml
    references/
      task-router.md
      early-writing-card.md
      outline-contract-card.md
      draft-revise-card.md
      strict-review-card.md
      evidence-gate.md
      prose-style-gates.md
      artifact-consistency-gate.md
      short-paper-gate.md
      manual-overleaf-sync.md
      acoustics-examples.md
templates/
  project_passport.yaml
  decision_log.md
  novelty_matrix.md
  outline_contract.md
  chapter_contract.md
  paragraph_contract.md
  claim_evidence_table.yaml
  rejected_evidence_log.md
integrations/
  paperqa2.md
  folder-corpus.md
  zotero.md
examples/
  paragraph-contract/
    related-work-contract.md
```

## Using It In Another Project

Copy or symlink `skill/human-controlled-academic-writing` into your Codex skills directory, or keep this repository available and point your agent to the `SKILL.md` file.

The repository-level `templates/` directory contains optional project artifacts. Copy only the files needed for the active task; the installed skill does not create all of them by default.

## Core Rule

The human owns the thesis, contribution, scope, and final judgment. The agent may improve execution, but it must not silently change the accepted argument.

## Attribution

This workflow was adapted from project-specific writing protocols and from useful ideas in Imbad0202/academic-research-skills, especially Socratic planning, corpus-first screening, evidence gates, and review loops. The resulting workflow has been rewritten for a human-controlled, corpus-grounded paper-writing process.
