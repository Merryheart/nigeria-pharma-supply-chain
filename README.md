# Nigeria Pharmaceutical Supply Chain Analysis

## Project Overview
An end-to-end data analysis project examining Nigeria's pharmaceutical supply chain, 
modelled on Bloom Public Health's operations — Nigeria's leading supply chain management 
firm and winner of the West Africa Brand Excellence Award 2025.

## Dataset
- **Rows:** ~700 records
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

## Status
🔄 In Progress
