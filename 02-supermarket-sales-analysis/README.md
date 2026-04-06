# Supermarket Sales Analysis

**Tools:** Python, Pandas, Matplotlib, Seaborn, SQL (SQLite)  
**Dataset:** Supermarket Sales — 1,000 transactions across 3 branches, January to March 2019  
**Data source:** [Kaggle — Supermarket Sales Dataset](https://www.kaggle.com/datasets/aungpyaeap/supermarket-sales)

---

## Overview

This project analyses retail transaction data from a three-branch supermarket chain. The goal was to surface practical business insights around branch performance, product profitability, and customer behaviour — combining Python visualisation with SQL querying in a single workflow.

This reflects how a business analyst might work in practice: using Python for visual exploration and SQL for structured, repeatable queries against the same underlying data.

---

## Business Questions

1. Which branch generates the most revenue, and which has the highest customer satisfaction?
2. Which product lines are most and least profitable?
3. Do member customers spend more than non-members?
4. What payment methods do customers prefer?
5. How does revenue trend across the three-month period?

---

## Dataset Variables

| Column | Description |
|---|---|
| Branch | Store location — A, B, or C |
| Product line | Category of goods purchased |
| Total | Transaction value in USD including tax |
| Customer type | Member or Normal |
| Payment | Cash, Credit card, or Ewallet |
| Rating | Customer satisfaction score out of 10 |
| Date | Transaction date |

---

## What the Notebook Contains

**Section 1 — Setup and data loading**  
Reads the dataset, parses dates, and prints a summary of the data shape and date range.

**Section 2 — Visual dashboard**  
A six-panel figure covering all five business questions: revenue by branch, sales by product line, member vs normal split, payment preferences, average rating by branch, and monthly revenue trend.

**Section 3 — SQL analysis**  
Loads the dataframe into an in-memory SQLite database and runs four structured queries covering revenue by branch, product line performance, customer type comparison, and branch rating vs average sale value.

**Section 4 — Summary findings**  
A findings table translating each result into a concrete business recommendation.

---

## Key Findings

| Question | Finding | Recommendation |
|---|---|---|
| Branch revenue | All three branches within 3% of each other | No single branch dominates — network is well balanced |
| Product lines | Food and Beverages and Sports and Travel lead on revenue | Prioritise shelf space and promotions for these categories |
| Member vs Normal | Revenue split is close to 50/50 with similar basket sizes | Membership drives volume but not higher spend per visit |
| Payment method | Ewallet, cash, and credit card are evenly distributed | Maintain all three options — no single dominant preference |
| Revenue trend | February dips before recovering in March | Targeted mid-quarter promotions could smooth seasonal drop |
| Customer ratings | All branches rate between 6.9 and 7.1 out of 10 | Consistent but moderate — room to improve across the network |

---

## Setup

Install dependencies:
```bash
pip install pandas openpyxl matplotlib seaborn
```

Download the dataset from [Kaggle](https://www.kaggle.com/datasets/aungpyaeap/supermarket-sales) and place it at:
```
data/supermarket_sales.xlsx
```

Then open and run `supermarket_sales_analysis.ipynb` top to bottom.

---

*Divyanshi Shaw — Master of Business Analytics, Deakin University*
