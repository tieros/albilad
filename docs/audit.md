# Audit Method

## Purpose

The Audit workstream evaluates the design system itself.

It is not a product usability review.
It is not a redesign deliverable.
It is a structured diagnosis of system-level quality and readiness.

## Deliverable Structure

Every audit item must preserve the existing report format:

1. `Finding / Current Case`
2. `Suggestion`
3. `Explanation`
4. `Severity`

Do not replace this structure with a different reporting model.

## What Each Column Means

### Finding / Current Case

Describe what is wrong today.

The finding should be:

- specific
- observable
- written in the present state
- grounded in actual DS evidence

### Suggestion

Describe what should change.

The suggestion should be:

- actionable
- system-friendly
- implementable
- benchmark-aware

### Explanation

Explain why the suggestion matters.

The explanation should connect the recommendation to:

- usability
- accessibility
- consistency
- scalability
- maintainability
- developer handoff
- operational efficiency

### Severity

Use the logic already established in the audit report:

- `High`: urgent and important problems with broad impact
- `Medium`: important issues that affect quality, scale, or maintainability
- `Low`: improvements that matter but are not critical to system function

Severity should reflect impact plus frequency or spread.

## Audit Categories

Use the existing taxonomy:

- General Recommendations
- Foundations
- Assets
- Patterns
- Components
  - Navigation
  - Actions
  - Selection Controls
  - Forms
  - Indicators
  - Alerts
  - Overlays
  - Structure

## Research Inputs

Before adding or editing an audit item, review:

1. the relevant section in the delivered Audit Report
2. the original Albilad DS source for the same area
3. the component or foundation implementation details
4. strong industry references where useful

## Continuation Rules

When a new audit task arrives:

- do not write in a new tone
- do not invent a new column model
- do not create duplicate findings if the issue already exists
- do not split one issue into many weak items unless the separation improves actionability

Instead, decide whether the task should:

- reuse an existing item
- extend an existing item
- become a new item

## Writing Standards

Use language that is:

- direct
- precise
- implementation-aware
- useful for both designers and stakeholders

Avoid language that is:

- vague
- generic
- decorative
- emotionally loaded

## Domain Routing

Use the domain files in `docs/audit-domains/` when working in a specific area.

Those files define what to inspect and how to decide whether an issue belongs in that domain.

