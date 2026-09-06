# NYC Citi Bike Time-Series Analytics

Time-series forecasting and business analytics for NYC Citi Bike demand using ARIMA, SARIMAX, Prophet, weather data, and Power BI.

## Overview

This repository presents the practical analytical work developed for my 2021 M.Sc. thesis:

**“Improvement of Bike Sharing Disposition by Business Analytics and Open Data Usage”**

The thesis was completed at **TH Köln University of Applied Sciences** in September 2021.

The project investigates how business analytics, open data, and time-series forecasting can support bike-sharing operations and planning. The analysis focuses on NYC Citi Bike usage and combines trip records with weather and operational inspection data.

## Project Objectives

The main objectives of the project were to:

- Perform descriptive and exploratory analysis of bike-sharing data
- Investigate daily, monthly, seasonal, and station-level usage patterns
- Examine the relationship between weather conditions and bike usage
- Analyze trip duration and station demand
- Evaluate stationarity and temporal patterns in bike-sharing data
- Develop station-level time-series forecasting models
- Compare different forecasting approaches
- Predict future daily and weekday bike usage
- Prepare analytical outputs for business-intelligence visualization

## Data

The analysis primarily uses data covering:

**January–December 2020**

Three main categories of data were considered:

### NYC Citi Bike Trip Data

Trip records were used to investigate:

- Daily and monthly bike usage
- Trip duration
- Station-level activity
- Seasonal patterns
- Ridership characteristics
- Time-series behavior

### Weather Data

Weather information, particularly **relative humidity**, was integrated with bike-sharing data to investigate the relationship between environmental conditions and bike usage.

Relative humidity was also explored as an external variable in the forecasting analysis.

### Bike-Sharing Inspection Data

Operational inspection data was analyzed to investigate factors associated with bike-sharing operations and support the business-analytics component of the project.

The complete raw datasets are not stored in this repository because they consist of multiple large files.

See [`data/README.md`](data/README.md) for additional dataset information.

## Analytical Workflow

The practical analysis includes:

1. Data collection and preprocessing
2. Monthly and seasonal data aggregation
3. Exploratory data analysis
4. Station-level usage analysis
5. Trip-duration analysis
6. Weather-data integration
7. Rolling mean and time-series visualization
8. Stationarity testing
9. Differencing
10. ACF and PACF analysis
11. Time-series model development
12. Forecast evaluation and model comparison
13. Operational inspection analysis
14. Preparation of analytical outputs for Power BI

## Time-Series Analysis

### Stationarity Testing

The **Augmented Dickey-Fuller (ADF) test** was used as part of the stationarity analysis.

Rolling statistics and differencing were also explored before developing forecasting models.

### ACF and PACF

Autocorrelation Function (**ACF**) and Partial Autocorrelation Function (**PACF**) analysis were used to examine temporal dependencies and support time-series model development.

## Forecasting Models

Several forecasting approaches were explored and compared.

### ARIMA

**Autoregressive Integrated Moving Average (ARIMA)** models were used for time-series forecasting after examining stationarity and autocorrelation characteristics.

### Auto-ARIMA

**Auto-ARIMA** was explored to support model-order selection and forecasting experiments.

### SARIMAX

**SARIMAX** was investigated with relative humidity as an exogenous variable, allowing weather information to be incorporated into the forecasting process.

### Prophet

**Prophet** was also evaluated as an alternative forecasting approach for bike-usage time series.

### Exponential Smoothing and Power BI

The project additionally explored forecasting and trend analysis within the business-intelligence workflow, including exponential smoothing and visualization in **Power BI**.

## Repository Structure

```text
NYC-CitiBike-Time-Series-Analytics/
├── README.md
├── requirements.txt
├── .gitignore
├── data/
│   └── README.md
├── notebooks/
│   ├── README.md
│   └── CitiBike_Time_Series_Analytics.ipynb
├── results/
├── dashboard/
└── thesis/
```

## Main Notebook

The practical implementation is available in:

[`notebooks/CitiBike_Time_Series_Analytics.ipynb`](notebooks/CitiBike_Time_Series_Analytics.ipynb)

The notebook contains the cleaned archival version of the analysis performed for the original 2021 thesis project.

## Technologies

The project uses tools and libraries including:

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Statsmodels
- pmdarima
- Prophet
- Plotly
- Jupyter Notebook
- Power BI

## Installation

To create a local environment for the Python dependencies:

```bash
pip install -r requirements.txt
```

> **Note:** This is an archival project originally implemented in 2021. Some APIs used in the notebook have since changed or been deprecated, so the notebook may require minor compatibility updates to run completely in a modern Python environment.

## Reproducibility

The original analysis was developed using 2020 datasets that are not included in this repository because of their size.

Some packages and APIs used in the original implementation have also changed since 2021. Examples include:

- The former `fbprophet` package, now distributed as `prophet`
- Legacy Statsmodels ARIMA APIs
- `DataFrame.append`, which has been removed from recent versions of Pandas

The repository therefore preserves the original analytical methodology and results while presenting the work in a cleaner portfolio-oriented structure.

## Thesis Information

**Title:** Improvement of Bike Sharing Disposition by Business Analytics and Open Data Usage  
**Author:** Nafiu Ikeoluwa Hammed  
**Degree:** Master of Science (M.Sc.) Informatik-Computer Science  
**Institution:** TH Köln University of Applied Sciences  
**Institute:** Institute of Informatics  
**Year:** 2021

## Portfolio Note

The original M.Sc. thesis and practical analysis were completed in **2021**.

This repository was subsequently curated for portfolio presentation. The organization and documentation have been improved while preserving the original analytical work and historical context.
