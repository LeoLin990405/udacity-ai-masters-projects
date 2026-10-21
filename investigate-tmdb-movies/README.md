# Investigate a Dataset: TMDb Movie Analysis

> Udacity Data Analyst Nanodegree — Project 1

## Overview

This project investigates the TMDb (The Movie Database) dataset containing information about **10,878 movies**, including user ratings, revenue, budget, genres, and more. The analysis explores trends in the movie industry through three research questions.

## Research Questions

1. **Which genres are most popular from year to year?** — Genre distribution and trends across decades
2. **What properties are associated with high-revenue movies?** — Relationships between budget, ratings, popularity, runtime, and revenue
3. **How has the movie industry evolved over time?** — Budget and revenue trends by decade, production volume changes

## Key Findings

- **Drama** and **Comedy** dominate across all decades, but **Thriller** and **Adventure** have grown significantly since the 2000s
- **Budget** (r=0.57) and **vote count** (r=0.65) show the strongest correlations with revenue; high ratings alone don't guarantee commercial success
- Median movie budgets and revenues (inflation-adjusted) have grown substantially, with a sharp acceleration in the 2000s
- Movie production volume exploded from ~100/decade (1960s) to 3,000+ (2010s)

## Files

| File | Description |
|------|-------------|
| `Investigate_a_Dataset_TMDb.ipynb` | Jupyter Notebook with full analysis |
| `Investigate_a_Dataset_TMDb.html` | HTML export for easy viewing |
| `tmdb-movies.csv` | TMDb dataset (10,878 movies) |

## Tech Stack

- Python 3, NumPy, pandas, Matplotlib, Seaborn

## Limitations

- Correlation does not imply causation
- ~50% of movies have missing budget/revenue data (replaced with NaN)
- Inflation adjustment (2010 dollars) may not fully capture purchasing power differences
- Genre analysis uses pipe-separated multi-label encoding (one movie can count in multiple genres)
- Dataset is limited to movies listed on TMDb, which may have selection bias

## License

This project is part of the Udacity Masters in AI program.
