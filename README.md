# Spotify Streaming Audit: Premium Playlist Optimization

## 📊 Business Case (SCQA Framework)

### Situation
Our streaming platform currently hosts a growing catalog of 2,000 distinct tracks. To drive user engagement and premium subscriptions, the business relies on curated "Premium Playlists" as a core product feature. 

### Complication
There is currently **no data-driven selection criteria** to determine which tracks qualify for premium status. This lack of segmentation leads to sub-optimal playlist curation, potentially diluting the premium user experience, underutilizing high-performing content, and leaving valuable catalog segments completely unmonitored.

### Question
How can we identify high-performing content segments and establish a scalable, data-backed framework to optimize our premium playlist catalog?

### Answer & Executive Summary
As Junior Data Consultants, Team 3 has developed an end-to-end analytical and machine learning framework that evaluates the catalog across performance quartiles and decades. By leveraging acoustic attributes, we built:
1. A **Clustering Model (K-Means)** to discover and profile unique musical "vibes".
2. A **Regression Pipeline** to predict track popularity scores.
3. An **Interactive Executive Dashboard** to translate these insights into actionable business decisions.

---

## 🚀 Key Project Deliverables

* **Exploratory Data Analysis (EDA):** A clean, end-to-end reproducible Python workflow identifying correlation thresholds between acoustic attributes and popularity scores.
* **Advanced SQL Auditing (DuckDB):** Targeted queries segmenting performance by era (decades) and track popularity quartiles to isolate low and high-performing content.
* **Vibe Clustering (Unsupervised ML):** K-Means clustering over normalized acoustic features (validated via Silhouette Score) to map the catalog's sonic landscape.
* **Popularity Predictor (Supervised ML):** A trained regression pipeline compared across multiple algorithms, evaluated using RMSE and R², and exported via `joblib` for instant inference.
* **Executive Dashboard:** A highly focused interactive dashboard (built with zero decorative clutter) mapped to strategic business KPIs.

---

## 📁 Repository Structure

```text
├── data/
│   ├── raw/            # Original immutable datasets
│   └── processed/      # Normalized and engineered features
├── notebooks/
│   ├── 01_eda_pandas.ipynb
│   ├── 02_clustering_vibes.ipynb
│   └── 03_regression_popularity.ipynb
├── sql/
│   ├── segmentacion_decadas.sql
│   └── cuartiles_popularity.sql
├── models/
│   └── popularity_predictor.joblib
├── dashboard/
│   └── dashboard_assets/
├── src/
│   ├── __init__.py
│   └── utils.py
├── README.md
└── requirements.txt
```

---

## 🛠️ Tech Stack & Prerequisites

+ Language & Environment: Python 3.x, VSCode (Git Bash)
+ Data Wrangling & Analytics: Pandas, DuckDB (SQL)
+ Machine Learning: Scikit-Learn, Joblib
+ Visualization & Dashboards: Tableau / Plotly Dash

---

## 👥 The Team (Group 3)

- Michelle Tirado Guerrero — Data Analyst
- Gustavo Segura — Data Scientist
- Emiliano Sandoval Samano — Data Analyst
- Aldo Tomás Orduña Fabila — Data Scientist

---

To replicate this environment locally, run:

Bash
```
pip install -r requirements.txt
```
Last update: May 26, 2026.
