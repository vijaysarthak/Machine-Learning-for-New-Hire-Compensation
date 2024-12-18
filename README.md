# TechWorks Salary Prediction Project

## Overview

This project focuses on developing a predictive model for determining employee salaries for TechWorks Consulting, a company specializing in IT talent recruitment. The goal is to create a reliable regression model using machine learning techniques to estimate continuous salary values based on various employee features.

---

## Problem Statement

TechWorks Consulting seeks to enhance its ability to predict employee salaries by leveraging regression models. Accurate salary predictions help the company streamline its operations, improve client satisfaction, and make informed business decisions.

### Key Objectives
- Use regression techniques to predict salaries.
- Handle missing values, outliers, and categorical data during preprocessing.
- Evaluate and compare the performance of multiple machine learning models.
- Provide actionable insights from the data.

---

## Dataset

The project utilizes three datasets:
1. **Employee Dataset**: Contains employee-specific data such as previous salaries, college, and city.
2. **College Dataset**: Contains information about colleges categorized into tiers.
3. **City Dataset**: Distinguishes between metro and non-metro cities.

### Features
- **Categorical Variables**: Colleges and cities.
- **Numerical Variables**: Salary, previous CTC, etc.

---

## Workflow

### 1. **Data Understanding**
- Examined data distribution, trends, and structure to guide preprocessing.

### 2. **Data Preprocessing**
- **Handling Missing Values**: Used imputation techniques.
- **Handling Outliers**: Analyzed using box plots; no significant outliers were identified.
- **Categorical Encoding**: Used one-hot encoding and numerical mapping for categorical variables.
- **Feature Scaling**: Applied standardization to numeric features.
- **Feature Selection**: Selected relevant features to improve model efficiency.

### 3. **Exploratory Data Analysis (EDA)**
- Conducted visual and statistical analysis to understand feature relationships.

### 4. **Model Selection and Training**
- Models implemented:
  - Linear Regression
  - Ridge Regression
  - Lasso Regression
  - Decision Tree Regressor
  - Random Forest Regressor
  - K-Nearest Neighbors
- Evaluated using metrics:
  - R-squared
  - Mean Absolute Error (MAE)
  - Mean Squared Error (MSE)

### 5. **Hyperparameter Tuning**
- Optimized model parameters using Grid Search for enhanced performance.

---

## Key Findings
- Linear Regression served as the baseline model.
- Ridge and Lasso regressions improved generalization by handling multicollinearity.
- Decision Trees and Random Forests excelled with flexible and robust performance.
- Feature scaling significantly impacted model accuracy in specific cases.

---

## How to Run the Project

### Prerequisites
- Python 3.7 or later
- Required libraries: `pandas`, `numpy`, `seaborn`, `matplotlib`, `scikit-learn`

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/techworks-salary-prediction.git
   ```
2. Navigate to the project directory:
   ```bash
   cd techworks-salary-prediction
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Run the script:
   ```bash
   python main.py
   ```

---

## Results and Insights
- Ridge Regression with feature scaling showed optimal performance with an R-squared of **0.89**.
- Random Forest provided robust predictions with minimal error.
- Salary prediction accuracy increased after handling categorical variables and scaling.

---

## Future Scope
- Incorporate additional features such as experience, certifications, or domain expertise.
- Use advanced models like Gradient Boosting or Neural Networks for further improvements.
- Deploy the model using Flask or FastAPI for real-time salary predictions.

---