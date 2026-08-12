---
name: dashboard-visual-design
description: Use when improving, redesigning, or visually polishing an existing dashboard page or dashboard section. Apply premium executive-ready visual design principles while adapting the layout to the page's specific purpose. Do not use this skill to change business logic, calculations, data sources, or KPI definitions unless explicitly requested.
---

# Dashboard Visual Design

## Purpose

Improve the visual quality of an existing dashboard page so it feels premium, executive-ready, intentional, and easy to understand.

Use the ServiceNow Campaigns page in the Partnerships Dashboard as the benchmark for visual polish.

Do NOT copy its exact layout. Reuse the design principles and adapt them to the purpose and content of the page being improved.

---

## 1. First understand the page

Before making changes:

- Inspect the existing page structure.
- Understand what the page is trying to communicate.
- Identify the primary executive question the page should answer.
- Identify the most important information and the supporting information.
- Preserve the existing business logic, calculations, data sources, and filters unless the user explicitly asks for changes.

Do not redesign blindly.

The visual hierarchy should follow the importance of the information.

---

## 2. Executive visual hierarchy

The page should have a clear hierarchy:

1. Page purpose / title
2. Primary KPI or business message
3. Important insights
4. Supporting analysis
5. Detailed data

Avoid giving every element equal visual weight.

The user should be able to understand the page's main message within approximately 10–30 seconds.

Use:

- size
- spacing
- typography
- positioning
- restrained color
- sectioning
- visual emphasis

to establish hierarchy.

---

## 3. Layout and spacing

Use generous, intentional spacing.

Avoid:

- cramped cards
- excessive borders
- tightly packed charts
- unnecessary empty gaps
- inconsistent padding
- misaligned sections
- excessive information inside one card

Prefer:

- clear section boundaries
- consistent internal padding
- aligned card edges
- predictable spacing between sections
- breathing room around charts and KPIs

Do not force multiple unrelated sections into one row simply to save vertical space.

If three large sections are easier to understand vertically, use three sections vertically.

---

## 4. Cards

Cards should feel like intentional information containers, not generic BI widgets.

Use:

- subtle borders
- restrained shadows where appropriate
- rounded corners
- consistent padding
- clear headings
- strong primary numbers
- secondary supporting information

Avoid:

- excessive shadows
- heavy gradients
- decorative elements without purpose
- too many nested cards
- excessive visual noise

A card should answer one clear question.

---

## 5. Typography

Maintain a strong typography hierarchy.

Use:

- large, confident headings
- readable section titles
- clear KPI numbers
- restrained uppercase labels for metadata
- readable supporting text

Avoid:

- excessive font sizes
- too many font weights
- overly small labels
- long blocks of text
- inconsistent capitalization

Typography should make the page easier to scan, not simply make it look decorative.

---

## 6. Color

Use color intentionally.

The dashboard should have a restrained visual language.

Use color to communicate:

- category
- status
- emphasis
- comparison
- interaction

Do not color every element.

Avoid:

- rainbow charts
- excessive saturated colors
- arbitrary colors between sections
- using color without semantic meaning

When a page contains multiple categories, use a consistent palette across related visualizations.

Maintain strong contrast and readability.

---

## 7. Visual variety

Do not make every section look like the same component.

Choose the visual treatment based on the information.

Examples:

- KPI → large number + concise supporting context
- composition → donut/pie
- ranking → horizontal bar
- trend → line/area
- distribution → horizontal bar
- comparison → grouped/stacked bars
- status → compact status treatment
- detailed records → table/drill-down

The goal is not maximum chart variety.

The goal is to use the **most intuitive visual representation for each question**.

---

## 8. Interaction quality

Interactions should feel smooth and intentional.

Use subtle transitions for:

- opening/closing modals
- expanding sections
- changing filters
- changing views
- loading states

Avoid unnecessary animation.

Hover states must never cause layout shifts.

Elements should not:

- move
- resize
- jump
- change column widths
- cause neighboring content to shift

unless the interaction explicitly requires it.

---

## 9. Tooltips

Use tooltips when they provide useful context.

Good tooltip examples:

- exact chart values
- full text for truncated labels
- definitions
- additional metadata

Do not use tooltips for information that should simply be visible.

Tooltips should be clean, readable, and consistent.

---

## 10. Data density

Do not try to show everything on the first screen.

Prioritize:

- what leadership needs immediately
- the main story
- the most useful comparisons

Move detailed information into:

- drill-downs
- expandable sections
- modals
- secondary views

The dashboard should feel informative without feeling crowded.

---

## 11. Responsive behavior

The layout must remain usable at different viewport sizes.

Do not allow:

- horizontal overflow
- clipped charts
- overlapping labels
- broken cards
- unreadable tables

When necessary, change the layout structure at smaller widths rather than simply shrinking everything.

---

## 12. Preserve existing functionality

Unless explicitly requested:

DO NOT change:

- business logic
- KPI calculations
- fiscal-year logic
- filtering logic
- data transformations
- API contracts
- Supabase logic
- Salesforce ingestion
- existing routes
- permissions
- authentication

This skill is primarily for visual and UX improvement.

---

## 13. ServiceNow Campaigns benchmark

The ServiceNow Campaigns page represents the desired quality bar for this dashboard.

Use it as a reference for:

- spacing
- typography
- card composition
- restrained color
- chart variety
- visual hierarchy
- section separation
- executive readability
- interaction quality

However:

DO NOT copy its exact page structure.

Every dashboard page should have its own layout based on its content and purpose.

---

## 14. Before implementation

First inspect the existing implementation.

Identify:

- current layout
- existing reusable components
- existing design tokens
- existing chart components
- existing modal/table components
- existing spacing conventions

Reuse existing components where appropriate.

Do not create duplicate components when an existing reusable component already provides the required behavior.

---

## 15. Quality bar

Before considering the work complete, verify:

- The page has a clear visual hierarchy.
- The most important information is visually dominant.
- Sections are not unnecessarily crowded.
- Charts are appropriate for the data.
- Typography is consistent.
- Spacing is intentional.
- Colors are restrained and meaningful.
- Cards feel polished.
- Interactions feel smooth.
- Hover states do not cause layout shifts.
- Charts and labels remain readable.
- No unnecessary visual decoration was introduced.
- Existing business logic remains unchanged.

The final result should feel like a polished executive product, not a generic BI dashboard.
