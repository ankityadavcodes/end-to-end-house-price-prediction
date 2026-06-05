# House Price Prediction using Machine Learning

## Project Overview

This project develops an end-to-end Machine Learning pipeline to predict residential house sale prices based on property characteristics such as plot size, house condition, construction year, remodeling year, basement area, and location-related features.

The project covers the complete machine learning workflow including data cleaning, exploratory data analysis (EDA), feature engineering, preprocessing, model training, evaluation, and model selection.

---

## Business Objective

Accurately predicting house prices helps real estate agencies, property investors, and homeowners make informed pricing decisions and understand the factors that influence property value.

---

## Dataset Information

* Total Records: 2,919
* Numerical Features: 8
* Categorical Features: 4
* Target Variable: SalePrice

### Key Features

* HouseType
* ZoneType
* PlotSize
* PlotShape
* BuildingType
* HouseCondition
* BuildYear
* RemodelYear
* BasementArea2
* TotalBasementArea

---

## Project Workflow

### 1. Data Cleaning

* Removed unnecessary ID column
* Handled missing values using Median and Mode Imputation
* Standardized column names

### 2. Exploratory Data Analysis (EDA)

* Correlation Analysis
* Feature Relationship Analysis
* Outlier Detection using IQR Method
* Heatmap Visualization

### 3. Feature Engineering

* One-Hot Encoding for categorical variables
* Feature Scaling using StandardScaler

### 4. Model Development

The following machine learning models were trained and evaluated:

* Linear Regression
* Decision Tree Regressor
* Random Forest Regressor
* XGBoost Regressor
* Support Vector Regressor (SVR)

---

## Model Performance

| Model                    | MAE    | R² Score |
| ------------------------ | ------ | -------- |
| Linear Regression        | 29,409 | 0.63     |
| Decision Tree Regressor  | 33,413 | 0.45     |
| Random Forest Regressor  | 21,573 | 0.78     |
| XGBoost Regressor        | 21,962 | 0.80     |
| Support Vector Regressor | 23,670 | 0.75     |

---

## Best Performing Model

### XGBoost Regressor

Performance:

* R² Score: 0.80
* MAE: 21,962
* Strong generalization ability
* Best overall predictive performance among all tested models

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* XGBoost

---

## Key Insights

* Total Basement Area showed the strongest relationship with house sale price.
* Newer houses generally had higher market values.
* Property size and basement size significantly influenced pricing.
* Ensemble learning methods outperformed traditional regression models.

---

## Future Improvements

* Hyperparameter Optimization
* Cross Validation
* Feature Selection Techniques
* Model Deployment using Streamlit or Flask
* Real-Time House Price Prediction API

---

## Repository Structure

```text
house-price-prediction-ml/
│
├── data/
│   └── house_price_dataset.xlsx
│
├── notebooks/
│   └── House_Price_Prediction.ipynb
│
├── images/
│
├── requirements.txt
├── README.md
└── LICENSE
```

---

## Author

Ankit Yadav

Aspiring Data Analyst | Python | SQL | Power BI | Machine Learning

