---
name: humanize-ai-content
description: "Use when revising AI-assisted code or prose to improve originality, author voice, factual grounding, maintainability, and reviewability. This skill helps reduce false positives from AI-detection tools by strengthening real human authorship signals, not by bypassing detectors or misrepresenting authorship."
---

# Humanize AI-Assisted Content

This skill revises AI-assisted writing and code so the final work is more accurate,
specific, maintainable, and clearly owned by the author. It must not be used to
evade AI-detection tools, fabricate authorship, hide prohibited assistance, or
optimize against a detector's scoring model.

AI detectors can produce false positives, especially on polished, formulaic, or
highly standardized work. The right response is to make the work more genuinely
grounded in the user's intent, evidence, context, and revision process.

## Boundaries

Do:

- Improve clarity, specificity, factual accuracy, structure, and voice.
- Ask for or incorporate the user's real notes, constraints, examples, drafts,
  sources, decisions, and domain context.
- Preserve or recommend transparent disclosure when a policy, school, employer,
  publisher, or platform requires it.
- Help the user keep process evidence: outlines, drafts, source notes, tests,
  review comments, commits, and rationale.
- For code, make it idiomatic to the target project and easier to review.

Do not:

- Claim the work will be undetectable as AI-assisted.
- Tune text against AI-detector metrics such as perplexity, burstiness, or
  stylometry scores.
- Recommend fake mistakes, fake citations, fake drafts, fake commit history, or
  fake developer traces.
- Add commented-out debug code, meaningless TODOs, inconsistent names, or other
  artifacts just to look human.
- Help violate academic, workplace, hiring, publication, or platform rules.

## Workflow For Prose

1. Clarify the real authorial input.

   If the user's draft is generic, ask for missing substance when practical:
   personal stance, intended audience, lived examples, source material, course
   readings, interview notes, product details, constraints, or disagreement with
   the draft.

2. Ground the piece.

   Add concrete details that are true and relevant. Prefer specific claims,
   examples, tradeoffs, definitions, and source-backed evidence over broad
   filler. Flag unsupported claims instead of dressing them up.

3. Restore the author's voice.

   Match the user's known style or requested register. Keep natural variation
   where it follows meaning, not as a detector trick. Remove generic AI phrasing
   when it weakens the writing.

4. Improve argument quality.

   Check whether each paragraph earns its place. Strengthen topic sentences,
   add counterarguments or limitations where useful, and remove summary
   paragraphs that merely repeat the obvious.

5. Preserve transparency.

   If disclosure is expected, suggest a short, honest note such as:
   "I used AI assistance for outlining and revision, then fact-checked, edited,
   and finalized the work myself."

## Workflow For Code

1. Fit the existing codebase.

   Read nearby files before editing. Follow local naming, error handling,
   component boundaries, formatting, and test patterns. Prefer the project's
   existing helpers over new abstractions.

2. Replace generic code with context-aware code.

   Remove unnecessary abstractions, defensive branches, comments, or patterns
   that do not match the real requirements. Keep simple code simple.

3. Add real reviewability.

   Include tests for changed behavior when risk justifies it. Add comments only
   for non-obvious business rules, edge cases, performance constraints, or
   integration assumptions.

4. Keep authorship evidence honest.

   Recommend meaningful commit messages, issue links, design notes, test output,
   and review explanations. Never fabricate history or add fake debugging debris.

5. Report changes clearly.

   Summarize what changed, why it changed, and how it was verified. Mention any
   remaining uncertainty or missing test coverage.

## Output Style

When revising content, provide:

- The revised text or patch.
- A brief note on substantive improvements: clearer thesis, added evidence,
  fixed unsupported claims, aligned with project conventions, added tests, or
  improved maintainability.
- Optional disclosure language when relevant.

Avoid describing detector-evasion tactics. The goal is not to hide AI assistance;
the goal is to make the final work genuinely better, more accountable, and more
representative of the user's own thinking.
