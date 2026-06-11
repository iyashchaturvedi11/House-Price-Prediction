# House-Price-Prediction


**Advanced Machine Learning Project for Predicting Residential House Prices**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-%2318B2A0.svg?style=for-the-badge&logo=xgboost&logoColor=white)

---

## 📋 Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Dataset](#dataset)
- [Project Workflow](#project-workflow)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Model Performance](#model-performance)
- [Results](#results)
- [Project Structure](#project-structure)
- [Future Improvements](#future-improvements)
- [Author](#author)

---

##  Overview

This project implements a comprehensive **House Price Prediction** system using the famous Ames Housing Dataset. The goal is to predict the final sale price of residential homes in Ames, Iowa with high accuracy through extensive data analysis, feature engineering, and ensemble machine learning techniques.

The final model (**Gradient Boosting Regressor**) achieves strong predictive performance on unseen test data and was used to generate submissions for the Kaggle House Prices competition.

---

##  Features

- **Comprehensive EDA**: Missing value analysis, distribution plots, correlation analysis
- **Robust Data Preprocessing**: Handling of categorical and numerical missing values with domain knowledge
- **Feature Engineering**: 
  - Conversion of numerical features to categorical where appropriate
  - Ordinal encoding for quality-related features
  - One-hot encoding for nominal variables
- **Advanced Modeling**: Multiple regression algorithms tested with cross-validation
- **Scalability**: Data standardization using `StandardScaler`
- **Production Ready**: Model serialization with Pickle

---

##  Dataset

- **Source**: [Kaggle - House Prices - Advanced Regression Techniques](https://www.kaggle.com/c/house-prices-advanced-regression-techniques)
- **Train**: 1460 samples, 81 features
- **Test**: 1459 samples, 80 features
- **Target**: `SalePrice` (continuous variable)

**Key Features Include**:
- Physical attributes (LotArea, GrLivArea, etc.)
- Quality ratings (OverallQual, ExterQual, etc.)
- Location and neighborhood information
- Basement, Garage, and Pool characteristics

---

##  Project Workflow

1. **Data Loading & Integration**
2. **Exploratory Data Analysis (EDA)**
3. **Missing Value Treatment** (Domain-knowledge based imputation)
4. **Feature Transformation & Encoding**
5. **Data Splitting & Scaling**
6. **Model Selection via Cross-Validation**
7. **Final Model Training**
8. **Prediction & Submission Generation**

---

## 🛠 Technologies Used

- **Language**: Python 3
- **Data Manipulation**: pandas, numpy
- **Visualization**: matplotlib, seaborn
- **Machine Learning**: scikit-learn, XGBoost
- **Others**: calendar, pickle

**Core Models Evaluated**:
- Linear Regression
- SVR
- Random Forest
- Gradient Boosting Regressor (Best)
- XGBoost
- Others

---

##  Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/house-price-prediction.git
cd house-price-prediction

# Create virtual environment (optional)
python -m venv venv
source venv/bin/activate    # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

numpy
pandas
matplotlib
seaborn
scikit-learn
xgboost

