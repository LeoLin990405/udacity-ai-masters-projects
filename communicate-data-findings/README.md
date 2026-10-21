# Communicate Data Findings: Ford GoBike Analysis

> Udacity Data Analyst Nanodegree — Project 3

## Overview

This project explores the Ford GoBike bike-sharing system dataset (February 2019), containing **183,412 trip records** from the San Francisco Bay Area. The analysis investigates usage patterns, trip duration characteristics, and behavioral differences between subscriber and customer user types.

## Research Questions

1. What factors affect trip duration in the bike-sharing system?
2. How do usage patterns differ between subscribers and customers?
3. What are the temporal patterns (hourly, daily) of bike usage?

## Key Findings

- **Trip duration** follows a log-normal distribution; most trips are 5–15 minutes (median ~8.5 min)
- **Subscribers** (90%) take short, routine commute trips with clear weekday rush-hour peaks (8–9 AM, 5–6 PM)
- **Customers** (10%) take longer exploratory rides, more evenly distributed across weekends
- **Weekday vs. weekend** patterns are strikingly different, driven primarily by subscriber commute behavior

## Files

| File | Description |
|------|-------------|
| `Part_I_exploration.ipynb` | Exploratory analysis (9 visualizations) |
| `Part_I_exploration.html` | HTML export of Part I |
| `Part_II_explanatory.ipynb` | Explanatory analysis (4 polished visualizations) |
| `Part_II_explanatory.html` | HTML export of Part II |
| `201902-fordgobike-tripdata.csv` | Ford GoBike trip data (Feb 2019) |

## Visualizations

### Part I (Exploratory)
1. Histogram — trip duration distribution (log scale)
2. Count plot — user type distribution
3. Bar chart — trips by hour of day
4. Scatter plot — hour vs duration
5. Box plot — duration by user type
6. Heatmap — day-of-week × hour
7. Faceted box plot — duration by day × user type
8. Line chart — hourly patterns by user type
9. Pair plot — multi-feature relationships

### Part II (Explanatory)
1. Polished histogram with median/mean annotations
2. Heatmap with peak-hour annotations
3. Grouped line chart with commute-hour shading
4. Box plot with inline statistics

## Tech Stack

- Python 3, NumPy, pandas, Matplotlib, Seaborn

## License

This project is part of the Udacity Masters in AI program.
