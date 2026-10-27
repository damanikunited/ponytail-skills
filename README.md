# Presentation Skills

Composable agent skills for building presentation decks, in the spirit of [ponytail](https://github.com/DietrichGebert/ponytail): small, adaptable, model-agnostic. Each one is a lazy senior-deck-builder — the smallest deck that fully makes the point, with every claim backed by evidence.

Built from Telkomsel Data Engineer Chapter assessment patterns, but the shape is generic: swap the brand template and competency framework for your own.

## Skills

Each skill lives in `skills/<name>/SKILL.md` and runs on its own. Activate with `/<name>`, switch depth with `lite | full | ultra`, stop with "normal mode".

- **[assessment-deck](skills/assessment-deck/SKILL.md)** — One slide per competency, a sub-competency table with evidence and a self-claimed grade tied to a rubric descriptor. For performance reviews, capability matrices, and certification submissions.
- **[rubric-deck](skills/rubric-deck/SKILL.md)** — Turn an Excel rubric into grade-level comparison slides (A/B/C/D) with descriptor and evidence example per level. For scoring guides and peer-review calibration.
- **[biz-tech-slide](skills/biz-tech-slide/SKILL.md)** — A two-column "Business Need ↔ Technical Solution" slide, each pairing backed by an artifact and one outcome metric. For architecture reviews, proposals, and stakeholder alignment.
- **[playground-deck](skills/playground-deck/SKILL.md)** — A technical showcase: the stack, a numbered demo walkthrough with real commands and expected output, and the assessment evidence it produces. For interviews, handover, and live demos.

## Levels

Every skill takes a level, same as ponytail:

| Level | Behavior |
|-------|----------|
| **lite** | Build what was asked; name the gaps and let you decide. |
| **full** | The default discipline. |
| **ultra** | Also push back on claims the evidence does not justify. |

## Install

Copy the `skills/` folder (or the individual skill folders) into your agent's skills directory. These are editable files — adapt the brand colors, template path, and competency framework to your own.

## License

MIT
