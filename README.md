# PharmacoSense: Sales Forecasting and Analytics Platform for Pharmacy Businesses

## Overview
**PharmacoSense** is an integrated sales forecasting and analytics platform specifically designed for pharmacy businesses.  
The system leverages **Seasonal ARIMA (SARIMA)** models to generate sales forecasts based on historical data and provides detailed interactive analytics to support data-driven business decision-making.  
Users can seamlessly upload sales datasets, perform automated data preprocessing, explore insightful trends, and obtain sales predictions through a user-friendly Streamlit web interface.

---

## Key Features
- **Automated Data Ingestion and Cleaning**: Upload sales datasets (CSV format) with automatic handling of missing values and formatting inconsistencies.
- **Advanced Time-Series Forecasting**: Utilizes SARIMA models optimized via Auto-ARIMA for accurate future sales predictions.
- **Interactive Visual Analytics**: Explore sales trends, top-performing products, category-wise breakdowns, and revenue insights with dynamic Altair and Matplotlib visualizations.
- **Predictive Modeling Interface**: Forecast sales for top-selling products across various future time intervals (weekly, biweekly, monthly).
- **Modular and Scalable Architecture**: Organized application structure enabling easy extension for additional models and features.

---

## Tech Stack
- **Programming Language**: Python
- **Frontend**: Streamlit
- **Data Processing**: Pandas, NumPy
- **Machine Learning / Forecasting**: Statsmodels (SARIMA), Pmdarima (Auto-ARIMA)
- **Visualization**: Altair, Matplotlib
- **Other Tools**: Scikit-Learn

---

## How to Run the Application
1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/pharmacosense.git
    ```

2. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Launch the application:
    ```bash
    streamlit run Home.py
    ```

- Upload your sales dataset following the required column format.
- Navigate through the sidebar to access **Analytics** or **Sales Predictions** modules.

---

## Dataset Requirements
Uploaded CSV files must include the following columns:
- **Product Name** (string)
- **Quantity** (integer)
- **Sell Price** (integer)
- **Date Sold** (datetime format: dd-mm-yyyy or mm/dd/yyyy)
- **Product Category** (string)

---

## Future Enhancements
- Extend forecasting capabilities to hybrid models combining ARIMA and LSTM techniques.
- Implement user authentication and session management for personalized analytics.
- Integrate real-time database storage with Firebase or PostgreSQL.
- Offer customizable prediction windows and multivariate time-series forecasting.
