# Teerapat-
# Analysis and Comparison of Time Series Models for Sales Forecasting

## Abstract  
This study aims to analyze, develop, and compare the forecasting performance of the **Prophet** and **SARIMAX** models using the historical sales data of **ABC Company Limited (2021–2024)**. The monthly aggregated sales data were split into **training data (2021–2023)** and **testing data (2024)** to evaluate forecasting accuracy.  

The models’ performances were measured using the following error metrics:  
- **Mean Absolute Error (MAE)**  
- **Root Mean Squared Error (RMSE)**  
- **Mean Absolute Percentage Error (MAPE)**  

The experimental results indicate that the **Prophet model outperforms the SARIMAX model**, demonstrating superior forecasting accuracy. Therefore, the Prophet model is more suitable for the company’s sales forecasting, enabling more precise and effective prediction of future sales trends.

---

## Project Objective
- To build time series models for predicting monthly sales.  
- To compare the performance between **Prophet** and **SARIMAX**.  
- To identify the most accurate forecasting model for practical business use.  

---

## Tools & Technologies
- **Python**  
- **Pandas, Numpy**  
- **Matplotlib**  
- **Prophet**  
- **SARIMAX (Statsmodels)**  
- **Scikit-learn**  
- **Microsoft Excel** (Data preparation)

---

## Dataset Description
- Sales data of **ABC Company Limited** from **January 2021 – December 2024**  
- Monthly aggregated time series format  
- Data split:  
  - **Training:** 2021–2023  
  - **Testing:** 2024  

---

## Methodology

### 1. **Data Preprocessing**
- Handling missing values  
- Converting date columns to datetime format  
- Resampling to monthly frequency  
- Train-test split  

### 2. **Model Development**
#### Prophet Model  
- Trend + yearly seasonality  
- Multiplicative model configuration  

#### SARIMAX Model  
- Grid search for optimal (p, d, q)(P, D, Q)m  
- Seasonal order based on monthly pattern  

### 3. **Model Evaluation Metrics**
- **MAE**  
- **RMSE**  
- **MAPE**  
- Visual comparison between actual vs predicted values  

---

## Results & Findings
- The **Prophet model** achieved consistently lower error values across MAE, RMSE, and MAPE.  
- The **SARIMAX model** showed reasonable performance but tended to underfit seasonal patterns.  
- Visualization indicates Prophet provides smoother and more accurate future trend estimation.  

> **Conclusion:** Prophet is the recommended model for forecasting the company’s monthly sales data due to its superior accuracy and ability to capture trend-seasonality patterns effectively.

---

## Visualizations
Key charts included in the notebook:  
- Sales trend (2021–2024)  
- Prophet forecast vs actual  
- SARIMAX forecast vs actual  
- Comparison of error metrics  


---

## Project Structure
├── data/
│   ├── sales_2021_2024.xlsx        # Raw sales dataset
│
├── notebooks/
│   ├── prophet_model.ipynb         # Prophet model development
│   ├── sarimax_model.ipynb         # SARIMAX model development
│   ├── comparison.ipynb            # Model comparison & visualization
│
├── src/
│   ├── preprocess.py               # Data cleaning & preprocessing
│   ├── train_prophet.py            # Prophet training script
│   ├── train_sarimax.py            # SARIMAX training script
│   ├── evaluation.py               # MAE/RMSE/MAPE calculation
│
├── README.md
└── requirements.txt
