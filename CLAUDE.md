# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Repository Is

This is a **business planning and research repository** (not a software codebase) for launching a Mississippi aggregate hauling company targeting the $49B data center construction boom. All content is Markdown documents, a CSV financial model, and planning tools — there are no build systems, tests, or application code.

## Repository Structure

- `BUSINESS-PLAN.md` — Full 16-section business plan (the master document; other files elaborate on sections within it)
- `README.md` — Public-facing summary of the business and repo
- `TODO.md` — Task tracker for remaining work items
- `research/` — Numbered deep-dive research files (01 through 07), covering projects, regulations, economics, trucks, office space, competitive analysis, and used equipment listings
- `projects/` — Site-specific hauling plans for each of the 5 data center projects (xAI Southaven, AWS Madison County, Compass Meridian, AVAIO Brandon, AWS Vicksburg)
- `tools/` — Operational documents: financial models (5-year P&L and monthly cash flow), contact tracker, truck comparison, launch checklist, office space research, hauling contract template, invoice and BOL templates, CDL driver job posting

## Key Conventions

- Research files use a numbered prefix (`01-`, `02-`, etc.) to indicate reading order
- Each project under `projects/` has a single `hauling-plan.md` with site-specific intel, quarry distances, routes, and strategy
- Financial figures should stay internally consistent across BUSINESS-PLAN.md, README.md, tools/financial-model.csv, and tools/monthly-cash-flow.md
- The contact tracker (`tools/contact-tracker.md`) is the single source of truth for quarry, contractor, and agency contact info — update it rather than scattering contacts across other files
- The competitive analysis (`research/06-competitive-analysis.md`) is the source of truth for competitor data — update it rather than duplicating competitor info in other files

## When Editing

- Keep the README.md financial tables and project table in sync with BUSINESS-PLAN.md when either is updated
- TODO.md tracks remaining deliverables — move items to "Completed" when finished
- New research topics should follow the existing numbering scheme in `research/` (next would be `08-`)
- New project hauling plans should follow the `projects/<name>/hauling-plan.md` pattern
- New operational tools go in `tools/`

## Domain Context

- **Geography:** Mississippi, primarily the I-20 corridor and Jackson metro area
- **Industry:** Aggregate/material hauling for heavy construction (dump trucks, belly dumps, end dumps)
- **Key regulation:** Mississippi Harvest Permit allows 84,000 lbs (above the 80,000 lb federal limit)
- **Timeline:** Peak demand 2026-2028; sustained through 2033+ (Compass Meridian is an 8-year build)
- **Five target projects:** xAI ($20B, Southaven), AWS ($10B, Madison County), Compass ($10B, Meridian), AVAIO ($6B, Brandon), AWS ($3B, Vicksburg)
