# Audit Skill

## Purpose

Use this skill when the task is to review, extend, or continue the Bank Albilad design-system audit.

## Required Reads

Read these before acting:

1. `design.md`
2. `docs/principles.md`
3. `docs/audit.md`
4. the relevant file in `docs/audit-domains/`

## What This Skill Must Do

1. Identify the correct audit domain.
2. Review the delivered audit section for that domain.
3. Review the original Albilad DS source for the same area.
4. Decide whether the issue is:
   - already covered
   - an extension of an existing item
   - a new item
5. Write in the existing audit structure:
   - Finding / Current Case
   - Suggestion
   - Explanation
   - Severity

## Continuation Rules

- Preserve the existing audit tone and granularity.
- Do not duplicate findings when an extension is enough.
- Do not change severity logic.
- Do not write screen-level UX findings as audit items unless they reveal a reusable DS issue.

## Escalation Rules

Delegate to a narrower audit skill when the domain is clear.

Examples:

- color issue -> `skills/audit-color-skill.md`
- typography issue -> `skills/audit-typography-skill.md`
- button issue -> `skills/audit-actions-skill.md`

## Output Contract

Return one of these outcomes:

- `existing-item-reused`
- `existing-item-extended`
- `new-item-created`

Then provide the final audit entry in report-ready form.

