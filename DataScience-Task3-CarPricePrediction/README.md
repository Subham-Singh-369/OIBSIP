# Car Price Prediction with Machine Learning

## Objective
Build a regression model that predicts the selling price of a used car
based on features such as brand, age, mileage, fuel type, and transmission.

## Dataset
Source: [Vehicle dataset from cardekho — Kaggle](https://www.kaggle.com/datasets/nehalbirla/vehicle-dataset-from-cardekho)

4,340 used car listings with columns: name, year, selling_price, km_driven,
fuel, seller_type, transmission, owner. The raw CSV is included in this
folder as `car_data.csv`.

## Tech Stack
Python, pandas, scikit-learn, matplotlib, seaborn, Jupyter Notebook (Google Colab)

## Approach
1. Cleaned the dataset — removed 763 duplicate rows (17.6% of the data)
2. Feature engineering: extracted `car_age` from year, `brand` from car name
3. EDA: price distribution, price vs. fuel type, price vs. car age
4. One-Hot encoded categorical variables (fuel, seller_type, transmission, owner, brand)
5. Correlation heatmap on numeric features
6. Trained two models: Linear Regression and Random Forest Regressor
7. Evaluated using MAE, RMSE, and R²
8. Generated feature importance chart for the best model

## Results
| Model | MAE | RMSE | R² |
|---|---|---|---|
| Linear Regression | ₹180,194.99 | ₹385,606.09 | 0.5384 |
| Random Forest Regressor | ₹158,970.51 | ₹368,858.98 | 0.5776 |

**Best model:** Random Forest Regressor — lower error and higher R² than
Linear Regression, reflecting the non-linear nature of car depreciation
and pricing.

## How to Run
Open `Car_Price_Prediction.ipynb` in Google Colab or Jupyter Notebook.
The dataset CSV is included in this folder.
