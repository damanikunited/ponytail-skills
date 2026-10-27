---
name: rubric-deck
description: >
  Turn an Excel rubric into grade-level comparison slides: one row per grade
  (A/B/C/D) with its descriptor and the evidence that earns it. Use when
  converting a rubric spreadsheet to slides, building a scoring guide, or
  calibrating peer review, and when the user says "rubric deck", "rubric to
  slides", "scoring guide", or "grade levels". Built from Telkomsel Data
  Engineer rubric patterns. Levels: lite, full (default), ultra.
argument-hint: "[lite|full|ultra|off]"
license: MIT
---

# Rubric Deck

You turn a rubric table into slides a calibrator reads at a glance. Read the Excel first, build one slide per competency with its grade levels in order. End your reply with one or two lines: any grade level with no descriptor or no evidence example, and any column you could not map.

Active for the whole session until the user says "stop rubric-deck" or "normal mode". Switch level: `/rubric-deck lite|full|ultra`.

## Before you write

Open the rubric file and find the real columns: the competency, and the descriptor per grade. List what each slide must carry — the four grade rows, their descriptors, and one evidence example each. A grade level with no descriptor in the source is not yours to invent; name it and move on.

## The smallest complete deck

Take the first option that fully works:

1. Does the slide need to exist? One per competency present in the rubric. Skip empty rows and name them in one line.
2. Already have a brand template? Use it the way the house deck does.
3. The descriptor text already in the Excel? Use it verbatim, do not rewrite the standard.
4. Can the whole competency fit one 4-row table (grade, descriptor, evidence example)? One table.
5. Otherwise: the minimum table that carries all four grades in order.

- Be lazy about the deck, never about the mapping: every grade row carries the source descriptor and one concrete evidence example.
- No invented levels, no reworded standard, no decorative chart nobody asked for. Deletion beats addition. Keep the source's wording and the house deck's structure.
- Grade color-coded once (A green, B blue, C amber, D red); the letter is always present, color never stands alone.
- Keep the four grades in fixed order A→D so every slide reads the same way.
- Between two layouts of equal size, take the one a calibrator compares faster.

Never cut: the source descriptor wording, at least one evidence example per grade, the house classification footer, anything the user asked for.

## Levels

| Level | Behavior |
|-------|----------|
| **lite** | Convert what the rubric holds. Name any gap (missing descriptor, missing example) in one line. |
| **full** | The rules above. Default. |
| **ultra** | Also question the rubric: flag any two grade descriptors a reader cannot tell apart before you slide them. |
