# Woody Boat

C&P (Coating & Protection) audit tool for ship compartments. Single-file app (`index.html`) — all HTML, CSS, and JS self-contained, no build step.

## What it does

- Ship silhouette SVG with labeled compartment blocks (A-H sections)
- Findings table below — enter RAG status, company, unit codes, themes
- RAG dots auto-appear on the ship diagram (worst status wins per compartment)
- Unit field maps to compartments: "UB14" highlights B14, "UD23/UD32" highlights both
- Click any compartment block to rename its label
- Multi-boat support: create/switch/rename/delete boats, each with own labels + findings
- CSV export per boat
- All data in `localStorage` (`woody_boats` key)

## Tech

- Vanilla HTML/CSS/JS, no frameworks
- SVG compartment blocks rendered by JS from `DEFAULT_COMPARTMENTS` array
- Google Fonts (DM Mono), dark theme, responsive
