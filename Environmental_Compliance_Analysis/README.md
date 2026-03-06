# Drinking Water Violations — County Analysis

Executive summary
- This notebook analyzes a drinking-water violations dataset to identify systems and counties with elevated violation activity. Key finding: many extreme per-capita violation rates are driven by very small systems, while population-weighted county rates reorder priorities compared with raw system counts. Recommendation: present both per-system and population-weighted county metrics when prioritizing inspections and investigate small-population outliers for data quality or local context.


**Data provenance**
- Source: Pennsylvania Department of Environmental Protection (DEP) — Safe Drinking Water Program
- Snapshot date: January 2026
- Filename used in repo: `Drinking_Water_Violations.csv` (included in this folder)

**Files**
- `Dwv.ipynb` — main Jupyter notebook (narrative, EDA, visuals, modeling outline)
- `Drinking_Water_Violations.csv` — dataset (place locally or provide download instructions)
- `README.md` — this file
- `requirements.txt` — Python dependencies for reproducibility
- `.vscode/settings.json` — workspace interpreter guidance (points to `.venv`)
- `outputs/` — directory (gitignored) for saved CSVs, plots, and HTML exports
- `src/` (optional) — Python modules if refactored out of the notebook
- `scripts/run_analysis.py` (optional) — script to run analysis end-to-end

**Quick reproducibility (local)**
- Recommended Python: `3.9` (adjust to your venv Python minor version)
- Create and activate a virtual environment, install deps:
```bash
# from repo root
python3 -m venv .venv
source .venv/bin/activate
pip install -r [requirements.txt](http://_vscodecontentref_/1)