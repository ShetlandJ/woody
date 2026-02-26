# Woody Boat

C&P (Coating & Protection) audit tool for ship compartments. Single-file app (`index.html`) — all HTML, CSS, and JS self-contained, no build step.

## What it does

- Ship silhouette SVG with labeled compartment blocks (A-H sections)
- Findings table below — enter RAG status, company, unit codes, themes
- RAG dots auto-appear on the ship diagram — one dot per finding, multiple findings show multiple dots
- Unit field maps to compartments: "UB14" highlights B14, "UD23/UD32" highlights both
- Compartment border highlights with worst RAG status (Red > Amber)
- Click any compartment block to set comma-separated label aliases (e.g. "D22, UD22, 196")
- Multi-boat support: create/switch/rename/delete boats, each with own labels + findings
- CSV export per boat
- All data in `localStorage` (`woody_boats` key, `woody_active_boat` for selection)
- Labels stored as arrays per compartment, migrates old string format automatically

## Tech

- Vanilla HTML/CSS/JS, no frameworks
- SVG compartment blocks rendered by JS from `DEFAULT_COMPARTMENTS` array
- Google Fonts (DM Mono), dark theme, responsive
