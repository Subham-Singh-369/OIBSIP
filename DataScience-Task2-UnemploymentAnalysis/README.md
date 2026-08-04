# Unemployment Analysis with Python

## Objective
Perform exploratory data analysis on unemployment data to uncover regional
and temporal trends, with a focus on the impact of the COVID-19 pandemic
on unemployment rates in India.

## Dataset
Source: [Unemployment in India — Kaggle](https://www.kaggle.com/datasets/gokulrajkmv/unemployment-in-india)

Contains monthly unemployment rate, estimated employed, and labour
participation rate by state, spanning 2019–2020 (pre-COVID and COVID-era).
The raw CSV is included in this folder as `Unemployment_in_India.csv`.

## Tech Stack
Python, pandas, matplotlib, seaborn, Jupyter Notebook (Google Colab)

## Approach
1. Loaded and cleaned the dataset (removed 28 fully-blank rows, converted
   Date to datetime, extracted Month/Year)
2. Performed EDA: descriptive statistics, region-wise and month-wise trends
3. Time-series line chart of unemployment rate for 3 states (Andhra Pradesh,
   Maharashtra, Delhi)
4. Bar chart of top 10 states by average unemployment rate
5. Correlation heatmap between unemployment rate, employment, and labour
   participation rate
6. Pre-COVID vs. post-COVID comparison (cutoff: March 2020)

## Key Findings
- Unemployment rate nearly **doubled** post-COVID: 9.51% → 17.77%
- Estimated employment **dropped** by ~950,000 on average
- Labour participation rate **fell** from 43.9% to 39.3%, indicating people
  exited the labour force entirely during the pandemic
- Tripura and Haryana had the highest average unemployment rates over the
  full period, though this is influenced by the COVID-era spike

## How to Run
Open `Unemployment_Analysis.ipynb` in Google Colab or Jupyter Notebook.
Requires the "Unemployment in India" dataset CSV (from Kaggle) to be
uploaded/available in the working directory.
