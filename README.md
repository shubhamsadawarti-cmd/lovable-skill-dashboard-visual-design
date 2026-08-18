# Lovable Dashboard Skills

Reusable design, UX, visualization, and interaction skills for the Partner Operations dashboard built in Lovable.

## Purpose

This repository acts as the shared design and implementation playbook for improving the dashboard.

The skills are intended to raise the overall quality and consistency of the dashboard while preserving the unique purpose and identity of each page.

## Core Principle

Skills should improve an existing page — not force every page to look identical.

When applying a skill:

1. Preserve the page's existing business purpose.
2. Preserve existing business logic and calculations.
3. Preserve the page's information hierarchy unless the task explicitly asks to change it.
4. Preserve the page's individual identity.
5. Apply the relevant skill principles appropriately to that page.
6. Avoid unnecessary redesign outside the requested scope.
7. Prioritize executive readability, visual hierarchy, polish, and usability.

## Available Skills

### 1. Dashboard Visual Quality

`dashboard-visual-quality`

Provides the overall visual quality bar for the dashboard, including:

- visual hierarchy
- spacing
- typography
- color usage
- component consistency
- whitespace
- executive readability
- premium visual polish
- interaction quality

## How Skills Should Be Used

Skills are reusable capabilities, not page templates.

For example:

> Apply the dashboard-visual-quality skill to the Pipeline page while preserving the existing Pipeline page identity, business logic, and information hierarchy.

A skill may be used independently or combined with other relevant skills.

## Skill Structure

Each skill lives under:

`.agents/skills/<skill-name>/`

The primary executable instructions are contained in:

`SKILL.md`

Additional supporting documentation may be included as `read.md` or under a `references/` directory.
