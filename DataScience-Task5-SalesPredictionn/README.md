# Sales Prediction Using Machine Learning

## Project Overview

This project focuses on predicting product sales based on advertising expenditure across three marketing channels: TV, Radio, and Newspaper. Using regression techniques, the relationship between advertising budgets and product sales is analyzed to build predictive models that can estimate future sales.

The project was developed as part of a Data Science Internship and demonstrates the complete machine learning workflow, including data exploration, visualization, model training, evaluation, and interpretation.

---

## Objective

The objective of this project is to develop a regression model that predicts product sales using advertising spending on different media channels and to identify which advertising channel has the greatest impact on sales.

---

## Dataset

This project uses the classic **Advertising Dataset**, which contains advertising budgets and corresponding sales figures.

**Dataset Source:**

- Kaggle: https://www.kaggle.com/datasets/ashydv/advertising-dataset

### Dataset Features

| Feature | Description |
|---------|-------------|
| TV | Advertising budget spent on TV |
| Radio | Advertising budget spent on Radio |
| Newspaper | Advertising budget spent on Newspaper |
| Sales | Product sales (Target Variable) |

**Number of Records:** 200

---

## Technologies Used

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

## Project Structure

```text
DataScience-Task5-SalesPrediction/
│
├── Sales_Prediction.ipynb
├── README.md
├── requirements.txt
│
├── data/
│   └── Advertising.csv
│
├── images/
│   ├── pairplot.png
│   ├── correlation_heatmap.png
│   ├── scatter_tv.png
│   ├── scatter_radio.png
│   ├── scatter_newspaper.png
│   ├── residual_plot.png
│   └── feature_importance.png
│
└── models/
```

---

## Workflow

1. Import required libraries
2. Load the dataset
3. Perform Exploratory Data Analysis (EDA)
4. Check missing values and descriptive statistics
5. Generate pairplot and scatter plots
6. Create correlation heatmap
7. Split the dataset into training and testing sets
8. Train a Linear Regression model
9. Train a Random Forest Regressor
10. Evaluate both models
11. Generate residual plot
12. Analyze feature importance
13. Draw conclusions

---

## Exploratory Data Analysis

The following analyses were performed before model training:

- Dataset overview
- Missing value check
- Descriptive statistics
- Pairplot
- Sales vs TV scatter plot
- Sales vs Radio scatter plot
- Sales vs Newspaper scatter plot
- Correlation matrix heatmap

These visualizations helped understand the relationships between advertising expenditure and product sales.

---

## Machine Learning Models

### Linear Regression

Linear Regression was used as the baseline model to establish a relationship between advertising expenditure and sales.

### Random Forest Regressor

Random Forest Regressor was trained as an additional regression model to improve prediction accuracy by combining multiple decision trees.

---

## Model Evaluation

The models were evaluated using the following regression metrics:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score

### Results

| Model | MAE | RMSE | R² Score |
|------|------:|------:|------:|
| Linear Regression | 1.275 | 1.705 | 0.906 |
| Random Forest Regressor | 0.918 | 1.199 | 0.953 |

The Random Forest Regressor achieved the best overall performance with the lowest prediction errors and the highest R² Score.

---

## Feature Importance

Feature analysis indicates that:

- TV advertising has the highest impact on product sales.
- Radio advertising has a moderate impact.
- Newspaper advertising has the least impact on sales.

These findings are consistent with the correlation analysis performed during exploratory data analysis.

---

## Residual Analysis

A residual plot was generated for the best-performing model to evaluate prediction errors.

The residuals were randomly distributed around zero, indicating that the model fits the data well without significant systematic errors.

---

## Key Learning Outcomes

Through this project, the following concepts were learned:

- Exploratory Data Analysis (EDA)
- Data visualization
- Correlation analysis
- Regression techniques
- Linear Regression
- Random Forest Regression
- Model evaluation using MAE, RMSE, and R² Score
- Residual analysis
- Feature importance interpretation

---

## Future Improvements

Possible improvements for this project include:

- Hyperparameter tuning using GridSearchCV
- Cross-validation for more robust evaluation
- Feature engineering
- Testing additional regression algorithms such as XGBoost and Gradient Boosting
- Deploying the model using Flask or Streamlit
- Building an interactive web application for sales prediction

---

## Requirements

Install the required Python libraries using:

```bash
pip install -r requirements.txt
```

Example `requirements.txt`:

```text
pandas
numpy
matplotlib
seaborn
scikit-learn
```

---

## How to Run

1. Clone the repository.

```bash
git clone https://github.com/your-username/DataScience-Task5-SalesPrediction.git
```

2. Navigate to the project directory.

```bash
cd DataScience-Task5-SalesPrediction
```

3. Install the required dependencies.

```bash
pip install -r requirements.txt
```

4. Open `Sales_Prediction.ipynb` using Jupyter Notebook or Google Colab.

5. Run all cells sequentially.

---

## Conclusion

This project demonstrates how machine learning regression models can be used to predict product sales from advertising expenditure. After comparing multiple models, the Random Forest Regressor achieved the best performance, explaining approximately 95% of the variation in sales. The analysis also revealed that TV advertising is the most influential factor in driving product sales, followed by Radio, while Newspaper advertising contributes the least.

---

## Author

Subham Singh

B.Tech in Information Technology

Data Science Internship Project
