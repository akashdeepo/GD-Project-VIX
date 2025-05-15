# 📊 Google Search Sentiment & Market Volatility

This repository contains the code, data processing pipeline, and visualizations for our research on using Google search trends as an early-warning signal for financial market volatility (VIX spikes).

---

## 🔍 Overview

We study how public search behavior — particularly terms like “Recession”, “Financial Crisis”, and “Market Crash” — correlates with and often precedes spikes in market volatility.

Using:
- Google Trends data (2004–2025)
- VIX index data (2000–2024)
- Gold price data for safe-haven analysis

We build:
- A composite sentiment index (via PCA)
- A feature-rich dataset with rate-of-change and anomaly scores
- A machine learning model (XGBoost) to forecast VIX spikes
- A scoring-based **Early Warning System**

---

## 📈 Key Results

- **3.1× lift** in predicting VIX spikes within 1 month using sentiment anomalies
- Top terms (“Recession”, “Financial Crisis”) show **r > 0.65** correlation with VIX
- Gold prices tend to rise during peak fear periods
- Early-warning system achieved:
  - ROC AUC: **0.825**
  - F1 Score: **0.618**

---

## 🧠 Tech Stack

- **Language:** Python 3.8+
- **Notebook Interface:** Jupyter Notebooks
- **Libraries:**
  - `pandas`, `numpy` — data manipulation
  - `matplotlib`, `seaborn` — visualization
  - `scikit-learn` — preprocessing, metrics, PCA
  - `xgboost` — model training
  - `scipy.stats` — statistical transformations
  - `warnings`, `datetime` — utilities for clean analysis

---

## 📦 Dependencies & Installation

Install all required packages using:

```bash
pip install -r requirements.txt
````

Minimal `requirements.txt`:

```txt
pandas>=1.3.0
numpy>=1.21
matplotlib>=3.4
seaborn>=0.11
scikit-learn>=0.24
xgboost>=1.5
scipy>=1.7
jupyter
```

---



## 📄 License

MIT License.

---

## ✉️ Contact

**Gagan Deep, Akash Deep**
Texas Tech University
📧 [deep@ttu.edu](mailto:deep@ttu.edu)
🌐 [deepaifinance.com](https://deepaifinance.com)

> *“Search behavior may be noisy — but in chaos lies signal.”*

