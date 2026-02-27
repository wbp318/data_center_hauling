# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Repository Is

This is a **business planning and research repository** (not a software codebase) for launching a Mississippi aggregate hauling company targeting the $49B data center construction boom. All content is Markdown documents, a CSV financial model, and planning tools — there are no build systems, tests, or application code.

## Repository Structure

- `BUSINESS-PLAN.md` — Full 16-section business plan (the master document; other files elaborate on sections within it)
- `README.md` — Public-facing summary with financial tables, project table, equipment guide, and repo file tree
- `TODO.md` — Task tracker; move items to "Completed" when finished
- `research/` — Numbered deep-dive files (`01-` through `07-`), next would be `08-`
- `projects/` — Site-specific hauling plans: `projects/<name>/hauling-plan.md` for each of the 5 data center projects
- `tools/` — Operational documents: financial models, templates, contact tracker, checklists

## Sources of Truth

These files are canonical — update them directly rather than duplicating their data elsewhere:

| Data | Canonical file |
|---|---|
| Business plan (all sections) | `BUSINESS-PLAN.md` |
| Financial projections (5-year P&L) | `tools/financial-model.csv` |
| Monthly cash flow (Year 1) | `tools/monthly-cash-flow.md` |
| Contacts (quarries, contractors, agencies) | `tools/contact-tracker.md` |
| Competitor data | `research/06-competitive-analysis.md` |
| Used equipment market data | `research/07-used-equipment-listings.md` |

## Cross-File Consistency Rules

When financial figures, project details, or startup costs change, these files must stay in sync:

- **Financial figures** → `BUSINESS-PLAN.md` ↔ `README.md` (Financial Overview tables) ↔ `tools/financial-model.csv` ↔ `tools/monthly-cash-flow.md`
- **Project table** (names, locations, investment amounts, status) → `BUSINESS-PLAN.md` ↔ `README.md` ↔ `research/01-mississippi-data-center-projects.md`
- **Equipment costs** → `BUSINESS-PLAN.md` ↔ `README.md` (Equipment Guide table) ↔ `tools/truck-comparison.md`

## When Adding New Content

- New research topics → `research/08-<topic>.md` (follow the numbered prefix scheme)
- New project hauling plans → `projects/<name>/hauling-plan.md`
- New operational tools/templates → `tools/`
- New contacts → add to `tools/contact-tracker.md`, not scattered in other files

## Domain Context

- **Geography:** Mississippi, primarily the I-20 corridor and Jackson metro area
- **Industry:** Aggregate/material hauling for heavy construction (dump trucks, belly dumps, end dumps)
- **Key regulation:** Mississippi Harvest Permit allows 84,000 lbs (above the 80,000 lb federal limit)
- **Timeline:** Peak demand 2026-2028; sustained through 2033+ (Compass Meridian is an 8-year build)
- **Five target projects:** xAI ($20B, Southaven), AWS ($10B, Madison County), Compass ($10B, Meridian), AVAIO ($6B, Brandon), AWS ($3B, Vicksburg)
