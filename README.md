# Toronto Shooting Incidents Prediction

## Project Overview
The purpose of this project is to develop predictive models for the Toronto Police Services (TPS) to forecast shooting call volumes based on neighborhood metrics and weather factors. The goal is to provide solutions to allocate resources more effectively across police divisions to reduce or prevent future incidences.

## Objectives
1. Determine how neighborhood metrics (income, education, household size) and weather characteristics (snow, precipitation, temperature, visibility) affect shooting incidences in Toronto.
2. Develop models to predict call density per division and the number of casualties per incident.
3. Provide recommendations for the TPS to improve resource allocation and incident response.

## Data
- **Dataset Name:** Toronto Neighborhood Profile and Weather Data
- **File Name:** Adjusted_Flight_Price_Time_Series.csv (for example data, replace with relevant data file names)

## Methodology
1. **Data Intake & Manipulation:**
   - Ingest external datasets and merge by neighborhood values.
   - Clean and preprocess data (fixing datatypes, updating column names, encoding categorical data).

2. **Grouping and Aggregation:**
   - Group data by neighborhood number, year, and division.
   - Aggregate columns appropriately (sum, mean, mode, etc.).

3. **Feature Engineering:**
   - Create additional variables: Prosperity Index, Income Per Family Member Index, Division Risk, Call Density.

4. **Feature Impact Analysis:**
   - Identify significant variables using correlation coefficient, R-Squared testing, and Decision Tree Feature Importance.

5. **Model Testing:**
   - Test models: Linear, Ridge, Lasso, ElasticNet.
   - Select Ridge Regression based on performance metrics (RMSE, R-Squared, etc.).

## Recommendations
1. **Ridge Regression Model:** Use to allocate police resources based on predicted call density per division per year.
2. **Decision Tree Model:** Use to allocate resources based on daily weather conditions.
3. **Neighborhood Metrics:** Track long-term trends to predict future developments in neighborhoods.

## Contents
- `Toronto_Shooting_Incidents_Prediction.ipynb`: Jupyter Notebook containing the entire analysis, including data intake, manipulation, feature engineering, model testing, and recommendations.
- `data/`: Folder containing the datasets used for analysis.

## Tools and Libraries Used
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn

## How to Run
1. Clone this repository: `git clone https://github.com/mredshaw/Toronto_Shooting_Incidents_Prediction.git`
2. Open the Jupyter Notebook: `Toronto_Shooting_Incidents_Prediction.ipynb`
3. Execute the cells in the notebook to see the analysis and results.

## Key Insights
The notebook provides detailed insights into the factors influencing shooting incidences in Toronto and offers predictive models to help TPS allocate resources more effectively.
