---
name: dashboard-visual-quality
description: Elevates existing dashboard pages to a polished, premium, executive-ready visual standard while preserving the page's existing identity, structure, business logic, and purpose. Use when improving page-level visual quality, layout, spacing, typography, colors, cards, interactions, animations, responsiveness, and overall UX.
---

# Dashboard Visual Quality

## Purpose

Improve the visual quality and usability of an existing dashboard page without unnecessarily redesigning its structure or changing its business logic.

The goal is:

> Make the page feel intentionally designed, premium, modern, smooth, executive-ready, and easy to understand.

This skill is a **quality framework**, not a fixed page template.

Every page has its own identity, content density, purpose, and interaction model. Apply these principles intelligently rather than forcing every page to look identical.

---

# Core Rule

Before making changes:

1. Inspect the existing page.
2. Understand its purpose and information hierarchy.
3. Identify what already works.
4. Identify the biggest visual and UX weaknesses.
5. Preserve existing business logic and data calculations.
6. Preserve the page's identity and primary structure unless the requested improvement requires otherwise.
7. Improve visual quality through deliberate refinement rather than adding more UI.

Do not redesign a page simply because it looks different from another page.

The ServiceNow Campaigns page may be used as a **quality benchmark**, but it is NOT a visual template that every page must copy.

---

# 24 Visual Quality Principles

## 1. Visual Hierarchy

The most important information must be visually dominant.

Prioritize:

1. Page purpose
2. Primary business insight
3. Important KPIs
4. Supporting analysis
5. Detailed information

Do not give equal visual weight to everything.

Use size, spacing, typography, contrast, placement, and emphasis to establish hierarchy.

---

## 2. Page Composition

Create a clear visual flow from top to bottom.

The page should naturally answer:

> What am I looking at?
> What matters?
> What should I notice?
> What can I explore next?

Avoid layouts that feel like unrelated widgets placed next to each other.

Sections should feel intentionally connected.

---

## 3. Section Structure

Use clear sections to organize information.

Each section should have:

- clear purpose
- appropriate heading
- consistent spacing
- logical grouping
- visual separation where necessary

Avoid excessive boxes, borders, and unnecessary containers.

Use whitespace as a structural element.

---

## 4. Spacing

Use consistent spacing throughout the page.

Pay particular attention to:

- page margins
- section spacing
- card padding
- chart spacing
- heading-to-content spacing
- gaps between cards
- modal/table spacing

Avoid both:

- cramped layouts
- excessive empty space

Spacing should create rhythm.

---

## 5. Typography

Typography should establish hierarchy rather than simply display text.

Use clear differentiation between:

- page title
- section title
- card title
- KPI value
- supporting label
- metadata
- tooltip text
- table content

Avoid unnecessary font-size variation.

Keep text readable and concise.

Do not use typography as decoration.

---

## 6. Color System

Use a restrained and intentional color system.

Colors should communicate meaning.

Use:

- neutral colors for structure
- accent colors for emphasis
- semantic colors for status
- stronger contrast for important information

Do not introduce many unrelated colors.

Do not use bright colors simply to make the page look more exciting.

Maintain consistency with the dashboard's existing visual language.

---

## 7. KPI and Card Design

Cards should communicate information quickly.

A good KPI card should have:

- clear metric
- strong primary value
- concise label
- optional supporting context
- clear hierarchy

Avoid oversized decorative cards that consume space without adding information.

Use subtle borders, shadows, backgrounds, or highlights where appropriate.

Cards should feel connected to the page rather than floating independently.

---

## 8. Chart Selection

Choose the chart based on the question being answered.

Examples:

- comparison → bar chart
- ranking → horizontal bar chart
- trend → line/area chart
- composition → donut/pie
- distribution → histogram/bar distribution
- geographic mix → donut/pie or appropriate geographic visualization
- progression → funnel/progress visualization

Do not use the same chart type repeatedly simply for consistency.

Chart choice should improve comprehension.

---

## 9. Chart Composition

Charts must be visually clear and purposeful.

Prioritize:

- readable labels
- sensible axis ranges
- appropriate spacing
- useful legends
- meaningful annotations
- clear data hierarchy

Avoid:

- unnecessary gridlines
- excessive labels
- tiny text
- excessive chart decoration
- overly dense visuals

A chart should be understandable within seconds.

---

## 10. Chart Styling

Charts should feel modern and integrated into the page.

Use:

- clean backgrounds
- subtle gridlines
- appropriate corner radius
- restrained colors
- strong emphasis for important data
- muted styling for secondary data

Avoid stale-looking default chart styles.

Do not over-style charts with unnecessary gradients, shadows, or decoration.

---

## 11. Tooltips

Tooltips should add useful context without becoming distracting.

Tooltips should:

- appear smoothly
- remain readable
- show relevant values
- use consistent formatting
- avoid covering critical information where possible

Use tooltips for information that would otherwise clutter the chart.

Do not duplicate every visible label inside the tooltip.

---

## 12. Hover Behavior

Hover states should be intentional and stable.

Use subtle hover effects when they improve discoverability.

Examples:

- slight background change
- subtle border emphasis
- small elevation change
- cursor change for clickable elements

Avoid:

- layout shifts
- changing element dimensions
- text jumping
- columns moving
- charts resizing
- table rows changing height

For tables and dense data views, prioritize stability over decorative hover effects.

---

## 13. Animation

Animations should communicate state changes, hierarchy, or interaction.

Use subtle animation for:

- page transitions
- modal opening
- expanding sections
- chart appearance
- hover states
- filtering

Animations should be:

- short
- smooth
- purposeful
- consistent

Avoid excessive motion.

Do not animate every component independently.

