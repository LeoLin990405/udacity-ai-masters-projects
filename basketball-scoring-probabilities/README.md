# Calculate Basketball Scoring Probabilities

> Udacity — Statistics for Data Analysis Nanodegree, Course 3: Probability

## Overview

Analysis of Steph Curry's 2022-2023 NBA season shooting data (1,434 shots) using binomial distribution, conditional probability, and Bayes' Theorem.

## Key Findings

| Metric | Value |
|--------|-------|
| P(Make) | 49.02% (703/1,434) |
| P(Three-pointer) | 54.81% (786/1,434) |
| P(3 makes in 4 shots) | 24.02% (Binomial) |
| P(Make \| 3pt) | 41.86% (Bayes) |
| P(Make \| 2pt) | 57.72% (Bayes) |
| P(3pt \| Made) | 46.80% (Bayes) |

## Analysis Sections

1. **Overall Shooting Statistics** — P(Make), P(Miss), shot type proportions
2. **Binomial Probabilities** — P(3/4 makes), P(4/5 three-pointers), assumptions
3. **Conditional Probabilities (Future)** — P(Make|shot_type), P(Lead|shot_type) via Bayes
4. **Conditional Probabilities (Past)** — P(shot_type|Made) via Bayes with verification

## Tech Stack

Python 3, pandas, python-pptx

## License

MIT
