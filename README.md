# Data Analytics Portfolio

## Environmental Compliance Analysis

Statistical analysis of drinking-water system violations across 9 counties in Pennsylvania. The project demonstrates end-to-end data analysis: cleaning, EDA, hypothesis testing, statistical modeling, and actionable insights.

**Key Finding:** Population size drives violation rates, not system type. Small systems appear riskier due to statistical effects, not necessarily worse compliance.

**Methods:** Kruskal-Wallis test, Spearman correlation, Negative-Binomial GLM with population offset.

**Deliverable:** System-level risk flags and county-level exposure-weighted metrics for inspection prioritization.

---

## Setup
```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r Environmental_Compliance_Analysis/requirements.txt
jupyter notebook Environmental_Compliance_Analysis/Dwv.ipynb
```

See `Environmental_Compliance_Analysis/README_UPDATED.md` for details.