Animation should never slow down a business workflow.

---

## 14. Transitions

Interactive state changes should feel smooth.

Use consistent transitions for:

- tabs
- filters
- cards
- modals
- dropdowns
- expandable sections
- hover states

Avoid abrupt visual changes unless immediate feedback is necessary.

---

## 15. Interactive States

Every interactive component should have clear states.

Consider:

- default
- hover
- active
- selected
- disabled
- loading
- error
- empty

Users should understand what is clickable and what is currently selected.

Do not rely solely on color to communicate state.

---

## 16. Highlights and Emphasis

Important insights should receive intentional visual emphasis.

Use:

- accent color
- bold typography
- subtle background
- border treatment
- callout
- annotation
- visual positioning

Do not highlight everything.

If everything is emphasized, nothing is emphasized.

---

## 17. Filters

Filters should feel integrated rather than consuming excessive visual space.

Prioritize:

- clear labels
- logical grouping
- easy scanning
- obvious active state
- consistent controls

Avoid unnecessary filter controls.

Where possible, preserve the dashboard's existing global filter behavior.

Do not introduce page-specific filtering that conflicts with global filtering without a clear reason.

---

## 18. Tables

Tables should prioritize readability and stability.

Use:

- clear headers
- appropriate column widths
- consistent alignment
- readable row height
- sensible sorting
- useful filtering
- pagination where appropriate

Avoid unnecessary decoration.

Hovering over rows should NOT cause layout shifts.

Columns must remain stable when interacting with the table.

Long text should use truncation or controlled wrapping with tooltips where appropriate.

---

## 19. Modals and Drill-Downs

Drill-downs should feel like a natural extension of the page.

Use:

- smooth opening transition
- strong modal hierarchy
- clear title
- contextual summary
- stable table layout
- useful sorting/filtering
- clear close action

Do not make drill-downs feel like separate applications.

Reuse existing reusable modal/table patterns whenever available.

---

## 20. Loading, Empty, and Error States

Every major interactive component should handle:

- loading
- empty
- error

states gracefully.

Avoid blank areas that look broken.

Use concise messaging.

Loading states should preserve layout dimensions where possible to avoid content jumping.

---

## 21. Responsive Fitment

The page must remain visually coherent across supported screen sizes.

Check:

- card widths
- chart dimensions
- table overflow
- modal sizing
- text wrapping
- spacing
- navigation
- filter controls

Avoid layouts where components become cramped or unreadable.

Prioritize desktop dashboard usability while maintaining reasonable adaptability.

---

## 22. Information Density

The objective is not to maximize information displayed.

The objective is:

> Maximum useful information with minimum cognitive load.

Remove or visually de-emphasize information that does not contribute to the page's purpose.

Prefer progressive disclosure when detailed information is needed.

Use drill-downs, modals, expandable sections, or secondary views instead of overcrowding the main page.

---

## 23. Executive Storytelling

The page should help a leader understand the business quickly.

A strong page should make it easy to identify:

- what is happening
- what matters
- where there is risk
- where there is opportunity
- what changed
- what requires attention

Visual hierarchy should support the business narrative.

Do not optimize purely for visual beauty.

The page must remain useful for decision-making.

---

## 24. Final Visual QA

Before completing the task, inspect the page as a user.

Check:

### Visual
- Does the page feel premium?
- Is the hierarchy obvious?
- Is spacing consistent?
- Are colors intentional?
- Do charts look modern?
- Are sections visually balanced?

### Interaction
- Do hover states remain stable?
- Are transitions smooth?
- Are clickable elements obvious?
- Do modals open naturally?
- Do filters behave predictably?

### Data presentation
- Are labels readable?
- Are tooltips useful?
- Are charts understandable?
- Are tables aligned?
- Are numbers formatted correctly?

### Fitment
- Does the page feel cohesive?
- Is anything unnecessarily crowded?
- Is there excessive empty space?
- Are components aligned?

### Regression
- Did any existing business logic change?
- Did any existing KPI calculation change?
- Did global filters change?
- Did unrelated pages change?

If the answer to any regression question is yes, fix it before completing the task.

---

# Design Benchmark

Use the existing ServiceNow Campaigns page as a benchmark for:

- visual polish
- spacing
- typography
- chart quality
- color discipline
- interaction smoothness
- section composition
- executive readability

However:

DO NOT copy its layout blindly.

Each dashboard page should retain its own:

- identity
- purpose
- information hierarchy
- content structure
- interaction model

The benchmark defines the **quality bar**, not the page template.

---

# Implementation Rules

When applying this skill to an existing page:

1. Inspect the existing implementation first.
2. Do not rewrite the page unnecessarily.
3. Preserve existing data sources.
4. Preserve existing business logic.
5. Preserve existing calculations.
6. Preserve existing global filters unless explicitly asked to change them.
7. Reuse existing components where appropriate.
8. Prefer targeted improvements over wholesale rewrites.
9. Avoid introducing new dependencies unless necessary.
10. Keep visual behavior consistent with the rest of the dashboard.
11. Do not change unrelated pages.
12. Do not create placeholder data when real data already exists.
13. Do not invent metrics or business logic.
14. Do not sacrifice usability for visual effects.

---

# Definition of Done

A page is visually improved when:

- the hierarchy is immediately understandable
- the page feels cohesive
- charts are purposeful and modern
- colors communicate meaning
- spacing feels intentional
- typography is consistent
- interactions feel smooth
- hover states are stable
- tables remain readable
- drill-downs feel polished
- information density is controlled
- the page is executive-friendly
- existing functionality still works
- no unrelated functionality has changed

The goal is not "more design."

The goal is **better communication, better usability, and a premium dashboard experience.**
