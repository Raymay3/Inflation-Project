# Inflation, Employment Growth, and Housing Affordability in the United States (2016–2026)

## Overview

This project analyzes economic trends in the United States between 2016 and 2026 by examining three key indicators:

* Consumer price inflation
* Employment growth across major industries
* Regional housing rent growth

Using data from the U.S. Bureau of Labor Statistics (BLS) and Zillow, the project explores how changes in prices, labor markets, and housing costs may have affected affordability for U.S. households.

## Research Questions

1. How have consumer prices changed between 2016 and 2026?
2. Which industries experienced the greatest employment growth?
3. How has rent growth varied across regions of the United States?
4. What do these trends suggest about housing affordability and cost-of-living pressures?

## Data Sources

### BLS Average Prices

Monthly average consumer prices for selected goods and household items.

### BLS Current Employment Statistics (CES)

Monthly employment counts across industries and sectors.

### Zillow Observed Rent Index (ZORI)

Monthly rent estimates for metropolitan areas throughout the United States.

## Project Structure

```text
.
├── data/
│   ├── Dataset #1 - earnings.txt                # BLS employment data
│   ├── Dataset #2 - inflation.txt               # BLS average prices data
│   ├── Dataset #3 - Metro_zori_uc_sfrcondomfr_sm_month.csv
│   │                                            # Zillow rent index data
│   ├── earnings_ids.txt                         # Employment series lookup table
│   ├── inflation_ids.txt                        # Inflation series lookup table
│   └── regional_index.csv                       # Processed regional rent index
│
├── overview_eda.ipynb                           # Initial exploratory analysis
├── regional_rent_analysis.ipynb                 # Regional housing affordability analysis
├── industry_growth.ipynb                        # Employment growth analysis
├── Headcount_inflation.ipynb                    # Inflation and employment correlation analysis
│
├── industry_employment_growth.png               # Employment growth visualization
├── SIADS 593 - Milestone I Project Report.pdf   # Final project report
└── README.md
```

## Methods

### Inflation Analysis

* Mapped BLS series IDs to product names
* Reshaped data from wide to long format
* Converted prices to indexed values (January 2016 = 100)
* Compared price growth across consumer goods

### Employment Analysis

* Cleaned and transformed CES employment data
* Selected seasonally adjusted employment series
* Calculated employment growth from 2016 to 2026
* Compared growth across major industries

### Housing Analysis

* Filtered Zillow data to metropolitan statistical areas (MSAs)
* Grouped metros into Northeast, Midwest, South, and West regions
* Calculated average regional rents
* Indexed rent values to January 2016 = 100
* Compared regional rent growth trends over time

## Visualizations

The project includes:

* Inflation trend heatmaps and correlation analysis
* Industry employment growth comparisons
* Regional rent growth line charts

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook

## Key Findings

The analyses indicate that:

* Consumer prices increased substantially across many categories during the study period.
* Employment growth varied considerably by industry.
* Rent growth was not uniform across regions, with some areas experiencing much stronger increases than others.
* Combined trends suggest increasing affordability pressures for many U.S. households.

## Authors

Gabriella Gass,
Colten Wasden,
Garret Obenchain
