# Walmart Weekly Sales Forecasting with XGBoost  

This project demonstrates how to build a **time series forecasting model** using lag features, rolling averages, and calendar features, trained with **XGBoost Regressor**. The dataset is split into **training** and **testing** sets, and the model predicts weekly sales for each store and department.

## 📂 Dataset Used  

This project uses the **[Walmart Sales Forecasting dataset](https://www.kaggle.com/datasets/aslanahmedov/walmart-sales-forecast)** from Kaggle.  

The dataset contains weekly sales data across multiple **stores** and **departments**, along with indicators for **holidays**.  

---
## 🗂️ Project Structure
```
├── Data/
│ └── train.csv # Input dataset
├── model.ipynb # Main script
└── README.md # Documentation
```
## 📊 Features Engineered
- Calendar Features:
  - Day of week
  - Year
  - Month
  - Quarter
  - Day of year
- Lag Features:
  - Sales from 1, 2, and 52 weeks before
- Rolling Averages:
  - 4, 12, 26, and 52-week rolling means
---
## 🚀 Workflow
### The notebook will:
- Load and visualize the dataset
- Perform feature engineering
- Split into training and testing sets
- Train an XGBoost model on historical sales
- Predict future sales on the test set
- Plot Actual vs Predicted sales
- Plot Residuals (prediction errors)
- Show Feature Importance
---
## 📈 Outputs
### The notebook generates the following visualizations:
- Training vs Testing sales split
- Actual vs Predicted sales curve
- Residual errors over time
- XGBoost Feature Importance chart

---
## ⚙️ Requirements  
Install the required libraries before running the script:  
```bash
pip install pandas numpy matplotlib xgboost
```
---
