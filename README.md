# Data Analytics Portfolio

## Environmental Compliance Analysis

This project analyzes drinking-water system violations in Pennsylvania and presents a full analytics workflow: data cleaning, exploratory analysis, statistical testing, interpretable modeling, and communication of results.

**Project framing:** This notebook demonstrates data cleaning, statistical testing, modeling, and plain-language communication in a public-sector data context.

**Core finding:** Population size explains much more of the observed violation-rate pattern than system type. Small systems often look riskier because per-capita rates become unstable when the served population is very small.

**Methods used:** Exploratory data analysis, Kruskal-Wallis testing, Spearman correlation, Negative-Binomial GLM with population offset, and a small-sample logistic regression workflow with Leave-One-Out cross-validation.

**Scope of the data:** The notebook works with 9 systems that have complete system-level fields and 6 counties with sufficient data for the county-level modeling section.

---

## Open The Project

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r Environmental_Compliance_Analysis/requirements.txt
jupyter notebook Environmental_Compliance_Analysis/Dwv.ipynb
```

For project-specific context, see `Environmental_Compliance_Analysis/README.md`.
