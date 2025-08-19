# Manufacturing Energy Flow — Sankey Diagram (RAWGraphs)

**Email (as required):** 23ds3000034@ds.study.iitm.ac.in

This repository contains:
- `chart.png` — Sankey diagram exported from RAWGraphs (300–512 px, PNG).  
- `energy_sankey_data.csv` — Input dataset (flows from sources → conversions → end uses).  
- `energy_sankey_data.tsv` — Same data in TSV format.  

## How to Reproduce (RAWGraphs)
1. Open **https://rawgraphs.io/**
2. **Load your data** → paste the contents of `energy_sankey_data.csv`.
3. **Select chart** → *Sankey Diagram*.
4. **Map the fields**:
   - **Source** → `source`
   - **Target** → `target`
   - **Size** → `flow (MWh/yr)`
   - (Optional) **Color** → `source` (gives intuitive grouping by upstream source / system)
5. **Refine**:
   - Enable **labels** for nodes and links.
   - Set **thousands separator** and **no decimals** for values (e.g., “1,720 MWh”).
   - Choose a **professional palette** (e.g., muted/neutral with distinct hues).
   - Sort nodes to reduce crossings (try *by value* or *alphabetical* per column).
6. **Export** → **PNG** → set **width/height** between **300×300** and **512×512** (recommended: **512×512**).  
   Save as `chart.png` in this repository's root.

## Notes on the Data
- Units: **MWh/year**.
- Multi-level flow: *Sources → Conversion/Distribution → End Uses*.
- Flows are balanced at intermediate nodes (e.g., **Boilers** total inflow = total outflow).
- Designed to be **publication-ready** for annual reports and board decks.

---

© Donnelly and Sons — Strategic Consulting, Advanced Data Visualization & BI.