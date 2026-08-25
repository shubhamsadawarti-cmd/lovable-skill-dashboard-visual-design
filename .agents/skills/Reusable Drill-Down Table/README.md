# Drill-Down Table

## Purpose

This skill defines the reusable drill-down table and modal pattern for the dashboard.

It allows users to click a dashboard insight and inspect the underlying records without leaving the current page.

## When to Use

Use this skill when:

- clicking a KPI should show underlying records
- clicking an account count should show an account list
- clicking a chart segment should show matching records
- users need to inspect opportunities behind a metric
- an existing drill-down table needs visual or UX improvement
- a page needs a reusable account/opportunity table modal

## Core Experience

The standard flow is:

Dashboard Insight  
↓  
Click  
↓  
Contextual Modal  
↓  
Search / Filters  
↓  
Stable Table  
↓  
Sort / Explore  
↓  
Close  
↓  
Return to Dashboard

## Key Principles

The drill-down should be:

- contextual
- stable
- reusable
- searchable
- sortable
- filterable where useful
- visually polished
- easy to scan
- free of layout shifts

## Important UX Rule

Hovering over table rows must never cause layout shifts.

Do not allow:

- columns to move
- rows to resize
- text to jump
- borders to change dimensions
- modal dimensions to change

Use subtle visual highlighting instead.

## Reusability

The pattern should work across different dashboard pages and datasets.

Examples:

- ServiceNow campaign accounts
- partner accounts
- pipeline opportunities
- revenue records
- closed-won opportunities
- KPI drill-downs

The component should support different datasets and column configurations without creating a completely separate table implementation for each page.

## Relationship With Other Skills

Use this skill together with:

- `dashboard-visual-quality` for overall visual polish
- `chart-design` when the drill-down originates from a chart
- future filter/table-specific skills when available

This skill controls the **drill-down experience**, while the other skills control the broader page and visualization quality.

## Quality Benchmark

The ServiceNow Campaigns account drill-down is the reference experience for:

- modal presentation
- table stability
- spacing
- sorting
- filtering
- account exploration
- visual polish

Use it as a quality benchmark while keeping the implementation reusable for other dashboard pages.
