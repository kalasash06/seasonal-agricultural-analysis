# Seasonal Agriculture Performance Analysis

**VOIS AICTE Batch1 2026-2027 — Major Project**

## Problem Statement
Agricultural performance varies across seasons due to differences in environmental conditions,
resource usage, and market factors. This project analyzes a farm-level dataset to identify
meaningful seasonal patterns, trends, and relationships in yield, resource usage, and
economic performance across **Kharif**, **Rabi**, and **Zaid** seasons.

## Dataset
`seasonal_agriculture_performance_dataset.csv` — 4,000 farm records with 28 columns covering:
- Location & crop info (State, District, Crop, Season)
- Environmental conditions (Rainfall, Temperature, Humidity, Sunlight, Soil pH/Moisture)
- Inputs & resources (Fertilizer, Pesticide, Irrigation Method, Water Used)
- Outcomes (Yield, Production, Revenue, Cost, Profit, Water Efficiency, Disease/Pest Risk)

## What the Notebook Covers
1. Data loading, cleaning (missing values, duplicates), and outlier handling (IQR method)
2. Seasonal comparison of yield, environmental conditions, and resource usage
3. Seasonal comparison of economic performance (cost, revenue, profit)
4. Best-performing crops per season
5. Correlation analysis of numeric features
6. One-way ANOVA tests to confirm seasonal differences are statistically significant
7. Impact of irrigation method on yield, by season
8. Key insights and data-driven recommendations

## Key Findings
- Kharif has the highest average yield (2.25 t/ha) and is the most profitable season
  (₹91,700/farm average).
- Zaid has the lowest yield (1.81 t/ha) and runs at an average **loss** (-₹51,600/farm),
  driven by high heat, low rainfall, and poor water efficiency.
- Seasonal differences in yield and profit are statistically significant (ANOVA p < 0.001).
- Drip irrigation consistently gives the best yield across all seasons, with the largest
  benefit in Zaid.

## How to Run (Google Colab)
1. Open [Google Colab](https://colab.research.google.com/).
2. Click **File → Upload notebook** and upload `Seasonal_Agriculture_Performance_Analysis (1).ipynb`
   (or open it directly from GitHub via **File → Open notebook → GitHub** and paste this repo's URL).
3. Upload `seasonal_agriculture_performance_dataset.csv` to the Colab session:
   click the folder icon on the left sidebar → **Upload to session storage**.
4. Run all cells: **Runtime → Run all**.

## How to Run (Locally)
```bash
pip install pandas numpy matplotlib seaborn scipy jupyter
jupyter notebook Seasonal_Agriculture_Performance_Analysis.ipynb
```

## Repository Structure
```
├── Seasonal_Agriculture_Performance_Analysis.ipynb   # Main analysis notebook
├── seasonal_agriculture_performance_dataset.csv      # Dataset
└── README.md                                         # This file
```

## Tools Used
Python, Pandas, NumPy, Matplotlib, Seaborn, SciPy (stats), Jupyter/Google Colab
