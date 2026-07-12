# 📈 Sales Forecasting and Business Intelligence using Time Series & Machine Learning

![Python](https://img.shields.io/badge/Python-3.13-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-green)
![XGBoost](https://img.shields.io/badge/XGBoost-Machine%20Learning-orange)
![Prophet](https://img.shields.io/badge/Prophet-Time%20Series-red)
![SARIMA](https://img.shields.io/badge/SARIMA-Statistical%20Forecasting-purple)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

---

## 📌 Project Overview

Sales forecasting plays a crucial role in inventory management, demand planning, revenue estimation, and strategic business decision-making.

This project develops and compares multiple forecasting approaches to accurately predict future sales using historical sales data. Both traditional statistical time-series models and modern machine learning techniques are implemented, evaluated, and compared.

The project demonstrates a complete end-to-end data science workflow including:

- Data preprocessing
- Exploratory Data Analysis (EDA)
- Time Series Analysis
- Statistical Forecasting
- Machine Learning Forecasting
- Hyperparameter Tuning
- Model Evaluation
- Business Insights

---

# 🎯 Objectives

The primary objectives of this project are:

- Forecast future sales using historical sales data.
- Compare statistical and machine learning forecasting techniques.
- Identify the best-performing forecasting model.
- Generate actionable business insights.
- Support inventory planning and demand forecasting.

---

# 📂 Dataset

**Source**

Kaggle – Sales Forecasting Dataset

https://www.kaggle.com/datasets/rohitsahoo/sales-forecasting

The dataset contains customer orders including:

- Order Date
- Ship Date
- Customer Information
- Product Category
- Region
- Sales
- Shipping Details

---

# 🛠️ Technologies Used

| Category | Tools |
|-----------|---------------------------|
| Programming | Python |
| Data Processing | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Machine Learning | Scikit-learn |
| Statistical Models | Statsmodels |
| Time Series Forecasting | Prophet |
| Machine Learning Forecasting | XGBoost |
| Notebook | Jupyter Notebook |

---

# 📊 Project Workflow

```
Raw Dataset
      │
      ▼
Data Cleaning
      │
      ▼
Feature Engineering
      │
      ▼
Exploratory Data Analysis
      │
      ▼
Time Series Analysis
      │
      ▼
SARIMA Forecasting
      │
      ▼
Prophet Forecasting
      │
      ▼
XGBoost Forecasting
      │
      ▼
Hyperparameter Tuning
      │
      ▼
Model Evaluation
      │
      ▼
Business Insights
```

---

# 📈 Exploratory Data Analysis

The following analyses were performed:

- Monthly Sales Trend
- Regional Sales Analysis
- Seasonal Analysis
- Category-wise Sales
- Shipping Time Analysis
- Sales Distribution
- Correlation Analysis

Key observations:

- Sales exhibit strong yearly seasonality.
- Certain months consistently generate higher revenue.
- Regional sales performance differs significantly.
- Sales demonstrate an upward long-term trend.

---

# 📉 Time Series Forecasting Models

## 1️⃣ SARIMA

Seasonal Auto-Regressive Integrated Moving Average (SARIMA) was used as the baseline statistical forecasting model.

### Performance

| Metric | Value |
|---------|-------:|
| MAE | 14504.91 |
| RMSE | 17429.94 |

---

## 2️⃣ Prophet

Meta Prophet was implemented to capture trend and yearly seasonality.

Hyperparameter tuning was performed using Grid Search.

### Performance

| Metric | Value |
|---------|-------:|
| MAE | 11352.52 |
| RMSE | 12823.24 |
| MAPE | 17.74% |
| R² | 0.7150 |

---

## 3️⃣ XGBoost (Final Model)

A feature-engineered XGBoost regression model was developed using:

- Lag Features
- Rolling Mean
- Rolling Standard Deviation
- Calendar Features

Hyperparameter tuning was performed using GridSearchCV.

### Final Performance

| Metric | Value |
|---------|-------:|
| MAE | **9084.05** |
| RMSE | **11695.47** |
| MAPE | **12.90%** |
| R² | **0.7846** |

---

# 🏆 Model Comparison

| Model | MAE | RMSE | MAPE | R² |
|-------|------:|------:|------:|------:|
| SARIMA | 14504.91 | 17429.94 | — | — |
| Prophet | 11352.52 | 12823.24 | 17.74% | 0.7150 |
| **XGBoost** | **9084.05** | **11695.47** | **12.90%** | **0.7846** |

---

# 📌 Key Findings

- XGBoost achieved the best forecasting performance.
- Lag features significantly improved prediction accuracy.
- Hyperparameter tuning reduced forecasting errors.
- Prophet effectively modeled seasonality but was outperformed by XGBoost.
- SARIMA served as a reliable statistical baseline but produced higher forecasting errors.

---

# 💼 Business Impact

The developed forecasting system can help organizations:

- Improve inventory planning
- Reduce stock shortages
- Minimize excess inventory
- Estimate future revenue
- Support strategic decision-making
- Improve demand forecasting

---

# 🚀 Future Improvements

Future enhancements may include:

- Integration with real-time sales databases
- Holiday and promotional effect modeling
- LSTM and Transformer-based forecasting
- Deployment using Streamlit
- Cloud deployment using AWS or Azure
- Automated forecasting dashboards

---

# 📁 Repository Structure

```
Sales-Forecasting-Analysis/

│── Sales_Forecasting_Analysis.ipynb
│── train.csv
│── requirements.txt
│── README.md
```

---

# ▶️ How to Run

Clone the repository

```
git clone https://github.com/YOUR_USERNAME/Sales-Forecasting-Analysis.git
```

Install dependencies

```
pip install -r requirements.txt
```

Launch Jupyter Notebook

```
jupyter notebook
```

Open

```
Sales_Forecasting_Analysis.ipynb
```

Run all cells sequentially.

---

# 👨‍💻 Author

## N. A. Harshal

**B.Tech (Hons.) Computer Science Engineering**

Major: Data Science & Machine Learning

RV University

Bengaluru, Karnataka, India

---

# ⭐ Acknowledgements

- Kaggle for providing the dataset.
- Meta Prophet Team.
- XGBoost Development Team.
- Statsmodels Community.
- Open-source Python community.

---

## ⭐ If you found this project useful, consider giving the repository a star.
