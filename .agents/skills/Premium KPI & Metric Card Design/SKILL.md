---
name: kpi-card-design
description: Design and improve premium KPI cards and metric summaries for the dashboard while preserving page identity, hierarchy, business meaning, and usability.
---

# KPI Card Design Skill

Use this skill whenever creating, redesigning, or improving KPI cards, metric cards, summary cards, or executive metric blocks in the dashboard.

The goal is to make KPI cards feel like part of a premium executive product rather than generic BI tiles.

## 1. Preserve page identity

Do not apply a generic KPI-card template across the dashboard.

First understand:
- the purpose of the page
- the audience
- the surrounding visual language
- the importance of the metric
- whether the page is executive, analytical, operational, or exploratory

KPI cards should adapt to the page rather than making every page look identical.

## 2. Establish clear hierarchy

Each KPI card should communicate, in order:

1. What is being measured
2. The current value
3. Why the value matters
4. Optional supporting context

Avoid giving equal visual weight to every element.

The primary number should remain the strongest visual anchor.

## 3. Keep cards concise

Avoid putting too much information inside a KPI card.

Prefer:
- Metric label
- Primary value
- Short comparison/context
- Small trend or status indicator when useful

Do not turn KPI cards into miniature dashboards.

## 4. Use meaningful supporting context

Where relevant, include:
- vs previous period
- vs target
- vs prior year
- percentage change
- contribution/share
- status
- trend direction

Supporting information should answer "so what?" rather than simply adding decoration.

## 5. Use typography intentionally

Use clear typographic hierarchy:

- Small/medium label
- Large, prominent metric value
- Secondary supporting text
- Small contextual metadata

Avoid excessive font sizes, excessive weights, or too many text styles.

Numbers should be immediately scannable.

## 6. Format numbers intelligently

Use appropriate business formatting:

- `$1.2M`
- `$425K`
- `1,245`
- `24.5%`
- `3.2x`

Do not unnecessarily display long raw numbers.

Preserve precision where it materially affects interpretation.

## 7. Use color semantically

Color should communicate meaning, not decoration.

Use:
- positive states appropriately
- negative states appropriately
- neutral states appropriately
- warning/risk states appropriately

Do not color every KPI differently simply to make the page colorful.

Prefer restrained use of accent colors.

## 8. Use RYG semantics consistently

Where applicable:

- Green = healthy / positive
- Yellow/amber = attention / moderate risk
- Red = negative / risk

Apply these consistently throughout the dashboard.

Do not invent new meanings for colors on individual pages.

## 9. Avoid unnecessary gradients and decoration

Cards should feel premium through:
- spacing
- typography
- hierarchy
- subtle borders
- restrained shadows
- intelligent highlights
- clean alignment

Do not rely on heavy gradients, oversized icons, or decorative effects.

## 10. Use subtle visual depth

Cards can use:
- soft borders
- subtle shadows
- slight elevation
- restrained background differentiation
- subtle hover feedback where interaction exists

The visual treatment should remain sophisticated and lightweight.

## 11. Hover behavior

If a KPI card is not interactive:

- Do not make the contents move
- Do not shift text
- Do not resize the card
- Do not introduce distracting animations

If interactive:

- Use subtle elevation or border/highlight changes
- Preserve the card's dimensions
- Keep the interaction smooth

## 12. Interactive KPI cards

If a KPI card opens a drill-down:

Make the affordance clear without making the card visually noisy.

Possible cues:
- subtle cursor behavior
- small chevron
- understated "View details"
- controlled hover highlight

Do not make every card look clickable if only some are interactive.

## 13. KPI cards with drill-downs

When clicking a KPI opens detailed information:

Use the dashboard's existing reusable drill-down/modal pattern.

The KPI should act as the entry point, while the drill-down contains the detailed table, breakdown, or analysis.

Do not duplicate large amounts of detail inside the card.

## 14. Comparison indicators

For comparisons such as MoM, YoY, or vs target:

Make the comparison visually subordinate to the primary metric.

Example:

