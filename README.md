# ML‑Asset‑Management (Tutorial 5)

[![CI: Python application](https://github.com/LosingTouch/ml-asset-management/actions/workflows/python-app.yml/badge.svg)](https://github.com/LosingTouch/ml-asset-management/actions/workflows/python-app.yml)

**Machine Learning for Asset Management**  
Tutorial 5 code for ESILV’s *C++ & Python for Finance* course.

This project covers:

- **OLS & Regression Trees** – forecasting EUR / USD with MACD & RSI  
- **Mean–Variance Optimization** (classic & L₂‑regularized)  
- **Risk Parity** – equal‑risk contributions  
- **Hierarchical Risk Parity** – clustering + risk‑parity allocation  
- **Backtests & metrics** (Sharpe ratio, max drawdown)

---

## ✨ Key Features

| Module                                    | File / Script                        |
|-------------------------------------------|--------------------------------------|
| Data ingestion & preprocessing            | `src/data_loader.py`                 |
| RSI & MACD indicator computation          | `src/indicators.py`                  |
| OLS & Lasso regression                    | `src/models/ols_lasso.py`            |
| Regression trees (DecisionTreeRegressor)  | `src/models/tree.py`                 |
| Mean–Variance & Ridge portfolio optimizer | `src/portfolio/mvo.py`               |
| Classical Risk Parity                     | `src/portfolio/rp.py`                |
| Hierarchical Risk Parity                  | `src/portfolio/hrp.py`               |
| Backtest & performance metrics            | `src/backtest.py`                    |

---

## 📁 Folder Structure

```
ml-asset-management/
├── data/             # CSV inputs (EURUSD, stock prices)
├── notebooks/        # Jupyter notebooks (.ipynb)
├── src/              # Python scripts (.py)
├── .github/
│   └── workflows/    # CI pipeline definitions (YAML)
├── requirements.txt  # Python dependencies
└── README.md         # Project overview (this file)
```

---

## 🛠️ Installation & Setup

```bash
git clone https://github.com/LosingTouch/ml-asset-management.git
cd ml-asset-management

# (optional) create & activate a virtual environment
python3 -m venv .venv
source .venv/bin/activate    # macOS/Linux
.venv\Scripts\activate.bat   # Windows

pip install --upgrade pip
pip install -r requirements.txt
```

---

## ▶️ Running the Code

```bash
# run all backtests & generate plots
python src/backtest.py

# or launch the exploratory notebook
jupyter lab notebooks/MLTutorial5.ipynb
```

---

## 📜 License

MIT © Ihab M


