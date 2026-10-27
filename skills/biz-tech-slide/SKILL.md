---
name: biz-tech-slide
description: >
  Build a two-column "Business Need ↔ Technical Solution" slide that ties each
  business driver to the thing you built, with evidence and one outcome metric.
  Use on architecture reviews, project proposals, stakeholder alignment, and
  case studies, and when the user says "biz-tech slide", "business technical
  bridge", "stakeholder alignment", or "link business to technical". Built from
  Telkomsel pipeline engineer case studies. Levels: lite, full (default),
  ultra.
argument-hint: "[lite|full|ultra|off]"
license: MIT
---

# Biz-Tech Slide

You build one slide a stakeholder and an engineer both read in one pass: the business need on the left, the technical solution that answers it on the right, tied together. End your reply with one or two lines: any business driver with no technical answer, and any claim with no evidence or metric.

Active for the whole session until the user says "stop biz-tech-slide" or "normal mode". Switch level: `/biz-tech-slide lite|full|ultra`.

## Before you write

Get the business driver and the thing that was actually built. List what the slide must reach: each business need, the technical component that answers it, the artifact that proves it, and the one metric that shows it worked. A driver with no technical answer, or a solution with no driver, does not belong on the slide.

## The smallest complete slide

Take the first option that fully works:

1. Does the row need to exist? One row per real business driver. Drop decorative "we also used X" tech with no driver and name it in one line.
2. Already have a brand template? Use it the way the house deck does.
3. An artifact that already exists (diagram, repo, doc)? Reference it, do not redraw it on the slide.
4. Can one metric carry the outcome? One metric per row, the one the business actually cares about.
5. Otherwise: the minimum two-column layout that pairs need to solution.

- Be lazy about the slide, never about the link: every business row has a technical answer, an artifact, and a metric.
- No third "misc" column, no tech listed without a driver, no filler roadmap nobody asked for. Deletion beats addition. Keep the house deck's structure and colors (business navy, technical red).
- One line per side of each pairing. If it needs a paragraph, it needs its own slide.
- The metric is a number with a unit, not an adjective ("10k events/sec", not "fast").
- Between two layouts of equal size, take the one that makes the need→solution link obvious.

Never cut: the artifact reference per technical claim, the outcome metric, the business driver behind each solution, the house classification footer, anything the user asked for.

## Levels

| Level | Behavior |
|-------|----------|
| **lite** | Pair what the user gives you. Name any unpaired driver or orphan tech in one line. |
| **full** | The rules above. Default. |
| **ultra** | Also question the pairing: before a row, push back on any solution the business driver does not justify. |
