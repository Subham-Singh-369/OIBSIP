# Email Spam Detection using Machine Learning

## Project Overview

This project implements an **Email/SMS Spam Detection System** using **Natural Language Processing (NLP)** and **Machine Learning**. The objective is to classify messages as **Spam** or **Ham (Legitimate)** by preprocessing the text, extracting features using **TF-IDF**, and training machine learning classifiers.

This project was developed as part of a **Data Science Internship Task**.

---

## Objective

Build an NLP-based binary classification model that can automatically distinguish spam messages from legitimate messages.

---

## Features

* Load and explore the SMS Spam Collection dataset
* Analyze class distribution (Spam vs Ham)
* Perform text preprocessing:

  * Convert text to lowercase
  * Remove punctuation and special characters
  * Remove English stopwords
* Convert text into numerical features using **TF-IDF Vectorization**
* Split the dataset into training and testing sets
* Train two machine learning models:

  * Multinomial Naive Bayes
  * Logistic Regression
* Evaluate models using:

  * Accuracy
  * Precision
  * Recall
  * F1-Score
  * Confusion Matrix
* Generate WordCloud visualizations for Spam and Ham messages

---

## Technologies Used

* Python
* Google Colab
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* NLTK
* WordCloud

---

##  Dataset

This project uses the **SMS Spam Collection Dataset**, which contains **5,572 English SMS messages** labeled as **Spam** or **Ham**.

### Dataset Source

* Kaggle: https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset
* Original UCI Repository: https://archive.ics.uci.edu/dataset/228/sms+spam+collection

---

## Machine Learning Workflow

1. Load Dataset
2. Exploratory Data Analysis (EDA)
3. Text Preprocessing
4. TF-IDF Feature Extraction
5. Train-Test Split
6. Model Training
7. Model Evaluation
8. WordCloud Visualization
9. Conclusion

---

## Machine Learning Models

### 1. Multinomial Naive Bayes

A probabilistic classifier widely used for text classification problems such as spam detection.

### 2. Logistic Regression

A supervised learning algorithm commonly used for binary classification tasks.

---

## Model Performance

| Model                   |   Accuracy |   Precision |     Recall |   F1 Score |
| ----------------------- | ---------: | ----------: | ---------: | ---------: |
| Multinomial Naive Bayes | **97.20%** | **100.00%** | **80.00%** | **88.89%** |
| Logistic Regression     |     95.26% |      93.64% |     71.03% |     80.78% |

### Best Performing Model

**Multinomial Naive Bayes** achieved the best overall performance on this dataset.

---

## Visualizations

The project includes:

* Spam vs Ham distribution
* Message length analysis
* Confusion Matrix
* Spam WordCloud
* Ham WordCloud

---

## How to Run

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/DataScience-Task4-EmailSpamDetection.git
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Launch Jupyter Notebook or Google Colab

Open:

```
Email_Spam_Detection.ipynb
```

Run all cells in sequence.

---

## Requirements

```
pandas
numpy
matplotlib
seaborn
scikit-learn
nltk
wordcloud
```

---

## Future Improvements

* Hyperparameter tuning using GridSearchCV
* Support Vector Machine (SVM) implementation
* Email spam detection using real email datasets
* Deploy the model using Flask or Streamlit
* Build a web application for real-time spam detection

---

## Learning Outcomes

Through this project, I learned:

* Text preprocessing techniques in NLP
* Feature extraction using TF-IDF
* Binary text classification
* Model evaluation using classification metrics
* Data visualization
* Building an end-to-end machine learning pipeline

---

## Author

**Subham Singh**

B.Tech Information Technology

Data Science Intern
