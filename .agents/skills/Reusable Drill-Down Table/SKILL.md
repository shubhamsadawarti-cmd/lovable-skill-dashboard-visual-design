---
name: drill-down-table
description: Creates and improves reusable premium drill-down tables and modal views for dashboard data. Use when users need to click a KPI, chart, account count, metric, or other dashboard element to inspect the underlying records. Prioritizes stable layout, smooth opening transitions, sorting, filtering, search, tooltips, highlighting, readable tables, and zero layout shift.
---

# Reusable Drill-Down Table

## Purpose

Create a reusable drill-down experience that allows users to move from a dashboard summary to the underlying records without leaving the current page.

The drill-down should feel like a natural extension of the dashboard rather than a separate application.

The primary goals are:

- fast access to underlying records
- clear context
- stable table layout
- easy filtering and sorting
- smooth interaction
- executive-friendly presentation
- reusable implementation across dashboard pages

---

# Core Principle

When a user clicks a dashboard metric, chart element, account count, KPI, or other interactive element:

> Show the underlying data in a polished, contextual, stable modal/table without disrupting the user's current page.

Do not create a completely different table design for every page.

Build or reuse a common drill-down pattern wherever possible.

---

# 1. Reuse the Existing Drill-Down Pattern

Before creating a new drill-down:

1. Inspect the existing dashboard for an existing drill-down modal/table.
2. Reuse the existing component if it already meets the requirements.
3. Improve the reusable component rather than duplicating it.
4. Keep the visual language consistent across pages.

If a reusable drill-down component already exists, do NOT create another competing implementation.

---

# 2. Contextual Modal Title

The modal must clearly explain what the user is looking at.

Examples:

- `39 Existing Customers`
- `Hot Prospects — 102 Accounts`
- `Open Pipeline — 24 Opportunities`
- `Closed Won — 18 Opportunities`
- `North America Accounts — 42 Accounts`

The title should reflect the exact selection/filter that triggered the drill-down.

Avoid generic titles such as:

- `Data`
- `Details`
- `Records`
- `Table`

---

# 3. Summary Context

Where useful, provide a small contextual summary above the table.

Examples:

- total records
- total ACV
- total pipeline
- selected region
- selected campaign
- selected industry

Keep the summary lightweight.

Do not turn the drill-down modal into another dashboard.

---

# 4. Modal Size and Fitment

The modal should provide enough space for the table without feeling oversized.

Prefer:

- wide desktop modal
- strong horizontal space
- comfortable vertical scrolling
- clear internal padding
- fixed header area
- stable table area

Avoid unnecessarily narrow modals that cause excessive wrapping.

Avoid full-screen layouts unless the dataset genuinely requires it.

---

# 5. Opening Transition

The modal should open smoothly.

Use a subtle transition such as:

- fade
- slight scale
- slight vertical movement

Keep the animation short and professional.

Do not use dramatic motion.

The user should feel that the table has appeared naturally from the element they clicked.

---

# 6. Background Treatment

When the modal opens:

- preserve the underlying page context
- use a subtle backdrop
- maintain sufficient contrast
- keep focus on the modal

The background should not become visually distracting.

---

# 7. Table Structure

Use a clear table structure:

- stable column widths
- readable headers
- consistent row height
- appropriate alignment
- sufficient cell padding
- clear separation between header and body

Avoid excessive borders.

Use whitespace and subtle separators to create structure.

---

# 8. Stable Table Layout

This is critical.

Hovering over a row must NOT cause:

- column movement
- text shifting
- row resizing
- width changes
- alignment changes
- scrollbar jumps
- modal resizing

The table must remain visually stable during interaction.

Do not use hover effects that modify dimensions.

---

# 9. Hover Behavior

Hover states should be subtle.

Preferred behavior:

- slight background highlight
- cursor change where appropriate

Avoid:

- changing font size
- changing font weight if it affects width
- adding borders that change dimensions
- expanding cells
- moving content
- changing row height

For dense account/opportunity tables, stability is more important than decorative interaction.

---

# 10. Column Selection

Do not display every available field automatically.

Choose fields based on the user's purpose.

Prioritize:

1. identifying information
2. key business information
3. useful segmentation
4. status/activity
5. supporting context

Example account table:

| Account | Industry | Employees | Country | Status | Last Activity |
|---|---|---:|---|---|---|

Example opportunity table:

| Opportunity | Account | Stage | ACV | Region | Owner | Close Date |
|---|---|---|---:|---|---|---|

Avoid unnecessary columns that increase cognitive load.

---

# 11. Column Widths

Column widths should be intentional.

Use:

- wider columns for account/opportunity names
- medium width for industry/status
- narrower width for numeric values
- appropriate width for dates
- truncation for unusually long text

Do not allow long content to destroy the table layout.

---

# 12. Text Overflow

Long text should not force columns to expand.

Use:

- truncation
- ellipsis
- controlled wrapping where appropriate

When text is truncated, provide a tooltip where useful.

Tooltips should show the complete value without changing the table layout.

---

