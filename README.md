# Econometric Analysis of U.S. Money Supply (M2) & Inflation (1959–2025)

**Module:** Data Modelling
**Project Type:** Individual Coursework
**Language & Environment:** R (v4.x)

## Project Overview

This individual coursework project analyses the relationship between **U.S. Broad Money Supply (M2)** and **inflation (CPI)** using econometric modelling techniques in R.

The analysis covers monthly U.S. economic data from **January 1959 to August 2025** and includes regression modelling, lagged effects, diagnostic testing, forecasting, scenario analysis, and nonlinear polynomial modelling.

## Analysis Covered

The coursework consists of two main parts.

### Part 1 – Simple Regression Analysis

The analysis includes:

* Calculation of M2 growth and inflation rates
* Time-series exploration and visualisation
* Correlation analysis
* Simple linear regression
* Analysis of a 3-month lagged M2 growth rate
* Predictions and scenario-based inflation forecasts

### Part 2 – Multiple & Polynomial Regression

The analysis extends the modelling approach to include:

* Multiple Linear Regression
* 3-month lagged M2 growth
* 1-month lagged inflation
* Regression diagnostic testing
* Multicollinearity assessment
* Autocorrelation testing
* Residual normality assessment
* Heteroskedasticity testing
* HC1 robust standard errors
* Expansionary and contractionary policy scenarios
* Quadratic polynomial regression
* Model comparison using AIC and BIC

## Key Findings

* Contemporaneous monthly M2 growth showed a weak negative correlation with inflation (**r = -0.067**).
* Introducing a 3-month lag resulted in a statistically significant positive effect of lagged M2 growth on inflation (**β = 0.0879, p = 0.00118**).
* Including lagged inflation substantially improved the model's explanatory power, with **R² increasing from 0.0132 to 0.3257**.
* Lagged inflation was statistically significant (**β = 0.5559, p < 2 × 10⁻¹⁶**).
* No significant multicollinearity issues were identified, with **VIF < 1.13**.
* The Durbin-Watson test indicated no significant residual autocorrelation (**DW = 2.074, p = 0.8355**).
* Residual normality was not supported by the Shapiro-Wilk test (**p < 0.001**).
* HC1 robust standard errors were used to assess the robustness of the regression results, with key variable significance remaining intact.
* The Multiple Linear Regression model performed better than the Quadratic Polynomial Model based on AIC and BIC.

| Model                           |    AIC |    BIC |
| ------------------------------- | -----: | -----: |
| Multiple Linear Regression      | 307.46 | 330.86 |
| Quadratic Polynomial Regression | 310.68 | 334.08 |

## Dataset

The analysis uses monthly U.S. data covering **1959–2025**, with the main variables being:

| Variable          | Description              | Unit               |
| ----------------- | ------------------------ | ------------------ |
| `Date`            | Monthly observation date | YYYY-MM-DD         |
| `Money Supply M2` | Broad Money Supply       | Billions USD       |
| `CPI`             | Consumer Price Index     | Index (2015 = 100) |

The dataset contains **800 monthly observations**, covering January 1959 to August 2025.

## R Code

The **R code used for the analysis is included within the PDF report**. The report contains the code together with the corresponding analysis, results, visualisations, diagnostic tests, and interpretations.

No separate R scripts, raw dataset, or assignment question document are included in this repository.

## Repository Contents

```text
m2-inflation-analysis/
│
├── AssignmentDM.pdf
│
└── README.md
```

### Report.pdf

The PDF contains the complete individual coursework, including:

* R code
* Data analysis
* Econometric models
* Statistical results
* Visualisations
* Diagnostic tests
* Forecasting and scenario analysis
* Model comparison
* Interpretation and conclusions

## Tools & Techniques

* **R 4.x**
* RStudio
* Econometric modelling
* Time-series analysis
* Linear regression
* Multiple Linear Regression
* Polynomial regression
* Lagged-variable analysis
* Regression diagnostics
* Robust standard errors
* Forecasting
* Data visualisation

## Skills Demonstrated

This individual project demonstrates practical application of:

* Econometric analysis
* Statistical modelling
* Time-series analysis
* Regression modelling
* Statistical inference
* Model diagnostics
* Forecasting and scenario analysis
* R programming
* Data interpretation
* Economic data analysis

## Conclusion

The analysis demonstrates the importance of considering **lagged money supply effects and inflation persistence** when modelling inflation.

The results indicate that the relationship between M2 growth and inflation is more evident when a time lag is incorporated, while lagged inflation provides substantial additional explanatory power. Among the models compared, the **Multiple Linear Regression model** provided the preferred specification based on the reported model comparison criteria.
