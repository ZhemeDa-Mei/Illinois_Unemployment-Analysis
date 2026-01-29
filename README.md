# Illinois Unemployment Data Analysis

## Overview

This project analyzes how unemployment rates have evolved across major metropolitan areas in Illinois from 1990 to 2025.

Rather than focusing on a single statewide average, the analysis compares city-level unemployment dynamics over time to identify whether metropolitan areas tend to move together, or whether persistent structural differences exist between cities.

The goal is not to predict unemployment, but to understand which observed patterns are likely structural and which conclusions require caution when interpreting time-series data.

---

## Research Questions

This analysis focuses on three core questions:

1. How has unemployment evolved over time across Illinois metropolitan areas?
2. Are there cities that consistently experience higher or lower unemployment relative to others?
3. How do different economic shocks (e.g. the 2008 financial crisis vs. the COVID-19 shock) differ in terms of divergence, convergence, and recovery speed across cities?

---

## Data & Methodology

- Data source: Federal Reserve Economic Data (FRED)
- Dataset: Unemployment Rate by Metropolitan Statistical Area, Monthly, Smoothed Seasonally Adjusted
- Original provider: U.S. Bureau of Labor Statistics (BLS)
- Link: [fred.stlouisfed.org/](https://fred.stlouisfed.org/release/tables?rid=113&eid=181532#snid=181543)


The dataset contains monthly unemployment rates for selected Illinois metropolitan statistical areas (MSAs) from 1990 to 2025.

The analysis is primarily descriptive and focuses on:
- Long-term trends
- Relative differences between cities
- Time-window comparisons around major economic shocks

To improve interpretability, unemployment trends are examined both over the full sample and within selected time windows (e.g. pre- and post-crisis periods).

---

## Key Findings

- Across the full period, Illinois metropolitan areas generally move in the same direction over time, suggesting strong common macroeconomic influences.
- Despite shared trends, persistent level differences exist:
  - Some cities (e.g. St. Louis, Springfield, Champaign-Urbana) tend to exhibit relatively lower unemployment rates.
  - Others (e.g. Danville, Decatur) consistently experience higher unemployment levels.
- Volatility differs substantially across cities:
  - Certain metropolitan areas display smoother unemployment paths.
  - Others show larger cyclical swings, particularly during economic downturns.
— Central Tendency and Representative Cities
  -Beyond extremes and volatility, some metropolitan areas appear to function as representative benchmarks of overall unemployment conditions within Illinois, though this role shifts over time.
  -Before the 2007–2008 financial crisis, Davenport–Moline–Rock Island frequently occupied a central position within the cross-city distribution, closely tracking the statewide average pattern.
  -After 2007, Chicago–Naperville–Elgin increasingly assumed this role, with its unemployment rate often aligning near the middle of the metropolitan range.
  -This shift suggests that the city most representative of statewide labor market conditions is not fixed, but evolves with structural and economic changes over time.

---

## Interpretation & Caution

Comparing different economic shocks reveals important timing differences:

- During the 2008–2009 financial crisis, unemployment rose gradually and remained elevated for several years before a slow recovery.
- In contrast, the COVID-19 shock in 2020 produced a sharp, synchronized spike across cities, followed by a relatively rapid recovery.

These differences highlight that similar peak unemployment levels can reflect very different underlying dynamics. Conclusions based solely on point-in-time comparisons may therefore be misleading without considering the broader time context.

---

## Repository Structure

- `data/`  
  Raw unemployment data downloaded from FRED.

- `notebooks/`  
  Jupyter notebook containing data processing, visualization, and analysis.

- `figures/`  
  Line charts and time-window visualizations used in the analysis.



