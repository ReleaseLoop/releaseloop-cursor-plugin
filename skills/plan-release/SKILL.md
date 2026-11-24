---
name: plan-release
description: Inspect and plan a music release in ReleaseLoop. Use when the user asks to list scheduled releases, open a release, or summarize its tracks, open tasks, marketing, and budget.
---

# Plan or inspect a release

The assistant uses the signed-in user's ReleaseLoop account. It can only see what that user can see.

## Steps

1. If the user belongs to more than one workspace, ask which one. Do not guess.
2. List releases. They come back newest first. Ask for a date range if the user gave one.
3. Open the release the user named. Summarize credits, tracks, tasks, marketing, and budget.
4. Report open tasks (To do, In progress) separately from finished ones (Done, Approved).

## Hidden and empty sections

- If marketing or budget is not visible, say you do not have access to that section.
- If a section is visible but empty, say there is nothing there yet.

## Rules

- Release statuses are Draft, Scheduled, Released, and Archived.
- Only report what the tools return. Do not invent tracks, tasks, or amounts.
