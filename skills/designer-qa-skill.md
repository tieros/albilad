# Designer Q&A Skill

## Purpose

Use this skill when a designer asks an ad hoc question about how something existed, was criticized, was improved, or was used across the Bank Albilad workstream.

This skill assumes the agent has Figma access.

## Required Reads

1. `design.md`
2. `docs/principles.md`
3. `docs/source-map.md`
4. `docs/designer-qa.md`

Read additional method docs only when the question clearly requires them:

- `docs/audit.md` for audit interpretation
- `docs/heuristic.md` for heuristic interpretation
- `docs/boost.md` for redesign interpretation

## What This Skill Must Do

1. Normalize the question.
2. Identify the entity type and requested lens.
3. Route the question to the correct DS family using the original Albilad structure.
4. Read live evidence from the correct Figma sources.
5. Synthesize the answer in a structured way.
6. Preserve continuity with Commencis logic and visual direction.

## Retrieval Order

For component questions:

1. original Albilad DS
2. Audit
3. Boost component kit
4. Boost guideline page if available
5. Boost screen usage

For screen or flow questions:

1. original screen or flow
2. Heuristic review
3. relevant Audit findings
4. Boost redesign

## Answer Contract

When the question spans multiple layers, answer in this order:

1. Original Albilad DS state
2. Audit critique
3. Audit suggestion
4. Boost implementation
5. Boost usage
6. Practical takeaway

## Example Questions This Skill Should Handle

- How was Button handled in the original DS?
- What did we criticize about Tabs?
- How did we redesign Text Input?
- Where did we use Banner in Boost?
- Is there an Audit item that explains why this screen changed?
- If I extend this component now, what should I follow?

## Non-Negotiable Rules

- Do not answer from repo docs alone if Figma evidence is needed.
- Do not invent exact component details.
- Do not ignore Audit when the question is about DS quality.
- Do not ignore Boost precedents when the question is about current UI direction.
- Do not over-document the repo instead of retrieving live evidence.

## Confidence Rule

Label certainty mentally while reasoning:

- exact evidence in the expected layer set -> high confidence
- partial or nearby precedent -> medium confidence
- sparse evidence -> low confidence

Be transparent if a key layer is missing.
