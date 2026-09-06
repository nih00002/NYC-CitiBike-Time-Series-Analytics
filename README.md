# Dataset Information

The raw datasets used for this project are not stored in this repository because the complete 2020 data collection contains multiple large files.

The analysis was developed using open data associated with NYC bike-sharing operations, weather conditions, and operational inspections.

## Data Used

### 1. NYC Citi Bike Trip Data

The primary dataset contains NYC Citi Bike trip records for 2020.

The trip data was used for:

- Daily and monthly bike-usage analysis
- Trip-duration analysis
- User and ridership analysis
- Station-level demand analysis
- Seasonal usage patterns
- Time-series forecasting
- Overall bike-usage prediction

### 2. Weather Data

Weather information, particularly relative humidity, was incorporated into the analysis to investigate relationships between environmental conditions and bike usage.

Relative humidity was also explored as an exogenous variable in time-series modeling.

### 3. Bike-Sharing Inspection Data

Operational inspection data was used to investigate factors affecting station and bike-sharing operations and to support the business-analytics component of the study.

## Data Period

The primary analytical period is:

**January–December 2020**

## Why the Raw Data Is Not Included

The complete dataset consists of multiple large source files. To keep this repository lightweight, the raw data is excluded from version control.

The notebook documents the preprocessing, aggregation, analysis, and forecasting workflow used in the original 2021 thesis project.

## Local Data

When reproducing the analysis locally, downloaded datasets should be stored under the `data/` directory.

The repository `.gitignore` excludes raw data files from version control.
