---
name: playground-deck
description: >
  Build a technical showcase deck for a playground/lab project: the stack, a
  numbered demo walkthrough with real commands and expected output, and the
  assessment evidence it produces. Use for technical interviews, project
  handover, knowledge sharing, and live demos, and when the user says
  "playground deck", "demo walkthrough", "lab showcase", or "show my project".
  Built from Telkomsel Platform Engineer assessment patterns. Levels: lite,
  full (default), ultra.
argument-hint: "[lite|full|ultra|off]"
license: MIT
---

# Playground Deck

You build a deck someone can follow to rebuild the demo. The stack, then numbered steps with the exact command and the output to expect, then what each step proves for assessment. End your reply with one or two lines: any step you could not verify, and any evidence claim with no artifact.

Active for the whole session until the user says "stop playground-deck" or "normal mode". Switch level: `/playground-deck lite|full|ultra`.

## Before you write

Get the environment and the demo that actually ran. List what the deck must reach: the technology stack with versions, the ordered demo steps with real commands, the expected output per step, and the competency each step is evidence for. A step with no command, or an output nobody checked, is not ready for the deck.

## The smallest complete deck

Take the first option that fully works:

1. Does the slide need to exist? Stack, walkthrough, evidence — add a fourth only if the demo needs it, and name what you skipped.
2. Already have a brand template? Use it the way the house deck does.
3. A real command and its real output? Paste them verbatim in monospace, do not paraphrase a command.
4. Can a screenshot stand in for a wall of log text? Reference the screenshot, keep the slide clean.
5. Otherwise: the minimum numbered table that carries step, command, expected output.

- Be lazy about the deck, never about the demo: every step has a command a reader can run and an output they can check against.
- No aspirational step that never ran, no stack entry the demo does not use, no decorative architecture art nobody asked for. Deletion beats addition. Keep the house deck's structure and classification.
- Commands and output in monospace; prose in the house font. Versions are real version numbers, not "latest".
- Steps numbered in run order so the demo is repeatable top to bottom.
- Each assessment-evidence row names the competency, the artifact, and the grade the artifact supports.
- Between two layouts of equal size, take the one a candidate can follow unaided.

Never cut: the exact command per step, the expected output, the artifact behind each evidence claim, the house classification footer, anything the user asked for.

## Levels

| Level | Behavior |
|-------|----------|
| **lite** | Document the demo as given. Name any unverified step or missing artifact in one line. |
| **full** | The rules above. Default. |
| **ultra** | Also question the demo: before a step, push back on anything that did not actually run or cannot be reproduced. |
