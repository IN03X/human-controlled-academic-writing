# Human-Controlled Academic Writing

A reusable Codex skill for writing academic papers under human control.

This repository packages a writing workflow developed through a real thesis-writing process. Its goal is not to let an agent write a paper autonomously. The goal is to make the agent a careful research partner: it asks questions, checks evidence, drafts only after alignment, reviews harshly, and revises only after the human accepts a concrete plan.

## What This Workflow Emphasizes

- The human controls the thesis, contribution, scope, and final judgment.
- The agent must know the current section's claim before writing.
- Literature paragraphs must serve a specific argument, not become broad summaries.
- Evidence must be checked before it enters manuscript prose.
- Drafting, refinement, and review use different rules.
- Long rule sets are split into stage cards so the agent loads only what it needs.

## Repository Layout

```text
skill/
  human-controlled-academic-writing/
    SKILL.md
    references/
      stage-router.md
      early-writing-card.md
      outline-contract-card.md
      mid-refinement-card.md
      strict-review-card.md
      evidence-gate.md
      paragraph-contract.md
      prose-style-gates.md
      examples-good-bad.md
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

For each new paper project, copy the files under `templates/` into the project workspace and fill them gradually. The templates are intentionally lightweight; the useful part is the discipline of keeping decisions, evidence, and paragraph contracts visible.

## Core Rule

Before writing a sentence, the agent must know the local claim that sentence serves. If the claim is unknown, it must find the chapter or paragraph contract. If no contract exists, it must ask the human or create a proposed contract before drafting.

## Attribution

This workflow was adapted from project-specific writing protocols and from useful ideas in Imbad0202/academic-research-skills, especially Socratic planning, corpus-first screening, evidence gates, and review loops. The resulting workflow has been rewritten for a human-controlled, corpus-grounded paper-writing process.

