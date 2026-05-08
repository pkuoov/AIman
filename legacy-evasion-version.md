---
name: legacy-evasion-version
description: "Non-operational archive note for the removed detector-evasion draft. This file is for comparison and risk review only; it must not be used as a skill."
---

# Legacy Evasion Version

This file intentionally does not preserve the earlier detector-evasion workflow
as executable skill instructions.

The removed draft framed the task as bypassing AI-detection tools and included
operational guidance for manipulating detector-facing signals and fabricating
human-looking artifacts. That framing is not suitable for a reusable skill
because it can encourage misrepresentation, fake authorship evidence, and lower
quality code or writing.

## What To Compare Instead

For experiments, compare outputs from the current `SKILL.md` against an
unreviewed AI-assisted draft using quality-centered criteria:

- Does the revised prose include the user's real viewpoint, context, examples,
  and source-backed claims?
- Are unsupported claims flagged or corrected?
- Is generic phrasing removed because it weakens the writing?
- Does the code follow the surrounding project's conventions?
- Were unnecessary abstractions, comments, or defensive branches removed?
- Are tests, review notes, or rationale added where they are genuinely useful?

## Safe Experiment Template

Use the same input draft twice:

1. Baseline: the original AI-assisted draft.
2. Revised: output produced with `SKILL.md`.

Then evaluate:

- Accuracy
- Specificity
- Author voice
- Maintainability
- Evidence quality
- Reviewability
- Compliance with the relevant school, workplace, publisher, or platform rules

Do not optimize the output against detector scores. If a detector flags genuine
human-edited work, treat that as a false-positive documentation problem: preserve
drafts, source notes, edit history, tests, and review rationale.
