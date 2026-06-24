# Work History — Michel Pomares

Full-stack software developer. This repository is a public, verifiable summary of my professional work, currently about one year of contributions on a private company GitLab instance, kept as a portfolio reference for anyone interested in what I build. It contains statistics and summaries only: no source code, proprietary logic, company or client names, or client-confidential material.

All commit metrics below were produced from local git history with `git log --author`, so they reflect only commits authored under my own email.

## Role & focus

- Lead frontend developer on a competition and results-management platform, with substantial contributions to its backend as well.
- Full-stack developer on broadcast-graphics products for top-tier football and winter-sports televised events.
- Frontend developer on football broadcast apps and a maintainer of shared internal React component libraries.

## Tech stack

| Layer | Technologies |
| --- | --- |
| Frontend | React 19, TypeScript, Vite, shadcn/ui, dnd-kit, i18next (DE/EN) |
| Backend | .NET 9, NestJS, Supabase (PostgreSQL / PostgREST) |
| Tooling | Server-side PDF rendering (Gotenberg), GitLab CI, merge-request review workflow |

## Contribution summary

| Metric | Value |
| --- | --- |
| Commits authored | 1,364 across 14 repositories |
| Active days (distinct days with at least one commit) | 188 |
| Activity span | 3 Jul 2025 → 17 Jun 2026 (~1 year) |
| Merge requests authored (primary product) | 256 |
| Merge requests merged (primary product) | 209 |

## Commits by project

| Project | Commits | Detail |
| --- | --- | --- |
| Competition & results platform | 1,246 | frontend 855 · backend 391 |
| Winter-sports broadcast graphics | 46 | results FE 12 · NestJS BE 24 · shooting 10 |
| Football broadcast graphics | 38 | control 20 · backend 9 · tactical 6 · config 2 · db 1 |
| Football broadcast apps | 23 | in-game 23 |
| Shared React libraries | 8 | datahub lib 4 · components lib 4 |
| DataHub | 3 | flow frontend 3 |
| **Total** | **1,364** | |

## Merge requests — primary product (competition & results platform)

| Repo | Authored | Merged |
| --- | --- | --- |
| Frontend | 139 | 115 |
| Backend | 117 | 94 |
| **Total** | **256** | **209** |

Merge-request figures are from the platform's frontend and backend repositories, where the large majority of my merge-request workflow took place. All MRs went through peer code review.

## Scope of work — competition & results platform

The bulk of my work (~91% of commits) was on a platform for planning and running competitions and publishing results. Concrete areas I built or co-built:

- **Competition formats** — Swiss system, round-robin, and bracket/elimination modes, plus divisioning and progression wizards.
- **Start lists & result lists** — configurable columns persisted per discipline, drag-and-drop ordering, aggregation of earlier results.
- **Assignment tooling** — BIB numbers, lane assignment, and staff/personnel management.
- **Import pipelines** — CSV/XLSX import with dry-run preview, validation, and fuzzy matching.
- **Print & export system** — server-side PDF generation (start lists, result lists, blank scoresheets, delegation rosters) via Gotenberg, with per-sport template grouping.
- **Bilingual UI** — full German/English internationalization.
- **Backend** — .NET 9 API over Supabase/PostgREST, including schema migrations, permission gating, and query batching for large datasets.

## Other projects

- **Broadcast graphics (football & winter sports)** — React frontends backed by NestJS services, rendering live on-air graphics (start lists, shooting analysis, tactical lineups) driven by a real-time data hub.
- **Football broadcast apps** — React frontends for in-game and database-driven graphics.
- **Shared libraries** — maintained reusable React component and data-hub libraries consumed across the broadcast products.

## How these numbers were produced

Commit, active-day, and project figures were generated locally with `git log --all --author="<my-email>" --date=short` across every repository I had cloned, then de-duplicated by date. They count only commits authored under my email.

Merge-request figures were read from GitLab's merge-request dashboard, filtered to Author = me, across the Open / Merged / Closed tabs.

No contribution graphs were fabricated and no commit history was altered. Figures are reported as measured.
