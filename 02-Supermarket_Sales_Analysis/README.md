# Global Sustainability & Happiness Analysis

**Tools:** Python, Pandas, Matplotlib, Seaborn, NumPy  
**Dataset:** Global Sustainability & Peace Index (GSPI) — 140 countries  

---

## Overview

This project looks at what actually drives national happiness across 140 countries. Using the GSPI dataset, I analysed the relationships between economic output, governance quality, environmental health, and human development to see which factors matter most — and which are overstated.

The analysis moves beyond the obvious GDP assumption and finds that institutional quality and human development are stronger predictors of wellbeing than income alone.

---

## Questions Explored

1. Does higher GDP per capita lead to greater happiness?
2. Which regions lead and lag on happiness vs pollution?
3. How strongly does governance quality predict happiness?
4. Is HDI a better predictor than GDP?
5. Which variables are most correlated with national happiness overall?

---

## Dataset Variables

| Variable | Description |
|---|---|
| Happiness Index | Self-reported life satisfaction (0-10 scale) |
| GDP per Capita | Economic output per person (USD) |
| HDI | Human Development Index — combines income, education, and health |
| Corruption Index | Higher score = less corrupt, better governance |
| PM2.5 | Particulate matter air pollution (µg/m³) |
| Life Expectancy | Average years of life at birth |
| Education Index | Access and quality of education |
| Renewable Energy | Share of energy from renewable sources (%) |
| Urbanisation | Share of population in cities (%) |

---

## Key Findings

| Insight | Finding |
|---|---|
| GDP vs Happiness | Relationship is logarithmic — gains plateau above approximately USD 20,000 per capita |
| Regional comparison | Europe leads on happiness and has the lowest average pollution; Africa and Asia face both low happiness and high PM2.5 |
| Governance | Corruption Index (r = 0.74) is a strong independent predictor of happiness, holding across income levels |
| HDI vs GDP | HDI (r = 0.80) outperforms GDP alone — health and education matter more than raw income |
| Correlation heatmap | Life expectancy and HDI dominate; PM2.5 has a meaningful negative relationship with happiness |

---

## Setup

Install dependencies:
```bash
pip install pandas openpyxl matplotlib seaborn numpy
```

Place the GSPI dataset at:
```
data/gspi_dataset.xlsx
```

Then open and run `global_sustainability_analysis.ipynb` top to bottom.

Charts are saved to an `outputs/` folder which is created automatically on first run.

---

*Divyanshi Shaw — Master of Business Analytics, Deakin University*
