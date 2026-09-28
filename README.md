# StockSense: Stock Market Risk & Price Prediction Pipeline

A machine learning pipeline that analyzes global daily stock trading data. It predicts the direction of next-day price movement (supervised classification) and discovers market regimes and stock behavior groups (unsupervised clustering), with feature analysis for interpretability.

**Course:** IT7009 Artificial Intelligence, Bahrain Polytechnic
**Assessment:** Group Project (35%)
**Environment:** Google Colab (`.ipynb`)

---

## Project Overview

Financial time-series data is noisy, high-dimensional, and complex. This project builds an automated ML pipeline that:

1. **Classifies** the direction of a stock's next-day closing price (increase, decrease, or stable).
2. **Clusters** stocks and market conditions by behavior and volatility, without labels.
3. **Explains** which features (returns, volume changes, technical indicators) drive predictions.
4. **Evaluates** the approach critically, covering effectiveness, limitations, and practical deployment.

## Dataset

Multiple CSV files, each holding the daily historical trading data of one stock.

| Column | Description |
|---|---|
| Date | Trading date |
| Open | Price at market open |
| High | Highest price of the day |
| Low | Lowest price of the day |
| Close | Price at market close |
| Adj Close | Adjusted closing price |
| Volume | Number of shares traded |

Missing values occur on non-trading days (weekends, holidays, exchange suspensions).

---

## Work Distribution

| Team Member | Responsibility | Details |
|---|---|---|
| **Raghad Aleskafi** | Dataset preprocessing | Data loading and merging, handling missing values, cleaning and formatting, data consistency checks |
| **Zahraa Hubail** | Dataset preprocessing | Data loading and merging, handling missing values, cleaning and formatting, data consistency checks |
| **Norain Almajed** | Supervised learning | Target label creation, feature construction, model selection and training, tuning, classification metrics, model comparison |
| **Fatima Alaiwi** | Unsupervised learning | Clustering algorithm selection, identifying stock and market-regime groups, volatility structure analysis, cluster evaluation and interpretation |

---

## Repository Structure

```
├── notebook/
│   └── stock_risk_price_prediction.ipynb   # Full pipeline (preprocessing, supervised, unsupervised)
├── report/
│   └── Project_Report.docx                 # Final project report
├── data/                                   # Dataset (or link to source if large)
├── requirements.txt
└── README.md
```

## Pipeline Stages

1. **Data Preparation:** cleaning, missing-value handling, formatting
2. **Feature Development:** returns, volume changes, technical indicators
3. **Supervised Classification:** predicting next-day price direction
4. **Unsupervised Learning:** clustering stocks and market regimes
5. **Feature Analysis & Interpretability:** feature importance scores
6. **Evaluation & Reflection:** metrics, comparison, limitations

## How to Run

1. Open the notebook in [Google Colab](https://colab.research.google.com/).
2. Upload the dataset CSV files (or mount Google Drive and update the data path).
3. Run all cells from top to bottom (`Runtime → Run all`).

## Requirements

Install dependencies with:

```bash
pip install -r requirements.txt
```

Typical libraries: `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`.

## Team

- Fatima Alaiwi
- Norain Almajed
- Raghad Aleskafi
- Zahraa Hubail
