# Housing Affordability and Telecommunication Expansion

## Overview

This project explores the intersection of housing affordability and strategic telecom infrastructure expansion. Using public datasets from Zillow and the U.S. Census Bureau, the goal is to identify which cities in **Ohio, Pennsylvania, and Michigan** present strong opportunities for fiber internet deployment based on income and housing cost metrics.

As a telecommunications industry professional with over a decade of experience, I undertook this analysis to help fast-growing telecom startups take a data-driven approach to market selection, rather than relying on traditional or reactive methods.

## Business Problem

**How can a telecommunications startup prioritize cities for fiber network expansion using housing affordability and income data?**

By identifying affordable cities with growing potential, the company can:
- Reduce upfront construction costs
- Expand in areas underserved by high-speed internet
- Leverage existing regional infrastructure

## Data Sources

- **Zillow Research (2025)**  
  - Zillow Home Value Index (ZHVI) – Middle price tier  
  - Estimated income required for 20% down payment  
  - https://www.zillow.com/research/data/

- **U.S. Census Bureau (2023)**  
  - Median household income  
  - Income by race (aggregated for neutrality)  
  - https://data.census.gov/

## Methodology

- Combined and cleaned city-level housing price data with state-level income data.
- Calculated an **Affordability Ratio**:  
  `Affordability Ratio = Income Needed / Median Home Price`
- Built two predictive models:
  - **Logistic Regression** (baseline model; low accuracy)
  - **Random Forest Classifier** (final model; 88% accuracy, 100% recall)

## Key Findings

- **Philadelphia, Columbus, and Pittsburgh** emerged as consistently affordable cities with strong potential for telecom expansion.
- The Random Forest model effectively predicted cities likely to remain in or join the top 20 most affordable markets.
- The model is a useful guide for early-stage business development teams to prioritize construction investment.

## Tools and Technologies

- Python (Jupyter Notebook)
- Pandas, NumPy
- Scikit-learn (Random Forest, Logistic Regression)
- Matplotlib / Seaborn

## Limitations and Future Work

- **Income data is slightly dated** (2023); updated inputs would improve predictions.
- **Race-specific data** was ethically aggregated to ensure neutrality in model decision-making.
- **Metro-level income data** could enhance precision but was unavailable during this phase.
- Future improvements include:
  - Incorporating **population growth**
  - Adding **existing broadband infrastructure** data
  - Enabling **dynamic re-training** for economic shocks (e.g., inflation, recession)

## Recommendations

- Use model outputs as a **first-pass filter** for market selection.
- Perform deeper market research on predicted cities before committing to capital-intensive builds.
- Periodically update the dataset and retrain the model to ensure relevance.

## File Descriptions

- `Brionez680Week2and3.ipynb` – Jupyter Notebook containing EDA, affordability calculations, and machine learning model implementation
- `Project1 White Pages.docx` – Formal white paper summarizing business case, methods, results, and recommendations

---

Ruben Brionez Jr  
June 2025 – DSC680 Final Project  
Bellevue University
