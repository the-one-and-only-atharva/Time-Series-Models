# Time Series Models

Hands-on classical time series analysis and forecasting in Python — from mean models (AR/MA/ARMA/ARIMA) through seasonality, multivariate systems, and volatility (ARCH/GARCH), plus decomposition and Prophet.

![Python](https://img.shields.io/badge/Python-3.10+-blue)
![statsmodels](https://img.shields.io/badge/statsmodels-Time%20Series-green)
![arch](https://img.shields.io/badge/arch-GARCH-red)
![Prophet](https://img.shields.io/badge/Prophet-Forecasting-orange)

## What’s inside

| # | Notebook | Topics |
|---|----------|--------|
| 01 | [`ar_ma_arma_arima`](notebooks/01_ar_ma_arma_arima.ipynb) | AR, MA, ARMA, ARIMA; ACF/PACF; meteorological series |
| 02 | [`sarima_sarimax`](notebooks/02_sarima_sarimax.ipynb) | Seasonal ARIMA / SARIMAX with exogenous temperature |
| 03 | [`var`](notebooks/03_var.ipynb) | Vector Autoregression (ice cream vs heater) |
| 04 | [`arch`](notebooks/04_arch.ipynb) | ARCH volatility on market index returns |
| 05 | [`garch`](notebooks/05_garch.ipynb) | GARCH volatility modeling |
| 06 | [`arima_box_jenkins`](notebooks/06_arima_box_jenkins.ipynb) | Full Box–Jenkins workflow |
| 07 | [`decomposition_cma_ma`](notebooks/07_decomposition_cma_ma.ipynb) | Classical additive decomposition / CMA |
| 08 | [`holt_winters`](notebooks/08_holt_winters.ipynb) | Holt–Winters exponential smoothing |
| 09 | [`prophet`](notebooks/09_prophet.ipynb) | Prophet business forecasting |

## Techniques covered

- Stationarity testing (ADF)
- ACF & PACF analysis
- Model selection (AIC / BIC)
- Residual diagnostics
- Rolling forecasts & backtesting
- Forecast metrics (RMSE, MAE, MAPE)
- Volatility clustering (ARCH / GARCH)

## Project layout

```
Time-Series-Models/
├── data/                 # datasets used by the notebooks
│   ├── Index2018/
│   ├── catfish/
│   ├── ice_cream_vs_heater/
│   └── meteorological/
├── notebooks/            # numbered walkthroughs (run in order)
├── requirements.txt
└── README.md
```

## Setup

```bash
cd Time-Series-Models
python -m venv .venv
source .venv/bin/activate   # Windows: .venv\Scripts\activate
pip install -r requirements.txt
jupyter lab                 # or: jupyter notebook
```

Open notebooks from the `notebooks/` folder so relative `../data/...` paths resolve correctly.
