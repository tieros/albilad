# Boost Skill

## Purpose

Use this skill when the task is to redesign or improve an Albilad screen by combining Audit, Heuristic, and Boost component-kit insight.

## Required Reads

1. `design.md`
2. `docs/principles.md`
3. `docs/boost.md`
4. `docs/audit.md`
5. `docs/heuristic.md`

## Inputs This Skill Expects

- a target Albilad screen or flow
- access to the original Albilad DS
- access to existing Audit findings
- access to existing Heuristic findings
- access to the Commencis Boost component kit and delivered Boost precedents

## Execution Flow

1. Identify the main UI regions and component dependencies on the screen.
2. Check whether the relevant components already have Audit findings.
3. Check whether the exact screen or a similar flow already has Heuristic findings.
4. Check whether an existing Boost flow already solved a similar problem.
5. Check whether the needed solution already exists in the Boost component kit.
6. Reuse the kit component if available.
7. If reuse is not enough, extend an existing variant.
8. If extension is not enough, create a new component that still follows the kit logic.
9. If no explicit heuristic finding exists, derive one using the established heuristic method.
10. Produce the redesign while preserving Commencis visual taste.

## Non-Negotiable Rules

- Do not redesign in isolation from Audit.
- Do not redesign in isolation from Heuristic.
- Do not bypass the Boost component kit without a strong reason.
- Do not invent a new visual language.
- Do not create one-off components when an existing component or variant can solve the problem.

## Taste Rule

The redesign must inherit the tone of the delivered Boost after screens:

- refined
- orderly
- scalable
- accessible
- bank-grade
- clearly component-driven

## Component Decision Rule

Use this exact order:

1. existing Boost component
2. existing Boost variant
3. extension of existing Boost component
4. new Boost component

## Independent Operation Rule

This skill should work even if the task only starts as a screen redesign request.

If Audit or Heuristic coverage is missing, generate the minimum necessary continuity-safe reasoning internally and proceed without breaking the project method.

## Output Contract

Return:

- relevant Audit references used
- relevant Heuristic references used
- relevant Boost precedents used
- component reuse, extension, or creation decisions
- final redesign rationale

