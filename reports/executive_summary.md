# Executive Summary

## Morocco Electricity Consumption Analysis

### 1. Project Overview

This project examines electricity consumption readings across three geographical zones in Morocco using Python-based exploratory data analysis and visualisation.

The analysis investigates differences between zones, hourly and monthly patterns, and statistical relationships between recorded environmental variables and electricity consumption.

### 2. Dataset Overview

The dataset contains 52,416 observations and nine original columns, covering 1 January to 30 December 2017 at 10-minute intervals.

Data preparation included datetime validation, missing-value checks, duplicate checks, interval verification, outlier investigation and the creation of temporal features.

No missing values, duplicate timestamps, exact duplicate rows, invalid datetime values, irregular recording intervals or negative numerical values were identified during the reported quality checks.

Potential statistical outliers were retained because they could represent genuine demand patterns rather than data errors.

### 3. Key Findings

**Differences between geographical zones**

- Zone 1 recorded the highest mean consumption reading: approximately 32,344.97.
- Zone 2 followed at approximately 21,042.51.
- Zone 3 recorded the lowest mean at approximately 17,835.41.

**Hourly demand patterns**

All three zones recorded their highest average hourly readings at 20:00:

- Zone 1: approximately 43,822.59.
- Zone 2: approximately 28,186.91.
- Zone 3: approximately 26,027.61.

This shared evening peak provides a useful focus for further demand monitoring.

**Monthly patterns**

- Zone 1 recorded its highest monthly average in August.
- Zone 2 also recorded its highest monthly average in August.
- Zone 3 recorded its highest monthly average in July.

The monthly patterns were not identical across the three zones.

**Environmental relationships**

Temperature had positive Pearson correlations with consumption in all three zones:

- Zone 1: 0.44.
- Zone 2: 0.38.
- Zone 3: 0.49.

Humidity had negative Pearson correlations with consumption across all three zones. These results describe statistical associations and do not establish causal relationships.

### 4. Business Recommendations

1. Prioritise monitoring of the observed evening demand peak, particularly between 19:00 and 21:00.
2. Maintain zone-specific monitoring to identify differences in consumption patterns.
3. Investigate temperature and humidity as potential variables in future demand-forecasting models.
4. Review unusually high Zone 3 readings observed around 23–27 July 2017 to establish whether they reflect genuine demand or measurement issues.
5. Improve data documentation by confirming measurement units, interval conventions and environmental variable definitions.

### 5. Limitations

The dataset covers one year of observations and does not include 31 December 2017. The exact measurement convention for each 10-minute consumption reading has not been independently confirmed.

The definitions and units of GeneralDiffuseFlows and DiffuseFlows also require clarification.

The analysis is descriptive. It does not establish causation, explain the underlying reasons for zone differences, or prove that one zone is more energy-efficient than another.

### 6. Conclusion

The analysis identifies differences in consumption across the three geographical zones, a common evening peak and relationships between consumption and selected environmental variables.

These findings provide a starting point for more detailed demand monitoring and forecasting research. Stronger operational conclusions will require confirmed measurement definitions, additional years of data and relevant infrastructure and operational context.

### 7. Tools Used

Python, Jupyter Notebook, Pandas, NumPy, Matplotlib, Seaborn and Plotly.
