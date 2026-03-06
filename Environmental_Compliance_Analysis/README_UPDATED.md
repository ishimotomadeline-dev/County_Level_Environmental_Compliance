# Drinking Water Violations — County Analysis

## Executive Summary
This project analyzes drinking-water system violations to identify compliance risks at the system and county level. I found that small system size, not system type, drives violation rates. Population-weighted county metrics reveal where real people are most exposed—a critical insight that differs from raw system counts.

## Methods & Findings
- Computed violation rate as violations per 1,000 residents (standardized metric for fair comparison).
- Ran Kruskal-Wallis test (p=0.796): system type does NOT predict violation rate.
- Ran Spearman correlation (rho=-0.971, p<0.001): strong negative correlation between population and violation rate.
- Fit Negative-Binomial GLM (population offset): confirmed population is the dominant driver.
- Flagged high-risk small systems for human inspection.
- Built county-level metrics (both average and population-weighted) to guide resource allocation.


## How to Reproduce
```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r Environmental_Compliance_Analysis/requirements.txt
jupyter notebook Environmental_Compliance_Analysis/Dwv.ipynb
```

## Key Files
- `Dwv.ipynb` — main notebook
- `Dwv_executed.ipynb` — executed notebook with outputs
- `requirements.txt` — dependencies
- `requirements_pinned.txt` — pinned versions for reproducibility

## Data
The dataset (`Drinking_Water_Violations.csv`) contains system metadata and 3-year violation counts. No personal data is included; only system names, IDs, counties, and aggregated metrics.
