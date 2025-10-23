# Walmart Weekly Sales Forecasting using Prophet

## Project Overview

This project implements a robust **time-series forecasting model** to accurately predict **weekly sales** across Walmart stores based on historical transaction data.

Accurate sales forecasting is a critical capability in the retail sector, directly impacting **inventory management**, **staffing optimization**, and strategic **resource allocation**. By leveraging the power of time-series analysis, this model provides reliable future sales estimates for business planning.

The core analysis is contained in the Jupyter Notebook: [`walmart_sales_prediction_using_prophet_11.ipynb`](walmart_sales_prediction_using_prophet_11.ipynb).

This plot illustrates the model's fit on historical sales (black dots) and the extended forecast (blue line) for future weeks.

![Walmart Sales Forecast Plot](walmart_sales_forecast_plot.png)

---

## Methodology

The model utilizes the **Prophet** library (developed by Meta, formerly Facebook), an intuitive and robust tool designed specifically for business forecasting problems that exhibit strong seasonality and holiday effects.

### Key Features Modeled:

1.  **Time-Series Preprocessing:** Data transformation to the standard Prophet format (`ds` for datestamp and `y` for sales).
2.  **Seasonality and Trend:** Prophet automatically models long-term **trend** and multiple levels of **seasonality** (e.g., weekly, yearly).
3.  **Holiday Impact:** Specific features were engineered to explicitly capture the significant, short-term lift in sales driven by **retail holidays** (e.g., Thanksgiving, Christmas, Super Bowl).

---

## Technical Stack and Requirements

The project is built using Python and relies on the following major libraries. These packages are listed in the `requirements.txt` file.

* **Python **
* **Prophet** (Primary Forecasting Engine)
* **Pandas & NumPy** (Data Manipulation)
* **Matplotlib & Seaborn** (Data Visualization)
* **Scikit-learn** (Performance Metrics)

### Installation

To run this notebook locally, first clone the repository and install the dependencies:

```bash
git clone <Your-Repository-URL>
cd <Your-Repository-Name>
pip install -r requirements.txt
