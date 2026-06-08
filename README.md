# Steam Hidden Gems Classification

## Project Overview

This project aims to identify **Hidden Gem** games on Steam using Machine Learning classification models.

A custom metric called **Steam Rating** was created to measure game quality while considering ownership count. Games with exceptionally high user ratings but relatively low ownership numbers are classified as potential hidden gems.

The project explores Steam game data, performs exploratory data analysis (EDA), builds multiple machine learning models, and compares their performance to predict whether a game can be considered a hidden gem.

---

## Repository Structure

```
├── README.md
├── Hidden Gem Prediction.ipynb
└── Steam_Games_dataset.csv
```

### File Description

| File                       | Description                                                                 |
| -------------------------- | --------------------------------------------------------------------------- |
| README.md                  | General project overview and documentation                                  |
| Hidden Gem Prediction.ipynb   | Main notebook containing EDA, preprocessing, model training, and evaluation |
| Steam_Games_dataset.csv    | Dataset used for analysis and model development                             |


---

## Problem Background

Steam hosts thousands of games across various genres and categories. While many popular titles receive significant attention and large player bases, numerous high-quality games remain relatively unknown despite receiving overwhelmingly positive reviews.

The challenge is identifying these **Hidden Gems** systematically rather than relying solely on subjective opinions.

To address this issue, a custom metric called **Steam Rating** was developed. This metric combines review quality and ownership information to identify games that receive excellent player feedback while maintaining relatively low ownership counts.

---

## Project Objective

Build a machine learning classification model capable of predicting whether a Steam game can be categorized as a Hidden Gem.

### Target Labels

| Label | Meaning                 |
| ----- | ----------------------- |
| 1     | Hidden Gem / Success    |
| 0     | Not Hidden Gem / Failed |

---

## Dataset

### Source

Steam Games Dataset (SteamSpy API) by Aqeel Kabir

The dataset contains information such as:

* Developer
* Publisher
* User Score
* Ownership Estimates
* Playtime Statistics
* Price Information
* Review Metrics
* Additional Steam Metadata

---

## Methodology

The project follows a complete Machine Learning workflow:

### 1. Data Preparation

* Data Cleaning
* Handling Missing Values
* Feature Selection
* Feature Engineering

### 2. Exploratory Data Analysis (EDA)

* Distribution Analysis
* Correlation Analysis
* Hidden Gem Exploration
* Feature Insights

### 3. Model Development

Five classification algorithms were evaluated:

* K-Nearest Neighbors (KNN)
* Support Vector Machine (SVM)
* Decision Tree
* Random Forest
* Gradient Boosting

### 4. Model Evaluation

Evaluation metrics include:

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix

Cross-validation was performed using:

* K-Fold Cross Validation

### 5. Hyperparameter Tuning

Optimization performed using:

* GridSearchCV

---

## Technology Stack

### Programming Language

* Python 3

### Data Processing

* pandas
* numpy

### Data Visualization

* matplotlib
* seaborn

### Machine Learning

* train_test_split
* cross_val_score
* Pipeline
* SimpleImputer
* StandardScaler
* OneHotEncoder
* LabelEncoder
* ColumnTransformer
* GridSearchCV

### Models

* KNeighborsClassifier
* SVC
* DecisionTreeClassifier
* RandomForestClassifier
* GradientBoostingClassifier

### Evaluation

* classification_report
* confusion_matrix
* ConfusionMatrixDisplay

### Model Persistence

* pickle

---

## Results

Five machine learning models were trained and evaluated using cross-validation and hyperparameter tuning.

The final selected model achieved the highest overall performance and was saved for future inference. The trained model can predict whether a new Steam game possesses characteristics commonly associated with Hidden Gem titles.

---

## Future Improvements

Potential improvements for future work include:

* Incorporating genre-based features
* Using advanced ensemble methods
* Adding sentiment analysis from Steam reviews
* Improving feature engineering techniques
* Expanding dataset coverage

---

## References

### Dataset

Steam Games Dataset (SteamSpy API)

Author: Aqeel Kabir

Source: Kaggle

---



