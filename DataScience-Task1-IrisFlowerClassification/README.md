# Iris Flower Classification

## Objective
Train a machine learning classification model to identify the species of an
iris flower (Setosa, Versicolor, or Virginica) based on physical measurements
(sepal length/width, petal length/width).

## Dataset
Built-in Iris dataset from `sklearn.datasets` (150 samples, 3 balanced
classes of 50 each, no missing values).

## Tech Stack
Python, pandas, scikit-learn, matplotlib, seaborn, Jupyter Notebook (Google Colab)

## Approach
1. Loaded the dataset and performed exploratory data analysis (shape, dtypes,
   null check, descriptive statistics, class balance)
2. Visualized feature relationships using a pairplot and box plots per species
3. Identified petal length and petal width as the most discriminative features
4. Split data 80/20 into train/test sets (stratified to preserve class balance)
5. Trained two classifiers: Logistic Regression and K-Nearest Neighbors (KNN)
6. Evaluated both using accuracy, confusion matrix, and classification report

## Results
| Model | Accuracy |
|---|---|
| Logistic Regression | 96.7% |
| K-Nearest Neighbors (k=5) | 100% |

**Best model:** K-Nearest Neighbors — achieved perfect accuracy on the test
set, consistent with the tight, well-separated clusters observed during EDA.

## How to Run
Open `Iris_Classification.ipynb` in Google Colab or Jupyter Notebook and run
all cells sequentially. No external dataset download is required.
