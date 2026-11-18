# Morocco Electricity Consumption Analysis

## Project Overview

This project explores electricity consumption patterns across three geographical zones in Morocco using Python and data visualisation.

The analysis examines differences in recorded consumption, hourly and monthly patterns, and statistical relationships between consumption and selected environmental variables.

The objective is to generate evidence-based insights that can support further electricity demand monitoring, operational investigation and energy planning.

## Business Questions

1. How do recorded electricity consumption patterns differ across the three zones?
2. At what times of day are average consumption readings highest and lowest?
3. How do consumption patterns vary by day of the week and month?
4. What statistical relationships exist between environmental variables and consumption?
5. Which observed patterns should be investigated further by energy-management stakeholders?

## Dataset Overview

- Records: 52,416
- Original variables: 9
- Coverage: 1 January to 30 December 2017
- Recording frequency: 10 minutes
- Geographical zones: 3

### Original Variables

- Datetime
- Temperature
- Humidity
- WindSpeed
- GeneralDiffuseFlows
- DiffuseFlows
- PowerConsumption_Zone1
- PowerConsumption_Zone2
- PowerConsumption_Zone3

The original dataset should be placed in `data/raw/` before running the notebook.

**Data availability:** The raw dataset is not included in this repository by default. Only publish it if its licence and distribution terms permit redistribution.

## Tools and Technologies

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Plotly
- SciPy
- Statsmodels

## Project Workflow

1. Dataset loading and inspection.
2. Data-quality assessment.
3. Data cleaning and preparation.
4. Temporal feature engineering.
5. Descriptive consumption analysis.
6. Hourly, daily, weekly and monthly comparisons.
7. Environmental correlation analysis.
8. Business findings and recommendations.
9. Static and interactive visualisation exports.
10. Documentation and reporting.

## Key Findings

- Zone 1 recorded the highest mean consumption reading, approximately 32,344.97.
- Zone 2 recorded a mean of approximately 21,042.51.
- Zone 3 recorded a mean of approximately 17,835.41.
- All three zones recorded their highest average hourly readings at 20:00.
- Zone 1 and Zone 2 recorded their highest monthly averages in August, while Zone 3 peaked in July.
- Temperature showed positive Pearson correlations with consumption in all three zones.
- Humidity showed negative Pearson correlations with consumption in all three zones.

These are descriptive findings from the available 2017 dataset. They do not establish causal relationships.

## Visualisations

### Static Visualisations

The `visualizations/static/` folder contains:

- Average consumption by zone.
- Hourly consumption by zone.
- Monthly consumption by zone.
- Monthly consumption heatmap.
- Environmental and consumption correlation heatmap.

### Interactive Visualisations

The `visualizations/interactive/` folder contains:

- Interactive hourly consumption chart.
- Interactive monthly consumption chart.

Open the HTML files in a modern web browser to explore the charts.

## Project Structure

```text
Morocco_Electricity_Consumption_Analysis/
│
├── data/
│   ├── raw/
│   └── processed/
│       └── morocco_electricity_prepared.csv
│
├── notebooks/
│   └── Morocco_Electricity_Analysis.ipynb
│
├── visualizations/
│   ├── static/
│   └── interactive/
│
├── reports/
│   └── executive_summary.md
│
├── documentation/
│   ├── initial_data_quality_assessment.md
│   ├── data_preparation_log.md
│   ├── methodology_and_limitations.md
│   └── key_findings_and_recommendations.md
│
├── .gitignore
├── requirements.txt
└── README.md 
