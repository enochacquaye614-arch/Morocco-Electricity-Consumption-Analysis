# Analytical Methodology and Limitations

## Analytical Approach
The project uses Python-based exploratory data analysis to examine electricity consumption across three geographical zones and explore relationships with recorded environmental variables.

## Tools and Libraries
- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- Plotly
- SciPy and Statsmodels, where applicable

## Analysis Methods
- Descriptive statistics: mean, median, minimum, maximum and standard deviation.
- Temporal aggregation: hourly, daily, weekly and monthly averages.
- Zone comparison: grouped summaries, bar charts, boxplots and heatmaps.
- Environmental analysis: Pearson and Spearman correlation.
- Outlier screening: interquartile range (IQR).
- Visualisation: static Matplotlib/Seaborn charts and interactive Plotly charts.

## Important Limitations

### Measurement Units
The data dictionary describes consumption in kWh, but the exact measurement convention for each 10-minute observation has not been independently confirmed. Therefore, this analysis refers to recorded consumption readings and does not assume that summing the readings produces verified total energy consumption.

### Environmental Variable Definitions
The precise physical definitions and units of `GeneralDiffuseFlows` and `DiffuseFlows` require confirmation from the data provider. Their physical meaning should not be inferred from their names alone.

### Correlation and Causation
Pearson and Spearman correlations identify statistical associations. They do not demonstrate that environmental conditions cause changes in electricity consumption. Time of day, seasonality and other potential confounding factors may influence observed relationships.

### Time Coverage
The dataset covers 1 January to 30 December 2017. It does not contain 31 December 2017 or multiple years of observations. Findings should not be treated as evidence of long-term trends.

### Outliers
IQR flags identify values outside statistical thresholds, not necessarily erroneous measurements. Flagged values were retained unless there was evidence that they were invalid.

### Contextual Data
The dataset does not provide sufficient information about population, customer numbers, installed capacity, tariffs or operational conditions to explain why zones differ or to establish comparative efficiency.

## Interpretation Principle
All findings are descriptive and should be interpreted within the coverage, definitions and limitations of the available dataset.
