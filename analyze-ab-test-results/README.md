# Analyze A/B Test Results

> Udacity — Statistics for Data Analysis Nanodegree, Course 4: Hypothesis Testing

## Overview

End-to-end analysis of an e-commerce A/B test with 69,889 visitors across 3 countries (US, UK, CA). Determines whether a new treatment page significantly improves conversion rates over the existing control page.

## Key Findings

| Metric | Value |
|--------|-------|
| Control Conversion Rate | 10.53% |
| Treatment Conversion Rate | 15.53% |
| Delta | **+5.01 pp** |
| P-value (500 simulations) | **< 0.001** |
| Recommendation | **Implement treatment page** |

## Analysis Structure

### Part I — Descriptive Statistics
- Dataset exploration: 69,889 rows, 3 columns, no missing values
- Country distribution: US (69.9%), UK (25.1%), CA (5.0%)
- Groups evenly split: Treatment (50.4%) vs Control (49.6%)

### Part II — Probability
- Overall conversion rate: 13.0%
- Conditional probabilities by group and country
- Country × Group interaction analysis (no interaction found)

### Part III — Hypothesis Testing
- **H₀**: p_treatment - p_control ≤ 0
- **H₁**: p_treatment - p_control > 0
- Monte Carlo simulation (500 iterations) under the null
- P-value ≈ 0 → reject H₀ at α = 0.05

## Files

| File | Description |
|------|-------------|
| `analyze_ab_test_results_project.ipynb` | Complete Jupyter notebook with code, analysis, and interpretations |
| `Analyze_AB_Test_Results.pptx` | Presentation slide deck (5 slides) |

## Tech Stack

- Python 3, pandas, NumPy, matplotlib
- Jupyter Notebook
- Monte Carlo simulation for hypothesis testing

## Dataset

E-commerce A/B test data with columns:
- `country` — US, UK, CA
- `group` — control, treatment
- `converted` — 0 (no) or 1 (yes)

## License

MIT
