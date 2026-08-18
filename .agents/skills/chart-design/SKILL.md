---
name: chart-design
description: Design and improve dashboard charts and data visualizations so they are executive-ready, visually polished, intuitive, interactive, and appropriate for the business question. Use when creating, redesigning, or improving charts, graphs, data visualizations, chart interactions, tooltips, legends, labels, axes, colors, or chart layouts.
---

# Chart Design & Visualization Skill

## Purpose

Create dashboard charts that communicate insights quickly and feel polished, intentional, and executive-ready.

Charts should not simply display data. They should help the user understand the story behind the data.

The goal is to avoid generic, stale, overly dense, or technically correct visualizations and instead create charts that are:

- visually polished
- easy to interpret
- appropriately interactive
- consistent with the dashboard
- responsive
- executive-friendly
- insight-oriented
- visually differentiated
- easy to scan

Do not apply the same chart type everywhere. Select the visualization based on the question the chart needs to answer.

---

# 1. Start With the Business Question

Before selecting a chart, determine what the user needs to understand.

Typical questions include:

- How is something changing over time?
- How large is each category?
- How does one category compare with another?
- What contributes most to the total?
- How is a population distributed?
- Where is the concentration?
- What is the mix?
- What is underperforming?
- What is driving the result?

Choose the chart based on the question rather than defaulting to the easiest chart to implement.

---

# 2. Chart Selection

Use chart types intentionally.

### Trends over time

Prefer:

- line charts
- area charts when cumulative magnitude is important
- combination charts only when there is a clear reason

Use time-series charts when the primary question is movement over time.

Avoid unnecessarily complicated multi-series charts.

### Category comparison

Prefer:

- horizontal bar charts
- vertical bar charts when categories are few
- grouped bars when comparison across a small number of dimensions is necessary

For long category names, prefer horizontal bars.

### Distribution

Prefer:

- horizontal bar charts
- histograms where appropriate
- bucketed distributions

For employee-size distributions, company-size ranges, pipeline ranges, etc., horizontal bars are generally preferred.

### Composition / Mix

Prefer:

- donut charts
- pie charts when there are very few categories
- 100% stacked bars for more precise comparison

Use pie/donut charts when the user needs to understand composition rather than exact category comparison.

Avoid pie charts with too many slices.

### Geographic mix

When there are only a few meaningful geographic groups, a donut or pie chart can provide a strong executive summary.

For many countries or regions, prefer a sorted horizontal bar chart or another more scalable visualization.

### Ranking

Prefer:

- sorted horizontal bar charts
- ranked tables with visual emphasis
- compact leaderboard-style components

Always make the ranking order obvious.

### KPI / headline metrics

Use:

- KPI cards
- large-value metric blocks
- small supporting trend indicators

Do not use a chart when a single number communicates the insight better.

---

# 3. Visual Hierarchy

Every chart should have a clear hierarchy.

The user should immediately understand:

1. What the chart represents
2. What the most important insight is
3. What the comparison is
4. What the supporting detail is

Do not give every visual element equal visual weight.

Use:

- clear chart titles
- concise subtitles where useful
- highlighted primary values
- muted secondary information
- intentional spacing

The most important information should visually dominate.

---

# 4. Chart Titles

Chart titles should explain what the user is looking at.

Prefer:

- "Account Distribution by Employee Size"
- "Pipeline Trend vs Target"
- "Revenue Contribution by Partner"
- "Geographic Mix"

Avoid vague titles such as:

- "Distribution"
- "Overview"
- "Data"
- "Chart"
- "Analysis"

If useful, include a short contextual subtitle explaining the metric or timeframe.

---

# 5. Color System

Use color intentionally rather than decorating the chart.

Colors should communicate meaning.

Use a restrained palette.

### Semantic colors

Use consistent semantics across the dashboard:

- Green = positive / healthy / achieved
- Yellow or amber = warning / attention
- Red = negative / risk / below expectation
- Neutral gray = supporting or inactive information

Do not use red simply because it looks visually strong.

### Categorical colors

For categories that do not have semantic meaning:

- use a restrained set of complementary colors
- maintain consistency across the dashboard
- avoid excessive colors
- avoid rainbow palettes

### Highlighting

When one category is the focus:

- highlight the primary category
- keep secondary categories visually quieter

Do not make every bar, slice, or line equally prominent.

---

# 6. Backgrounds and Visual Treatment

Charts should generally sit on clean, uncluttered backgrounds.

Prefer:

- white or clean neutral chart areas
- subtle borders
- soft cards
- generous whitespace
- restrained shadows

Avoid:

- heavy gradients
- dark chart backgrounds unless specifically appropriate
- excessive borders
- excessive shadows
- decorative elements that compete with the data

The chart should feel premium without feeling ornamental.

---

# 7. Gridlines and Axes

Use gridlines only when they improve readability.

Prefer:

- subtle horizontal gridlines
- minimal vertical gridlines
- clean axes
- muted axis labels

Avoid:

- heavy gridlines
- unnecessary borders around the plotting area
- excessive tick marks
- visually dominant axes

Remove unnecessary chart furniture.

---

# 8. Labels and Data Values

Show values when they improve comprehension.

Use direct labels when:

- there are few categories
- exact values matter
- the chart would otherwise require excessive tooltip interaction

Avoid showing every value when it creates clutter.

For dense charts:

- prioritize tooltips
- highlight important values
- use abbreviated numbers where appropriate

Examples:

- 1.2M
- $450K
- 25.4K

Maintain consistent number formatting across the dashboard.

---

# 9. Tooltips

Tooltips should be polished and useful.

When hovering over a chart element, show:

- category / series name
- exact value
- relevant contextual information
- percentage where useful

Example:

```text
100K+ Employees
33 accounts
32.4% of prospects
