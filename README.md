# Titanic Survival Prediction - Logistic Regression

[![Python](https://img.shields.io/badge/Python-3.x-blue.svg)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

A machine learning project predicting passenger survival on the Titanic using Logistic Regression. This notebook demonstrates data preprocessing, exploratory analysis, feature engineering, and model evaluation on the famous Titanic dataset.

## 📋 Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Project Structure](#project-structure)
- [Features](#features)
- [Methodology](#methodology)
- [Model Performance](#model-performance)
- [Key Insights](#key-insights)
- [Requirements](#requirements)
- [Installation & Usage](#installation--usage)
- [Results](#results)
- [Files](#files)
- [Future Enhancements](#future-enhancements)
- [Author](#author)

## 📊 Overview

The Titanic disaster, one of the most tragic maritime events in history, claimed the lives of over 1,500 passengers and crew members. This project builds a predictive model to determine which passengers were more likely to survive based on historical data.

**Goal:** Create an interpretable binary classification model using Logistic Regression to predict passenger survival outcomes.

**Model:** Logistic Regression was chosen for its simplicity, interpretability, and effectiveness in binary classification problems.

## 🗂️ Dataset

The project uses the famous Titanic dataset containing information about 891 passengers.

**Source:** [Kaggle - Titanic Dataset](https://www.kaggle.com/c/titanic/data)

**Dataset Files:**
- `titanic_train.csv` - Training dataset (891 passengers)
- `titanic_test.csv` - Test dataset for validation
- `titanic_train_demo.csv` - Demo dataset for exploration

**Key Features:**
- **PassengerId:** Unique identifier for each passenger
- **Pclass:** Ticket class (1st, 2nd, or 3rd)
- **Name:** Passenger name
- **Sex:** Gender (male/female)
- **Age:** Age in years
- **SibSp:** Number of siblings/spouses aboard
- **Parch:** Number of parents/children aboard
- **Ticket:** Ticket number
- **Fare:** Ticket price
- **Cabin:** Cabin number
- **Embarked:** Port of embarkation
- **Survived:** Survival status (target variable: 0 = No, 1 = Yes)

## 📁 Project Structure

```
survival-prediction-titanic-logistic-regression/
├── README.md
├── Titanic_Dataset_Logistic_Regression.ipynb    # Main notebook
├── titanic_train.csv                            # Training data
├── titanic_test.csv                             # Test data
└── titanic_train_demo.csv                       # Demo data
```

## 🎯 Features

- **Exploratory Data Analysis (EDA):** Comprehensive data visualization and statistical analysis
- **Data Preprocessing:** Handling missing values, encoding categorical variables
- **Feature Engineering:** Creating new features, feature scaling and normalization
- **Model Training:** Logistic Regression implementation with parameter tuning
- **Model Evaluation:** Accuracy, precision, recall, F1-score, ROC-AUC
- **Interpretability:** Feature importance and decision boundary visualization

## 🔬 Methodology

### 1. **Data Exploration**
   - Dataset shape, data types, and missing values analysis
   - Statistical summary and distribution plots
   - Correlation analysis between features

### 2. **Data Preprocessing**
   - Handling missing values in Age, Cabin, and Embarked columns
   - Encoding categorical variables (Sex, Embarked)
   - Removing irrelevant features (PassengerId, Name, Ticket, Cabin)

### 3. **Feature Engineering**
   - Creating new features: Family size, Titles from names
   - Binning age groups
   - Scaling numerical features using StandardScaler

### 4. **Model Development**
   - Training Logistic Regression model
   - Hyperparameter tuning
   - Cross-validation for robust performance estimation

### 5. **Evaluation**
   - Confusion matrix analysis
   - Performance metrics calculation
   - Classification report generation
   - ROC curve and AUC score

## 📈 Model Performance

| Metric | Score |
|--------|-------|
| Accuracy | High |
| Precision | Strong |
| Recall | Robust |
| F1-Score | Balanced |
| ROC-AUC | Excellent |

*Note: Exact scores are available in the notebook output*

## 💡 Key Insights

1. **Gender Impact:** Female passengers had significantly higher survival rates (~74%) compared to males (~19%)
2. **Class Matters:** 1st class passengers had higher survival rates than 3rd class passengers
3. **Age Factor:** Younger passengers, especially children, had better survival chances
4. **Family Size:** Traveling with 1-2 family members increased survival odds; larger groups had lower survival rates
5. **Fare Correlation:** Higher ticket fares correlated with higher survival rates

## 📦 Requirements

- Python 3.x
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn
- jupyter

## 💻 Installation & Usage

### Prerequisites
Ensure you have Python and Jupyter installed on your system.

### Steps

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/survival-prediction-titanic-logistic-regression.git
   cd survival-prediction-titanic-logistic-regression
   ```

2. **Install dependencies:**
   ```bash
   pip install pandas numpy scikit-learn matplotlib seaborn jupyter
   ```

3. **Launch Jupyter Notebook:**
   ```bash
   jupyter notebook
   ```

4. **Open the notebook:**
   Open `Titanic_Dataset_Logistic_Regression.ipynb` in your browser

5. **Run the cells:**
   Execute cells sequentially to see data exploration, model training, and evaluation

## 🎓 Results

The logistic regression model successfully:
- ✅ Predicts survival with high accuracy
- ✅ Identifies key survival factors
- ✅ Provides interpretable predictions
- ✅ Demonstrates the importance of gender and class in historical survival

## 📄 Files

| File | Description |
|------|-------------|
| `Titanic_Dataset_Logistic_Regression.ipynb` | Main Jupyter notebook with complete analysis |
| `titanic_train.csv` | Training dataset (891 passengers) |
| `titanic_test.csv` | Test dataset |
| `titanic_train_demo.csv` | Demo/exploration dataset |
| `README.md` | Project documentation |

## 🔮 Future Enhancements

- [ ] Compare with other algorithms (Random Forest, SVM, Neural Networks)
- [ ] Implement advanced feature engineering techniques
- [ ] Create a web app for predictions
- [ ] Add cross-validation results
- [ ] Hyperparameter optimization with GridSearchCV
- [ ] Feature selection analysis
- [ ] Model deployment with Flask/FastAPI

## 🙋 Author

Camille Buan

## 📝 License

This project is open source and available under the MIT License.

## 🔗 References

- [Kaggle Titanic Competition](https://www.kaggle.com/c/titanic)
- [Scikit-learn Logistic Regression Documentation](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html)
- [Pandas Documentation](https://pandas.pydata.org/)
- [Titanic Dataset Information](https://www.kaggle.com/c/titanic/data)

---

**Happy Learning! 🚀**
