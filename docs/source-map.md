# Source Map

This file maps the Figma sources that define the project.

## Original Albilad Design System

### Foundations

- Albilad DS Foundations:
  [Albilad DS Foundations](https://www.figma.com/design/1jlJoWT0eXCUcNdSyVYWxn/Albilad-DS---Foundations?m=auto&t=ZitQqCLyT89oX0lN-1)

Primary areas:

- Colors
- Typography
- Spaces
- Grids
- Borders
- Elevations

### Components

- Albilad DS Components:
  [Albilad DS Components](https://www.figma.com/design/0xvCklESPRNTcEEIYsi1dO/Albilad-DS---Components?m=auto&t=ZitQqCLyT89oX0lN-1)

Primary categories:

- Navigation
- Actions
- Selection Controls
- Forms
- Indicators
- Alerts
- Overlays
- Structure

## Audit Report

- Full Audit file:
  [Design System Audit Report Phase 2 ai](https://www.figma.com/design/D0hxjqZ3MFWbSRYiAm8XW5/Design-System-Audit-Report---Phase-2-_ai?m=auto&t=ZitQqCLyT89oX0lN-1)

Sections:

- General Recommendations
- Foundations
- Assets
- Patterns
- Navigations
- Actions
- Selection Controls
- Forms
- Indicators
- Alerts
- Overlays
- Structure
- Action Plan

## Heuristic Analysis

- Full Heuristic file:
  [Heuristic Analysis](https://www.figma.com/design/IV7aUgWgeSTQEUxisb2XiE/Heuristic-Analysis?m=auto&t=ZitQqCLyT89oX0lN-1)

Reviewed flows:

- Dashboard
- Profile
- Transfers
- Bill Payment
- Account Card Management
- Credit Loan Application
- Cash Position
- Explore
- User Feedback and Satisfaction
- Onboarding

## UX/UI Boost

- Full Boost file:
  [UX UI Boost Component Kit](https://www.figma.com/design/eG5sVt1KersCtjIP6lb6oT/UX-UI-Boost---Component-Kit?m=auto&t=ZitQqCLyT89oX0lN-1)

Boost flow groups:

- Dashboard
- Transfers
- Accounts and Cards
- Bills
- Credit Card Application

Boost component foundations:

- Foundations node in Boost file

Boost component kit families:

- Avatar
- Badge
- Banner
- Button
- Icon Button
- FAB
- Bottom Navigation
- Card
- Checkbox
- Chip
- Header
- List Item
- Text Input
- Progress
- Progress Indicator
- Radio
- Search
- Tab
- Tabs
- Toggle
- Quick Actions
- Accordion
- Background
- Divider
- Overlay
- Section Header
- Text / Amount

Guideline pages exist for many of these components and should be used whenever available.

## Question-To-Source Routing

Use this retrieval model when a designer asks an ad hoc question.

### "How was this component in the original Albilad DS?"

Check:

1. `Albilad DS Foundations` if it is a foundation topic
2. `Albilad DS Components` if it is a component or pattern topic

### "What did Commencis criticize in Audit?"

Check:

1. the matching audit category
2. the matching subdomain logic in `docs/audit-domains/`

### "What did Commencis suggest instead?"

Check:

1. the matching audit item
2. the relevant explanation and severity context

### "How was it redesigned in Boost?"

Check:

1. the Boost component kit for the component implementation
2. the Boost guideline page if one exists

### "Where did we actually use it in redesigned screens?"

Check:

1. the Boost flow pages
2. the matching after screens
3. the nearest visual precedent if the exact component does not appear in only one place

### "How should I answer if the question mixes all of these?"

Answer in this order:

1. original Albilad DS state
2. audit critique
3. audit suggestion
4. boost implementation
5. boost usage in redesigned screens
6. practical takeaway for future work

## Lightweight Retrieval Rule

Do not pre-document every component.

Only store enough routing and method guidance here so an agent with Figma access can fetch the answer live.

