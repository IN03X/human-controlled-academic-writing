# Stage Router

Use this file first. Its job is to keep the active context small.

## Step 1. Classify The Current Stage

Choose one primary stage:

1. **early-writing**  
   Topic discovery, contribution alignment, novelty checking, outline design, or first chapter planning.

2. **outline-contract**  
   Turning an accepted outline into chapter contracts or paragraph contracts before drafting.

3. **mid-refinement**  
   Revising existing manuscript text, handling advisor comments, improving transitions, tightening cited paragraphs, or preserving the user's intended claim while improving wording.

4. **strict-review**  
   Harsh review, consistency check, thesis risk review, terminology audit, evidence audit, or final paper self-check.

5. **implementation-sync**  
   Checking whether manuscript claims match data, scripts, figures, tables, generated outputs, paths, or experiment status.

## Step 2. Read One Card

- early-writing -> `early-writing-card.md`
- outline-contract -> `outline-contract-card.md`
- mid-refinement -> `mid-refinement-card.md`
- strict-review -> `strict-review-card.md`
- implementation-sync -> use `strict-review-card.md` plus the implementation checks in `evidence-gate.md`

## Step 3. State The Stage

Begin with one short working note:

> Current stage: mid-refinement. Goal: align the advisor's comment before editing.

If the user says "do not edit yet", "think first", "show before/after", "I am not sure", or rejects an edit, stay in alignment mode. Do not edit the manuscript until a small target is accepted.

