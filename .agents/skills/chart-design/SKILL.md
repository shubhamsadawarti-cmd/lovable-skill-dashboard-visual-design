---
name: dashboard-charts
description: Use when reviewing, improving, replacing, or adding charts and data visualizations on an existing dashboard page. Choose visualizations based on the business question and data structure while preserving page identity, business logic, calculations, and existing data contracts.
---

# Dashboard Charts & Data Visualization

## Purpose

Create charts that communicate business information quickly, clearly, and confidently to an executive audience.

The goal is NOT to maximize the number of charts or make charts visually decorative.

The goal is:

> Turn data into an immediately understandable business story.

Use the ServiceNow Campaigns page as a benchmark for chart quality and polish, but DO NOT copy its chart layout or force the same chart types onto other pages.

Every page has its own identity and should use the visualization types that best communicate its specific business questions.

---

# 1. Preserve Page Identity

Before changing any chart:

- Understand the purpose of the page.
- Identify the primary business question.
- Understand what the current chart is intended to communicate.
- Preserve the page's existing identity and information hierarchy.
- Do not redesign the entire page unless explicitly requested.
- Do not introduce charts simply because they look visually impressive.

A Pipeline page should continue to feel like a Pipeline page.

A Revenue page should continue to feel like a Revenue page.

A Partner page should continue to feel like a Partner page.

Charts should strengthen the page's story rather than redefine it.

---

# 2. Start With the Business Question

Before choosing a chart type, determine what the visualization is answering.

Examples:

### Trend question

"How has pipeline changed over time?"

Prefer:

- line chart
- area chart
- cumulative line
- comparison line

### Composition question

"What makes up the total?"

Prefer:

- donut
- pie
- stacked bar
- 100% stacked bar

### Ranking question

"Which partners/accounts/industries contribute the most?"

Prefer:

- horizontal bar chart
- ranked bar chart

### Distribution question

"How are accounts distributed across company sizes?"

Prefer:

- horizontal bar chart
- histogram-style distribution
- grouped distribution

### Comparison question

"How does A compare with B?"

Prefer:

- grouped bar
- stacked bar
- paired KPI treatment
- comparison line

### Geographic mix

"Where are these accounts located?"

Prefer:

- donut/pie for simple regional composition
- ranked horizontal bar when there are many countries/locations

### Status progression

"How are accounts/deals progressing through stages?"

Prefer:

- funnel
- segmented progression
- horizontal stage bars
- carefully designed status pipeline

Do not use a chart type simply because it is available.

---

# 3. Choose the Simplest Effective Visualization

The best chart is the simplest chart that communicates the intended message.

Avoid unnecessary complexity.

For example:

If the question is:

"What percentage of accounts are NorAm vs INTL?"

A simple donut is preferable to a complex stacked visualization.

If the question is:

"Which industries have the most accounts?"

A horizontal bar chart is preferable to a pie chart with 12 slices.

If the question is:

"How has revenue changed month over month?"

A line chart is preferable to twelve separate KPI cards.

---

# 4. Avoid Repetitive Chart Design

Do not automatically turn every dataset into a vertical bar chart.

A page containing:

- Bar chart
- Bar chart
- Bar chart
- Bar chart

often feels like a generic BI dashboard.

Use visual variety when the underlying questions differ.

For example:

```text
Industry Mix
→ horizontal bar

Geography Mix
→ donut

Employee Distribution
→ horizontal bar

Trend
→ line / area

Status
→ segmented progression
