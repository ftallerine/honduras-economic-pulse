# Honduras Economic Pulse — CLAUDE.md

## What this project is
A 5-chapter interactive HTML dashboard presenting Honduras economic data.
Single-file HTML chapters. No build system. No framework. Vanilla HTML/CSS/JS only.

## Current phase
Phase 1 — POC with hardcoded dummy data from `data/dummy.json`.

## Chapter map
| File | Chapter | Flagship KPI |
|------|---------|--------------|
| chapter-01-big-picture.html | The Big Picture | GDP, remittances |
| chapter-02-what-honduras-runs-on.html | What Honduras Runs On | GDP by sector |
| chapter-03-how-people-earn.html | How People Earn | Salary vs. minimum wage |
| chapter-04-the-table.html | The Table | Salary-to-basket ratio (2.66x) |
| chapter-05-living-conditions.html | Living Conditions | Poverty rate |

## Key design principles
- Mobile-first, single-file HTML per chapter
- All CSS inline or in a single <style> block at top
- All JS inline at bottom of file in a single <script> block
- Dummy data imported from `data/dummy.json` via fetch() or hardcoded inline
- Charts: use Chart.js via CDN only (no npm)
- No external fonts — system font stack only

## Dummy data
All KPI values live in `data/dummy.json`. Always read from there.
Do not hardcode individual KPI values in HTML files.

## Sprint board
Notion: https://app.notion.com/p/04718f27ce7e43d59febdaf5374bc2ed
Sprint 1 (Jun 6–12): chapter-04, chapter-01, dummy dataset

## Phases (do not build ahead)
- Phase 1: HTML POC, dummy data ← YOU ARE HERE
- Phase 2: Real data APIs (World Bank, INE, BCH)
- Phase 3: Interactive geo map (Leaflet.js)
- Phase 4: Live Claude API for AI insight panel

## AI insight panel
Each chapter has a static placeholder insight blurb in Phase 1.
Real Claude API integration is Phase 4 only — do not wire up API calls now.

## Git workflow
- Remote: `ftallerine/honduras-economic-pulse` on GitHub
- Branch: `master` is the main branch — no force-pushes
- Commit messages: include `PULSE-###` for work tied to a sprint board story (triggers Notion sync via GitHub Action)
- PRs merged to `master` with `PULSE-###` in title or body auto-close the Notion story to "Done"

## What NOT to do
- Do not install npm packages
- Do not create a build system or bundler
- Do not use React, Vue, or any JS framework
- Do not fetch real external APIs in Phase 1
- Do not split CSS/JS into separate files (keep each chapter self-contained)
