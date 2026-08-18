
---

# `chart-design/README.md`

Create this file alongside `SKILL.md`:

```markdown
# Chart Design & Visualization

## Purpose

This skill defines the visual and interaction standards for charts across the Partner Operations dashboard.

It helps transform technically correct charts into polished, executive-ready visualizations that communicate insights quickly.

## When to Use

Use this skill when:

- creating a new chart
- redesigning an existing chart
- improving chart visual quality
- selecting the appropriate chart type
- improving tooltips
- improving hover behavior
- improving chart colors
- adding or refining animation
- improving labels or legends
- improving chart spacing or fitment
- making charts more executive-friendly
- reducing chart clutter
- improving chart interactions

## What This Skill Covers

### Visualization

- selecting the right chart for the business question
- trend visualization
- category comparison
- distribution
- composition
- geographic mix
- rankings
- KPI visualization

### Visual Design

- visual hierarchy
- color semantics
- restrained color palettes
- clean backgrounds
- spacing
- typography
- chart-card treatment
- responsive fitment

### Interaction

- tooltips
- hover states
- transitions
- animation
- filtering
- stable layouts
- zero and empty states

### Executive Readability

Charts should allow leadership to understand the primary insight quickly without needing to decode complex visualizations.

## Important Principle

This skill is **not a page template**.

It should not make every dashboard page look the same.

Apply the principles according to the individual page's:

- business purpose
- information hierarchy
- visual identity
- available space
- audience
- data

For example, the Campaigns page may use a donut for geographic mix and horizontal bars for employee distribution, while the Revenue page may use line and area charts for trends.

The goal is **consistent quality, not identical design**.

## Relationship With Other Skills

This skill works particularly well with:

- `dashboard-visual-quality`
- `executive-page-design`
- `interaction-design`
- `drill-down-table`

When multiple skills apply, preserve the page's existing business logic and identity while combining the relevant design principles.

## Implementation Principle

Improve the visualization without unnecessarily changing:

- business logic
- calculations
- data sources
- API contracts
- filters
- unrelated components

The skill is primarily concerned with **how information is communicated visually and interactively**.
