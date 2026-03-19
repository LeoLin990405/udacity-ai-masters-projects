# Model Salary Data with Linear Regression

> Udacity — Statistics for Data Analysis Nanodegree, Course 5: Linear and Logistic Regression

## Overview

Multiple linear regression analysis on 373 employees to identify factors significantly associated with salary. The final model explains 91.5% of salary variance using 7 features.

## Key Findings

| Variable | Coefficient | 95% CI | Significant |
|----------|------------|--------|-------------|
| Years of Experience | +$5,104/yr | ($4,756, $5,453) | Yes |
| PhD (vs Bachelor's) | +$23,081 | ($17,652, $28,510) | Yes |
| Director title | +$24,981 | ($18,092, $31,869) | Yes |
| Senior title | +$14,446 | ($10,867, $18,026) | Yes |
| Master's (vs Bachelor's) | +$14,037 | ($10,041, $18,033) | Yes |
| Male | +$7,630 | ($4,716, $10,544) | Yes |
| Manager title | +$4,285 | ($701, $7,869) | Yes |

**Model: R² = 0.9145, Adjusted R² = 0.9128**

## Analysis Structure

### Part I — Data Description
- 375 employees, 2 rows dropped for missing values
- Salary range: $350 – $250,000 (mean: $100,577)
- Strong correlation between experience and salary (r = 0.92)

### Part II — Regression
- Full model with 10 features → 3 removed (not significant)
- Reduced model with 7 significant predictors

### Part III — Interpretation
- Coefficient interpretation with confidence intervals
- Salary prediction example and residual analysis
- Model diagnostics (residual plots, R², F-test)

## Files

| File | Description |
|------|-------------|
| `salary_prediction_project.ipynb` | Complete Jupyter notebook |
| `Model_Salary_Linear_Regression.pptx` | Presentation slides (5 slides) |

## Tech Stack

Python 3, pandas, NumPy, matplotlib, statsmodels

## License

MIT
