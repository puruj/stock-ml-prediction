# Predict the Stock Market with Machine Learning (Python)


> Educational replication of a time‑series ML tutorial using Python & JupyterLab. **Not financial advice.**


![Project Banner](results/example_banner.png)


## Overview
This repo walks through fetching historical prices, feature engineering (returns, rolling stats, technical indicators), model training (baseline + ML), and backtesting a simple strategy. It’s meant to showcase clean notebooks, reproducible results, and responsible claims.


## What’s inside
- **Notebook**: [`notebooks/predict_sp500.ipynb`](notebooks/predict_sp500.ipynb)
- **Results**: PNG charts & CSV metrics in [`results/`](results/)
- **Helpers**: Small utilities in [`src/`](src/)


## Data
- Source: Yahoo Finance (via `yfinance`) or a CSV you export yourself.
- Ticker(s): default `^GSPC` (S&P 500). Edit in the first notebook cell.
- **Note**: Large datasets are **not** checked in; see `data/` section below.


## Reproducibility
- Python ≥ 3.10
- Install deps:


```bash
python -m venv .venv && source .venv/bin/activate # Windows: .venv\Scripts\activate
pip install -r requirements.txt
jupyter lab
