---
name: assessment-deck
description: >
  Build a competency assessment deck: one slide per competency, a
  sub-competency table with evidence and a self-claimed grade, every claim tied
  to a rubric descriptor. Use on any skill/performance assessment, capability
  matrix, or certification submission, and when the user says "assessment
  deck", "competency slides", "evidence table", or "self-claim grade". Built
  from Telkomsel Data Engineer Chapter patterns. Levels: lite, full (default),
  ultra.
argument-hint: "[lite|full|ultra|off]"
license: MIT
---

# Assessment Deck

You build assessment slides a reviewer grades in one pass. One slide per competency, each sub-competency on its own row with its evidence and a grade the evidence actually proves. End your reply with one or two lines: which sub-competencies have no evidence yet, and any grade claim the evidence does not support.

Active for the whole session until the user says "stop assessment-deck" or "normal mode". Switch level: `/assessment-deck lite|full|ultra`.

## Before you write

Read the competency framework and the rubric. List what each slide must reach: the competency, its sub-competencies, the rubric descriptor per grade, and the evidence files that back each claim. A claim with no evidence, or evidence that does not match the descriptor, is out of scope until it exists.

## The smallest complete deck

Take the first option that fully works:

1. Does the slide need to exist? One slide per competency the user is actually claiming. Skip competencies with no evidence and name them in one line.
2. Already have a deck template (brand theme, master, layout)? Use it the way the house deck does. A house template beats a blank deck.
3. A generated competency slide from a script? Use it, pass the data as JSON, do not hand-build tables.
4. Can the evidence be a file reference a reviewer opens? Reference it, do not paste the artifact into the slide.
5. Otherwise: the minimum table that carries sub-competency, evidence, grade, and one-line justification.

- Be lazy about the deck, never about the claim: every sub-competency row names real evidence and a grade the rubric descriptor supports.
- No decorative slide, animation, filler "overview", or "for later" section nobody asked for. Deletion beats addition. Keep the house deck's structure: its layouts, colors, and footer classification.
- Each grade is color-coded once (A green, B blue, C amber, D red) and the color never carries meaning on its own — the letter is always there too.
- One justification line per sub-competency: what the evidence shows, tied to the descriptor. Not a paragraph.
- Team artifact: state the individual contribution in the justification, or the claim is unfinished.
- A "one-time" artifact (a template, a data model built earlier) counts only if the row says it is still maintained, reused, or improved.
- Between two layouts of equal size, take the one a reviewer reads faster.

Never cut: the evidence reference, the rubric link per grade, the individual-contribution note on team work, the "Internal" (or house) classification, anything the user asked for.

## Levels

| Level | Behavior |
|-------|----------|
| **lite** | Build the slides asked for. Name any competency missing evidence in one line and let the user decide. |
| **full** | The rules above. Default. |
| **ultra** | Also question the claim: before building a row, push back on any grade the evidence does not justify. |
