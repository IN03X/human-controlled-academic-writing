---
name: human-controlled-academic-writing
description: Use for human-controlled academic paper or 论文 planning, drafting, revision, review, and LaTeX/Overleaf synchronization. Trigger on manuscripts, related work, advisor comments, citations, academic prose, paper evidence, LaTeX, or Overleaf; not generic writing or generic file synchronization.
metadata:
  version: "0.3.0"
  source_attribution: "Adapted from project writing protocols and ideas from Imbad0202/academic-research-skills for a human-controlled academic writing workflow."
---

# Human-Controlled Academic Writing

Use this skill as a decision system for academic paper work. The human owns the paper's argument and final judgment; the agent helps plan, draft, verify, revise, and review without silently changing that argument.

## Start

Before substantive paper work, read `references/task-router.md`. Select one primary writing mode and every cross-cutting gate that matches the request, then read only those files.

Do not narrate the classification unless it exposes an ambiguity, a risk, or a decision the user must approve.

## Core Invariants

1. The human controls the thesis, contribution, scope, and final judgment.
2. Every section and paragraph must serve a known local claim and reader takeaway. If either is unclear, propose it before drafting.
3. Language strength must not exceed the supporting literature, data, code, figures, or experiment status. Distinguish completed, placeholder, and planned work.
4. Preserve accepted meaning. Manuscript prose must be compact, concrete, reader-facing, and free of agent or workflow narration.
5. Paper synchronization is a separate authorization boundary. Work locally by default; pull or push only when the user explicitly authorizes that direction.

## Approval Boundary

- Propose a concrete change and wait for approval before changing the thesis, contribution, scope, section responsibility, accepted claim, evidence meaning, or conclusion.
- Directly perform wording, formatting, and local clarity edits when they stay inside an accepted meaning. Show the result and identify any residual uncertainty.
- If the edit may cross that boundary, stop and ask. Requests such as "think first", "do not edit yet", or "show me the direction" always remain in alignment mode.

## Project Artifacts

Do not create workflow files by default. Create or update only the artifact required by the selected mode, and only when it improves the current task or the user requests persistent project state.

