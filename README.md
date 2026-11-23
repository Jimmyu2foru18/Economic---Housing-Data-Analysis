# Economic & Housing Data Analysis

## Files
- `eda_analysis_executed.ipynb` — Jupyter notebook with full analysis
- `Stats annual economic & housing data 1990 - 2025.csv` — source data

## What the notebook does

1. **Exploratory Data Analysis** — time series plots, correlation heatmap, stationarity tests, Granger causality
2. **Model Comparison** — ARIMA, VAR, SARIMAX, OLS with Newey-West SEs
3. **5-Year Forecast (2026–2030)** — SARIMAX with 4 scenarios (Base, High Rate, Low Rate, Recession) plus prediction intervals
4. **Structural VAR** — sign-restricted SVAR with housing starts to identify causal effect of mortgage rates on home prices

## Key findings
- SARIMAX with exogenous Income & Mortgage Rate performs best (MAPE: 0.59%)
- Mortgage rates Granger-cause home prices (p=0.005)
- SVAR shows housing supply shocks dominate home price variation
- Base case forecast: median home price ~$458K in 2026 rising to ~$576K in 2029

## Run
Open `eda_analysis_executed.ipynb` in Jupyter to view all outputs.