# 13. Sorting

Provide sorting for meaningful columns.

Examples:

- account name
- employees
- ACV
- date
- status
- industry

Sorting should:

- clearly indicate active sort column
- indicate ascending/descending direction
- preserve table dimensions
- work consistently

Default sorting should be meaningful for the context.

Examples:

- largest ACV first
- most recent activity first
- highest employee count first
- alphabetical account name

---

# 14. Filtering

Provide filtering when the dataset is large enough to justify it.

Useful filters may include:

- industry
- region
- country
- account status
- employee range
- campaign
- owner
- stage

Do not add filters simply because fields exist.

Filters should answer realistic exploration questions.

---

# 15. Search

For sufficiently large account/opportunity lists, provide search.

Search should typically cover the primary identifying field:

- Account Name
- Opportunity Name

Search should update results smoothly.

Show the filtered record count.

Example:

`Showing 24 of 102 accounts`

---

# 16. Active Filter Visibility

Users should always understand why they are seeing a particular subset.

Show active filters clearly.

Examples:

`Campaign: Hot Prospects`

`Industry: Technology`

`Region: NorAm`

Provide an easy way to clear filters.

---

# 17. Result Count

Always show the number of records being displayed.

Examples:

- `39 accounts`
- `24 of 102 accounts`
- `18 opportunities`

The count should update when search/filtering is applied.

---

# 18. Numeric Formatting

Numbers must be formatted consistently with the rest of the dashboard.

Examples:

- employee counts → `51,633`
- ACV → `$2.4M`
- percentages → `42%`

Do not expose raw database formatting.

Use appropriate decimal precision.

---

# 19. Date Formatting

Dates should use the dashboard's established date format.

Avoid exposing raw JavaScript date strings.

Prefer concise formats such as:

- `Aug 11, 2026`
- `11 Aug 2026`

Use relative dates only where they provide genuine value.

---

# 20. Semantic Colors

Use dashboard-consistent semantic colors.

Examples:

- positive → green
- warning → amber
- negative → red
- neutral → gray
- selected → dashboard accent

Do not introduce arbitrary colors.

Color should communicate meaning rather than decoration.

---

# 21. Important Values

Important values can receive subtle emphasis.

Examples:

- high ACV
- high employee count
- active status
- recent activity
- priority account

Use restrained highlighting.

Do not highlight every row.

---

# 22. Empty State

If filters return no records:

Show a clear empty state.

Example:

`No accounts match the selected filters.`

Provide:

`Clear Filters`

Do not show an empty table with unexplained blank space.

---

# 23. Loading State

When records are being loaded:

- preserve the modal dimensions
- avoid layout jumping
- use a subtle loading state
- avoid excessive animation

Where possible, show contextual loading text.

Example:

`Loading accounts…`

---

# 24. Pagination and Large Datasets

For large datasets, avoid rendering unnecessary records simultaneously.

Use:

- pagination
- virtualization
- controlled scrolling

depending on the existing application architecture.

The user should be able to navigate large datasets smoothly.

---

# 25. Row Actions

Only add row-level actions when there is a clear business need.

Examples:

- open account
- view opportunity
- open Salesforce record

Do not add unnecessary action icons to every row.

---

# 26. Account / Opportunity Identification

The primary identifying field should be visually clear.

For example:

`Microsoft`

or

`Acme Corporation — HR Transformation`

Avoid making the primary identifier visually weaker than secondary metadata.

---

# 27. Modal Close Behavior

Provide multiple intuitive ways to close the modal where appropriate:

- close button
- Escape key
- clicking outside the modal if consistent with the dashboard's UX

Do not accidentally close the modal when the user is interacting with table content.

---

# 28. Preserve Dashboard Context

Closing the drill-down should return the user to exactly where they were.

Do not:

- reset filters
- reset scroll position unnecessarily
- change tabs
- navigate to another page
- lose the user's dashboard state

The drill-down should be reversible.

---

# 29. Accessibility

Ensure:

- keyboard-accessible controls
- visible focus states
- readable contrast
- meaningful labels
- logical tab order
- accessible close behavior

Do not rely only on hover to communicate information.

---

# 30. Responsive Behavior

The drill-down should remain usable across supported desktop screen sizes.

For narrower screens:

- allow horizontal table scrolling where necessary
- preserve important columns
- avoid breaking the modal
- maintain readable text

Do not compress every column until the table becomes unreadable.

---

# 31. Do Not Overload the Modal

The drill-down is for exploration, not a second dashboard.

Avoid adding:

- large KPI grids
- multiple charts
- unnecessary narrative
- excessive filters
- unrelated controls

The primary purpose should remain:

> Let the user inspect the records behind the dashboard insight.

---

# 32. Reusability

Build the component so it can support different datasets.

The reusable pattern should ideally allow:

- different titles
- different datasets
- different columns
- different default sorting
- different filters
- different search fields
- different record labels

Example:

```text
DrillDownModal
├── Context Header
├── Summary
├── Search / Filters
├── Result Count
├── Table
└── Pagination / Footer
