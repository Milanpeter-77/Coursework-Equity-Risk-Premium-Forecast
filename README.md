# Forecasting Equity Risk Premium

This project investigates the **forecastability of the equity risk premium** using historical macroeconomic and financial predictors. The analysis is fully implemented in Python within a Jupyter notebook environment and forms part of a quantitative finance group coursework project.

The study focuses on **predictive regression frameworks**, where excess market returns are modeled as a function of lagged predictor variables such as valuation ratios, interest rate spreads, and macro indicators. Both **in-sample** and **out-of-sample** forecasting performances are evaluated.

## Methodology

1. **Data Preparation**

   * Load and clean historical time series data of the equity market excess return and multiple predictive variables.
   * Align and lag predictors to ensure information availability consistency.
   * Handle missing values and normalize predictors when necessary.

2. **Predictive Regressions**

   * Estimate **univariate and multivariate predictive regressions** of the form
     
    $$r_{t+1} = \alpha + \beta x_t + \varepsilon_{t+1}$$
     
     where $(r_{t+1})$ is the equity risk premium and $(x_t)$ represents one or more lagged predictors.
   * Evaluate the **statistical significance** of coefficients to identify meaningful predictors.

3. **Out-of-Sample Forecasting**

   * Implement **expanding and rolling window forecasts** to simulate real-time prediction.
   * Compute performance metrics such as:

     * Out-of-sample $(R^2)$,
     * Mean Squared Forecast Error (MSFE),
     * Economic utility gains relative to a historical mean benchmark.

4. **Model Comparison & Robustness**

   * Compare single-predictor and kitchen-sink (multi-predictor) models.
   * Assess model stability and robustness across different sample periods.
   * Visualize forecast performance and error behavior over time.

5. **Interpretation**

   * Discuss which variables exhibit genuine predictive power.
   * Link model outcomes to theoretical explanations of **time-varying risk premia** and **business-cycle dynamics**.

The notebook and accompanying report document the **full empirical workflow** – from data import and regression estimation to out-of-sample evaluation and interpretation—highlighting the methodological rigor behind forecasting the equity risk premium in a reproducible way.
