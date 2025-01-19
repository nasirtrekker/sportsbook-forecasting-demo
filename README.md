# LeoVegas Sportsbook Turnover Forecasting Project

This repository contains three notebooks and their respective PDF reports focusing on sportsbook turnover prediction for LeoVegas. The project demonstrates data preprocessing, exploratory data analysis (EDA), advanced time series forecasting, and prediction reliability through conformal methods.

## Project Files
### Notebooks
- **`sportbookprediction_analysis-cpconformal.ipynb`**
  - Demonstrates conformal uncertainty estimation.
  - Explores prediction intervals to quantify the uncertainty in forecasts.

- **`v2_sportbookprediction_automl.ipynb`**
  - Implements AutoML tools like FLAML and H2O to automate feature engineering and hyperparameter tuning.
  - Focuses on feature-rich predictive models using ensemble techniques.

- **`v3_sportbookprediction_analysis-timeseris.ipynb`**
  - Implements advanced time-series forecasting techniques such as SARIMA.
  - Provides diagnostic residual analysis and uncertainty intervals for time-series predictions.

### PDF Reports
- **`sportbookprediction_analysis-cpconformal.pdf`**: Report summarizing conformal uncertainty estimation.
- **`v2_sportbookprediction_automl.pdf`**: Report summarizing machine learning workflows using AutoML tools.
- **`v3_sportbookprediction_analysis-timeseris.pdf`**: Detailed SARIMA time-series analysis with forecasting results.

## How to Execute the Notebook
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/nasirtrekker/sportsbook-forecasting-demo.git
   cd sportsbook-forecasting-demo


*Requirements* : 
 The project requires the following Python packages:

pandas
numpy
matplotlib
seaborn
statsmodels
xgboost
FLAML
H2O AutoML
mapie

A complete list of dependencies is provided in the requirements.txt file.

*Key Objectives* 

*Prediction Target:*  total_turn_over_EUR, representing the total betting turnover.
*Forecasting Models:*

Advanced machine learning (AutoML, ensemble models).
Time series forecasting (SARIMA, ETS decomposition).
Conformal uncertainty estimation for prediction intervals.

*Business Insights:*

- Identify high-turnover periods for marketing.
- Predict engagement trends using seasonal patterns.
- Offer stakeholder-friendly uncertainty intervals.

## Visualizations of Turnover Analysis

### 1. AutoARIMA SARIMA Residual Diagnostic Plot
![AutoARIMA SARIMA Residual Diagnostic](https://github.com/nasirtrekker/sportsbook-forecasting-demo/blob/main/plot_images/autoarima_sarima_residualDiagnosisplot.png)

### 2. Conformal Prediction for Turnover (90% Confidence Interval)
![Conformal Prediction Turnover](plot_images/cp_mapie_turnofer_pi90.png)

### 3. Daily Turnover Aggregation
![Daily Turnover Aggregation](plot_images/daily_turnover_aggr.png)

### 4. Decomposition of Original Data
![ETS Decomposition](plot_images/ETS_decom_originaldata.png)

### 5. Conformal Prediction on Time Series
![Conformal Prediction on Time Series](plot_images/timeseries_conformal_mapieNaive_turnover.png)

### 6. Total Turnover (Top 20 Leagues)
![Total Turnover Top 20 Leagues](plot_images/totalturnover_top20league.png)

### 7. Weekly Turnover Forecast with AutoARIMA
![Weekly Turnover Forecast](plot_images/weekly_forecast_turnover_autoarima.png)

### 8. Weekly Turnover Aggregation
![Weekly Turnover Aggregation](plot_images/weeklyturnover_aggr.png)

*Causal Inference: A Future Integration Possibility* 

The current repository and explanation focus on forecasting and conformal uncertainty estimation but do not include causal inference for deriving actionable insights. Causal inference involves determining cause-and-effect relationships between variables, going beyond statistical associations to understand how changes in one variable (e.g., marketing campaigns) directly impact another (e.g., total turnover). Implementing causal inference would require identifying key variables: the treatment variable (e.g., marketing campaigns), the outcome variable (e.g., total_turn_over_EUR), and potential confounders (e.g., seasonality or day of the week). Data preparation is essential to include these variables and ensure a clean dataset. Analytical methods such as Propensity Score Matching (PSM), Difference-in-Differences (DiD), Instrumental Variables (IV), or causal graphs (DAGs) could then be applied. Python libraries such as dowhy and econml provide streamlined approaches for causal inference, enabling businesses to derive actionable insights and assess the direct impact of interventions on turnover. This integration could further enhance decision-making by supporting “what-if” scenarios and simulations.


*GitHub Repository* 

The repository can be accessed here: [LeoVegas Sportsbook Forecasting Demo](https://github.com/nasirtrekker/sportsbook-forecasting-demo.git)

Author : Nasir Uddin
Contact: nasiru32@gmail.com