Revenue
$2.4M
↑ 18% vs last month

Avoid oversized comparison percentages competing with the main number.

## 15. Trend indicators

Small trend indicators can be useful:

- sparkline
- arrow
- percentage change
- mini trend line

Use them only when they add analytical value.

Do not add a sparkline to every KPI automatically.

## 16. Target / attainment KPIs

For target-oriented metrics, consider:

Current
$4.2M

Target
$5.0M

Attainment
84%

A compact progress indicator may be used when it improves comprehension.

Avoid turning every KPI into a progress bar.

## 17. Status KPIs

For metrics representing health or status:

Use clear semantic treatment.

Example:

Pipeline Health
Healthy
82%

The status should be immediately understandable without requiring the user to decode a visual.

## 18. Icons

Use icons sparingly.

Icons should:
- reinforce meaning
- improve scanning
- support navigation

Do not use generic decorative icons simply to fill space.

## 19. Alignment

Maintain consistent:
- card heights
- internal padding
- label alignment
- number positioning
- supporting text positioning

Cards displayed in the same row should feel structurally related.

## 20. Responsive behavior

KPI cards must remain usable across screen sizes.

On smaller screens:
- reduce columns
- preserve readable numbers
- prevent text wrapping from breaking hierarchy
- maintain appropriate spacing

Never allow cards to become cramped.

## 21. Tooltips

Use tooltips when metric definitions or calculation logic may not be obvious.

Good tooltip content:
- metric definition
- calculation methodology
- source
- important inclusion/exclusion rules

Do not use tooltips for information that should be visible by default.

## 22. Data integrity

Never change business logic merely to improve visual presentation.

Before displaying a KPI:
- verify the source
- verify filters
- verify calculation
- verify aggregation
- verify duplicate handling

If an existing KPI is incorrect, fix the logic rather than masking the issue visually.

## 23. Filter awareness

KPI cards should respond correctly to applicable global filters.

Ensure that:
- values update consistently
- labels remain accurate
- comparison periods remain logically valid
- cards do not display stale values

Do not create independent filtering logic unless explicitly required.

## 24. Avoid dashboard clutter

A page does not need many KPI cards to feel analytical.

Prefer a smaller number of meaningful metrics over a wall of cards.

Every KPI should answer a useful business question.

## 25. Executive storytelling

For executive-facing pages, prioritize:

1. What is happening?
2. How significant is it?
3. Is it improving or deteriorating?
4. Does leadership need to act?

The KPI design should support this narrative.

## 26. Visual consistency

Reuse established dashboard conventions where appropriate:
- typography
- spacing
- border radius
- shadows
- semantic colors
- interaction patterns
- modal/drill-down behavior

Do not introduce a completely new visual language for one KPI section.

## 27. Premium interaction

Where interaction exists, use subtle transitions.

Good:
- 150–250ms transitions
- slight elevation
- opacity/border changes
- controlled highlight

Avoid:
- bouncing
- excessive scaling
- flashing
- large movement
- distracting animation

## 28. Build before styling

When modifying KPI cards:

1. Confirm the metric/data logic.
2. Confirm the intended hierarchy.
3. Confirm whether the KPI is interactive.
4. Confirm applicable filters.
5. Then implement the visual design.
6. Verify the final rendering.

Do not redesign the visual before understanding the metric.

## 29. Do not redesign unrelated components

When this skill is invoked for KPI cards:

Do not automatically redesign:
- charts
- tables
- navigation
- page layout
- unrelated sections
- global filters

Only modify surrounding elements when necessary for KPI hierarchy or fitment.

## 30. Final quality check

Before completing the implementation, verify:

- KPI values are correct
- filters work correctly
- labels are accurate
- number formatting is appropriate
- hierarchy is clear
- cards align correctly
- no text shifts on hover
- no layout glitches occur
- interactive cards behave consistently
- colors have clear meaning
- cards do not feel overcrowded
- the result matches the visual quality of the strongest existing dashboard pages

The final result should feel like a polished executive analytics product, not a collection of generic dashboard tiles.
