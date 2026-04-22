# 📱 Smartphones 2025–2026: Value-for-Money Analysis

[![Python](https://img.shields.io/badge/Python-3.10-blue)](https://www.python.org/) [![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)](https://jupyter.org/) [![Scikit-learn](https://img.shields.io/badge/ML-Scikit--learn-red)](https://scikit-learn.org/)

A comprehensive data science case study on **997 smartphones** (Budget to Flagship) sourced from Smartprix — April 2026. This project demonstrates the full data science workflow: ingestion, cleaning, exploratory analysis, hypothesis testing, and supervised ML modelling.

---

## 🎯 Objectives
1. Understand how hardware specs scale across price segments
2. Identify **Value Kings** — devices that punch above their price bracket
3. Answer: *does a ₹1L phone offer 5× the value of a ₹20K phone?*
4. Build a regression model to predict smartphone prices from specs

## 📂 Project Structure
```
├── smartprix_smartphones_april_2026.csv   # Raw dataset
├── smartphone_vfm_analysis.ipynb          # Main analysis notebook
└── README.md
```

## 🔬 Methodology
| Stage | Details |
|-------|---------|
| Data Cleaning | Median-per-category imputation, feature engineering |
| EDA | 15+ visualisations across brands, categories, connectivity, charging |
| Business Analysis | Premium Gap, Brand Wars, Value King profiling |
| ML Models | Linear Regression, Ridge, Random Forest, Gradient Boosting |
| Evaluation | R², MAE, RMSE, 5-fold CV, residual analysis |

## 📊 Key Results
- **Gradient Boosting** achieved the best generalisation across price segments
- Flagship devices cost **7× more** than Budget but deliver only **1.6× the spec score**
- ~82.5% of price predictions fall within 20% of the actual price
- Top predictors: `processor_speed` (37%), `price_category` (14%), `vfm_score` (9%)

## 🛠️ Tech Stack
`Python 3.10` · `Pandas` · `NumPy` · `Matplotlib` · `Seaborn` · `Scikit-learn`

## 📦 Installation
```bash
git clone https://github.com/your-username/smartphone-vfm-analysis.git
cd smartphone-vfm-analysis
pip install -r requirements.txt
jupyter notebook smartphone_vfm_analysis.ipynb
```

## 📌 Data Source
Scraped from [Smartprix](https://www.smartprix.com) using Selenium + BeautifulSoup · April 2026
