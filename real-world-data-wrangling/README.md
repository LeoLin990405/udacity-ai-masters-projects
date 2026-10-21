# Real World Data Wrangling with Python

> Udacity Data Analyst Nanodegree — Project 2

## Overview

This project demonstrates the complete data wrangling process using two real-world datasets: FBI NICS firearm background check data and US Census demographic data. The analysis explores how state-level demographic and economic characteristics relate to firearm background check activity.

## Research Question

**How do state-level demographic and economic characteristics relate to firearm background check activity, and which factors are most strongly associated with per-capita background check rates?**

## Key Findings

- **Income correlation**: States with lower median household incomes tend to have higher per-capita firearm background check rates
- **Education link**: States with lower bachelor's degree attainment show higher per-capita check rates
- **Regional patterns**: Kentucky, Utah, and West Virginia lead in per-capita checks; states like New York and New Jersey are at the bottom
- **Strongest correlate**: Median household income (r ≈ -0.4) shows the strongest inverse relationship with per-capita checks

## Data Gathering Methods

| Dataset | Method | Source | Rows |
|---------|--------|--------|------|
| FBI NICS Background Checks | Manual Download (CSV) | FBI NICS | 12,485 |
| US Census Demographics | SQL Database (SQLite) | US Census Bureau | 86 facts × 51 states |

## Data Wrangling Summary

### Quality Issues
1. Extensive missing values in gun_data (columns with >50% NaN dropped)
2. Inconsistent data types in census data (commas, percentages, footnote markers)

### Tidiness Issues
1. Census data in wide format (states as columns → melted to rows)
2. Same observational unit in separate tables (merged on state)

## Files

| File | Description |
|------|-------------|
| `Real_World_Data_Wrangling.ipynb` | Complete Jupyter Notebook |
| `Real_World_Data_Wrangling.html` | HTML export |
| `gun_data.csv` | Raw FBI NICS data |
| `us_census_data.csv` | Raw US Census data |
| `census_data.db` | SQLite database |
| `cleaned_combined_data.csv` | Final cleaned dataset (50 states × 14 variables) |

## Tech Stack

- Python 3, NumPy, pandas, Matplotlib, Seaborn, sqlite3

## Limitations

- Census data is from a single snapshot (~2016), while gun data spans multiple years
- Per-capita normalization uses total population, not adult population
- Correlation does not imply causation
- Some census metrics have missing values for certain states

## License

This project is part of the Udacity Masters in AI program.
