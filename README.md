# Obesity in the United States: Data-Driven Insights 📊

## Overview 📋
This project addresses the escalating obesity crisis in the United States, a major public health challenge affecting over 42% of adults. By leveraging demographic and health data, we aim to predict obesity trends, identify vulnerable populations, and guide targeted public health interventions.

## Technical Details 🔍

### Objectives 🎯
The analysis focuses on:
- Forecasting obesity trends across age groups and regions through 2023.
- Pinpointing high-priority geographic areas for public health actions.
- Highlighting at-risk demographic groups for efficient interventions.

### Data Sources 🌐
Two key datasets are utilized:
- **BRFSS (Behavioral Risk Factor Surveillance System)**: Annual survey data on obesity prevalence, physical activity, and health behaviors.
- **ACS (American Community Survey)**: Demographic statistics including age, income, and education levels.

These datasets are integrated to examine the interplay between socio-economic factors and obesity rates.

### Methodology ⚙️
The approach involves:
- **Age Segmentation**: Data is categorized into age brackets (e.g., 18-24, 25-34, 35-44).
- **Obesity Rate Extraction**: Regional and yearly obesity rates are computed for 2010–2023.
- **BRFSS Aggregation**: Individual-level BRFSS data is aggregated into synthetic indicators (e.g., `obesity_18_24`, `obesity_percentage`) by age and state.
- **ACS Integration**: BRFSS indicators are merged with ACS socio-demographic variables (e.g., income, age) based on literature-driven feature selection.
- **Correlation Analysis**: Relationships between demographic factors (e.g., income, healthcare access) and obesity rates are quantified to reveal regional disparities.

### Predictive Modeling 🤖
A suite of machine learning models predicts obesity trends:
- **Targets**: Obesity rates by age group and overall percentage.
- **Evaluation Metrics**:
  - **R²**: Measures variance explained by the model (higher is better).
  - **RMSE**: Assesses prediction accuracy (lower is better).
- **Selected Models**: Include Random Forest, Gradient Boosting, Elastic Net, and LGBMRegressor, chosen for optimal R² and RMSE performance.

### Key Findings 📈
- **Regional Variations**: States like Indiana show declining obesity rates, suggesting effective local policies, while Oregon and North Carolina exhibit increases, especially among seniors.
- **Age-Specific Trends**: Significant disparities emerge, e.g., a notable decrease in obesity among those over 65 in New Hampshire versus a rise in Oregon.

## Applications 🚀
- **Trend Prediction**: Forecasts obesity evolution to 2023 by age and region.
- **Intervention Prioritization**: Identifies high-risk zones and demographics for resource allocation.
- **Policy Simulation**: Models the potential impact of initiatives like improved food access or exercise programs.

## Limitations ⚠️
- Model performance varies across age groups (e.g., lower R² for some targets).
- Regional disparities may reflect data gaps or unmodeled local factors.

## Conclusion 🌟
This data-driven framework provides the CDC with a decision-support tool to combat obesity proactively, targeting vulnerable groups and optimizing public health strategies based on age- and state-specific insights.
