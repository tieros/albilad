# Design Workflow Entry Point

This repository is the onboarding and execution layer for the Bank Albilad design-system modernization workflow.

Its goals are:

1. Onboard new designers quickly.
2. Give AI agents a reliable operating model.
3. Preserve continuity with the work already delivered by Commencis.
4. Keep Audit, Heuristic, and Boost workstreams independent but composable.

## What This Repository Covers

- `Audit` is about the design system itself.
- `Heuristic` is about UX review of existing product screens.
- `Boost` is about redesigning selected screens by combining Audit and Heuristic insight and implementing the result through the Boost component kit.

## How To Navigate

- Read [docs/brief.md](docs/brief.md) for project purpose and scope.
- Read [docs/source-map.md](docs/source-map.md) for the Figma source inventory.
- Read [docs/principles.md](docs/principles.md) for the shared operating rules.
- Read [docs/audit.md](docs/audit.md) for the DS audit method.
- Read [docs/heuristic.md](docs/heuristic.md) for the UX review method.
- Read [docs/boost.md](docs/boost.md) for the redesign method.

## Which File To Use

Use this routing logic:

- If the task is "review the design system", start with [docs/audit.md](docs/audit.md) and [skills/audit-skill.md](skills/audit-skill.md).
- If the task is "review a product flow or screen UX", start with [docs/heuristic.md](docs/heuristic.md) and [skills/heuristic-skill.md](skills/heuristic-skill.md).
- If the task is "redesign or improve a screen", start with [docs/boost.md](docs/boost.md) and [skills/boost-skill.md](skills/boost-skill.md).
- If the task is "add a new audit item for a specific DS area", use the matching audit domain skill in `skills/`.

## Core Rule

Method documents and skill documents are separate on purpose.

- `docs/*.md` explain how the work should be done.
- `skills/*.md` explain how an AI agent should execute the work.

Do not merge those responsibilities.

## Continuity Rules

- Match the structure, tone, and granularity of the existing Commencis artifacts.
- Continue the current Audit logic instead of inventing a new audit model.
- Continue the current Heuristic logic instead of introducing a different evaluation template.
- Continue the current Boost visual taste instead of creating a new visual language.

## Source Priority

When making decisions, use this order:

1. Existing Commencis deliverables in Audit, Heuristic, and Boost.
2. Original Albilad DS foundations and components.
3. Boost component kit and guidelines.
4. Industry best practices and well-known design systems such as Carbon, IBM, Atlassian, Polaris, Base, Wise, and similar mature systems.

## Combined Workflow

When a task is a full redesign request:

1. Identify the target screen, flow, or component.
2. Check whether an existing Audit item already covers the DS issue.
3. Check whether an existing Heuristic finding already covers the UX issue.
4. Check whether an existing Boost flow already solved a similar case.
5. Reuse the Boost component kit if possible.
6. If the kit does not cover the need, extend an existing variant before creating a new component.
7. Only create a new component when reuse or extension is insufficient.
8. Preserve accessibility, scalability, atomic structure, and visual taste.

## Expected Agent Profile

Any agent using this repository should behave like a strong UI/UX expert:

- strong heuristic analysis
- strong accessibility judgment
- strong design-system thinking
- strong component architecture judgment
- strong visual taste
- strong continuity discipline

## Deliverable Philosophy

This repository is not a generic design playbook.

It is a project-specific operating system for the Bank Albilad workstream.

