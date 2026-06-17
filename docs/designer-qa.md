# Designer Q&A Method

## Purpose

This method enables an AI agent with Figma access to answer designer questions without requiring one markdown file per component.

The repository should stay lean.
Answers should come from live retrieval across the original Albilad DS, Audit, Heuristic, and Boost sources.

## Use This Method When

A designer asks questions such as:

- How was this component built in the original Albilad DS?
- What did we criticize in Audit?
- What did we suggest instead?
- How did we implement it in the Boost component kit?
- Where did we use it in redesigned screens?
- What should I continue if I design a new variant or screen?

## Retrieval Model

Do not answer from memory.
Do not answer from repo docs alone.

Use the repo to route the question, then retrieve evidence from Figma in this order.

### Step 1. Normalize The Question

Identify:

- entity type:
  - foundation
  - component
  - pattern
  - screen
  - flow
  - process
- requested lens:
  - original state
  - audit critique
  - audit suggestion
  - heuristic finding
  - boost implementation
  - boost usage
  - future recommendation

### Step 2. Map To The Right Family

Examples:

- Button -> Actions
- Text Input -> Forms
- Tab -> Navigation
- Badge -> Indicators
- Banner -> Alerts or Structure depending on usage
- Color contrast -> Foundations / Color

Use the original Albilad DS structure first when choosing the family.

### Step 3. Read Evidence In The Right Order

For component and pattern questions:

1. Original Albilad DS source
2. Audit section for the same family
3. Boost component kit and guideline page
4. Boost flow pages showing real usage

For screen and flow questions:

1. Original screen or flow
2. Heuristic review if it exists
3. Relevant Audit items for the components involved
4. Matching Boost screen

### Step 4. Synthesize Instead Of Dumping

The answer should not be a raw reading of sources.
It should be a concise synthesis.

## Answer Format

Use this response shape whenever possible:

### 1. Original Albilad DS

State how the thing existed originally.

### 2. Audit Critique

State what Commencis criticized.

### 3. Audit Suggestion

State what Commencis recommended instead.

### 4. Boost Implementation

State how the component or pattern was handled in the Boost kit.

### 5. Boost Usage

State where or how it appears in redesigned screens.

### 6. Practical Takeaway

State what a designer should continue doing now.

## If Evidence Is Missing

If one layer is missing:

- say which layer is missing
- answer from the available layers
- do not fabricate certainty

Examples:

- no heuristic finding for this exact case
- no dedicated guideline page for this exact component
- no direct Boost usage, only a close precedent

## Confidence Rules

Be explicit about confidence:

- `high confidence` if the exact source exists in all relevant layers
- `medium confidence` if one layer is inferred from a close precedent
- `low confidence` if the answer depends on sparse or indirect evidence

## Repo Philosophy

This method replaces component-by-component markdown bloat with a repeatable retrieval-and-synthesis workflow.

The docs teach the agent how to investigate.
Figma provides the specific answer.

