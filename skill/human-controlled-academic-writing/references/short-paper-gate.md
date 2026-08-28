# Short Paper Gate

## Trigger

Load for a short conference, challenge, system, or technical paper, typically
about 3--4 pages, or when the human, venue, or advisor explicitly asks for a
compact paper structure, four-part introduction, or advisor-ready check. Do not
load merely because a document is academic. Venue requirements and an accepted
human outline override the defaults below.

## Reader-Facing Structure

Treat the paper as a compact argument rather than a project chronology. Every
section must earn its space by advancing the reader's understanding or the
paper's evidence.

- **Abstract:** When 150--200 words are available, use a compressed
  problem--gap--method--evidence flow. Name the main system idea, the main
  measured result, and at most one submission or post-processing constraint
  needed to interpret that result. Do not turn the abstract into a module list.
- **Introduction:** Cover four movements in this order:
  1. define the focal problem or concept, its value, and its application context
     for a non-specialist reader;
  2. summarize the most relevant prior work and what it already provides;
  3. state the remaining gap or challenge in two or three concrete points;
  4. state the paper's system and contributions in two or three concrete points.
- **System or method:** Define each module by its input, output, role, and
  connection to other modules before internal architecture details.
- **Experimental setup and results:** Place data, settings, metrics, export
  rules, compression or submission constraints, and result tables where their
  relationship is easiest to verify.
- **Conclusion:** Restate only the system and the most important measured result
  or limitation.

When a four-paragraph introduction is requested, assign one movement to each
paragraph. Otherwise the four movements are the default rhetorical sequence,
not an absolute paragraph count. Within the first movement, define the focal
task or concept before explaining why it is difficult.

## Placement Rules

- Keep dataset construction, implementation history, failed attempts,
  hyperparameter lists, and low-level output-format details out of the
  introduction unless readers need them to understand the contribution.

## Advisor-Ready Check

Before calling the paper ready for advisor review, check that:

- the abstract follows a reader-facing problem--gap--method--evidence flow;
- the introduction contains the four movements above, begins at a
  non-specialist-readable level, and does not overload implementation details;
- related work is substantial enough for the venue, and each paragraph serves
  a local claim rather than forming a thin citation list;
- contributions are two or three concrete points whose strength does not exceed
  the reported evidence;
- method modules expose input, output, role, and connection before internals;
- data, settings, metrics, export rules, and results are organized as verifiable
  experimental evidence;
- the applicable evidence, prose, and artifact consistency gates pass.

If any item fails, report it as a finding and do not call the manuscript ready.
