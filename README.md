# 🇭🇳 Honduras Economic Pulse

A 5-chapter interactive HTML dashboard presenting Honduras economic data — KPI cards, charts, food basket table, and an AI insight panel.

## Structure

```
honduras-economic-pulse/
├── index.html                          ← Landing page / chapter nav
├── data/dummy.json                     ← All KPI data (Phase 1 hardcoded)
├── chapters/
│   ├── chapter-01-big-picture.html
│   ├── chapter-02-what-honduras-runs-on.html
│   ├── chapter-03-how-people-earn.html
│   ├── chapter-04-the-table.html       ← Sprint 1 flagship
│   └── chapter-05-living-conditions.html
└── shared/
    ├── styles.css
    └── design-tokens.md
```

## Running it

No build step. Open `index.html` directly in a browser, or use a local server:

```
npx serve .
```

## Phases

- **Phase 1** (now): HTML POC with hardcoded dummy data
- **Phase 2**: Real data APIs (World Bank, INE Honduras, BCH)
- **Phase 3**: Interactive geo map (Leaflet.js)
- **Phase 4**: Live Claude API for AI insight panel

## Notion
[Sprint board](https://app.notion.com/p/04718f27ce7e43d59febdaf5374bc2ed) · [Project home](https://app.notion.com/p/3548d3d8f1cc81e5b8a4ccb7a6c68b61)
