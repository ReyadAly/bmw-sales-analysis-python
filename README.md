# bmw-sales-analysis-python
Python EDA analyzing 50,000 BMW car sales records: revenue, regional performance, model pricing, fuel types, and sales classification.


**Date:** 17th May, 2026  
**Tool:** Python (pandas, matplotlib, seaborn)  
**Author:** Reyad Aly  
**Dataset:** BMW_Car_Sales_Classification (attached to the repo)

## Objectives & Visualizations

1. Total revenue by year (Line chart)
2. Total sales volume by year (Area chart)
3. Total sales and revenue by region (Bar charts)
4. Total sales by model (Bar chart)
5. Average price by model across regions (Bar chart)
6. Total sales by top 5 models and colors (Stacked histogram)
7. Total sales by fuel type % (Pie chart)
8. Revenue distribution by mileage category and transmission (Violin plot)
9. Pairplot of key variables (Pairplot)
10. Top 5 engine sizes by sales volume distribution (Box plot)
11. Price distribution by sales classification (Histogram)


## Key Insights
- Revenue peaked at **$1.34 trillion in 2022**, a 6.5% increase over 14 years
- Regional distribution is nearly **equal across 6 regions** (~16-17% each)
- **Hybrid leads** fuel type sales (64.5M units), Diesel trails (62.4M)
- Top revenue engines: **2.5L and 1.9L**, smallest/largest engines contribute least
- Higher-mileage vehicles (150k+ km) generate the **most total revenue ($4.80T)**

## Data Engineering
- Created `Total` column: `Price_USD × Sales_Volume`
- Created `Mileage_Category` using `pd.cut()`:
  - 0–50k, 50–100k, 100–150k, 150k+

## Libraries Used
```python
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
import numpy as np
```


## Files Included
| File | Description |
|---|---|
| `BWM_Analysis_RA.ipynb` | Main Jupyter notebook |
| `BWM_Analysis_RA.html` | HTML version of the main file |
| `BMW_Car_Sales_Classification.csv` | Dataset |


## How to Run
1. Download the dataset from the repo and place it in the same folder
2. Update the file path in the first cell
3. Run all cells (Kernel → Restart & Run All)


## License
MIT License
