# Nigeria Pharmaceutical Supply Chain Analysis

## Project Overview
An end-to-end data analysis project examining Nigeria's pharmaceutical supply chain, 
modelled on Bloom Public Health's operations — Nigeria's leading supply chain management 
firm and winner of the West Africa Brand Excellence Award 2025.

## Dataset
- **Rows:** ~2000 records
- **Source:** Synthetic dataset based on real Nigerian pharma supply chain challenges
- **Coverage:** 36 states + FCT, multiple facility types (PHC, General Hospital, Teaching Hospital)
- **Medicines:** Antimalarials, ARVs, Antibiotics, Vaccines, Analgesics

## Data Quality Issues Identified
- Mixed date formats (YYYY-MM-DD, MM-DD-YYYY, DD/MM/YYYY, DD-Mon-YYYY)
- Negative stock values (data entry errors)
- Inconsistent state name and medicine name casing
- Duplicate Facility IDs across different states
- Status contradictions (expired medicines marked as In_Stock)
- Cold chain compliance flags inconsistent with actual storage conditions
- Zero stock levels with incorrect Status values

## Analysis Angles
1. Stockout & supply risk analysis
2. Cold chain & vaccine integrity
3. Regional disparities (North vs South)
4. Track & Trace coverage & counterfeit risk

## Tools
- Power Query (structural data cleaning)
- Python (cleaning, analysis & exploration)
- Power BI (dashboard)
- GitHub (version control & documentation)
- ## Notebooks
- `01_data_cleaning.ipynb` — Data quality audit and logic-based cleaning
- `02_analysis.ipynb` — Statistical analysis across 4 angles: stockout risk, cold chain, regional disparities, track & trace
- ## Dashboard

![Overview](dashboard/overview.png)
![Stockout & Supply Risk](dashboard/stockout_supply_risk.png)
![Cold Chain & Regional](dashboard/cold_chain_regional.png)
![Track & Trace](dashboard/track_trace_counterfeit.png)

## Status
✅ Complete

## Key Findings
- Only **26% of medicines** are healthy stock — 42% are expired
- **North West** has 4x more at-risk medicines than South West (42.3% vs 9.8%)
- Cold chain failure leads to **5x more wastage** (34.88% vs 6.77%)
- **0% counterfeit risk** where Track & Trace is enabled vs 2.85% where untracked
- Only **17.5%** of medicines have Track & Trace enabled
- **PHCs experience the most stockouts** — 3.15 events per 6 months on average
- North West facilities have only **27.5 days of stock remaining** vs 114.7 days in South West
