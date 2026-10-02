# Data Mining Portfolio | INF8111

A collection of applied data-mining projects completed for the INF8111 course. The notebooks cover data preparation, association-rule mining, and fraud-oriented anomaly detection using Python.

**Focus areas:** data cleaning and feature engineering, exploratory analysis, frequent-itemset mining, association rules, anomaly detection, model evaluation, and communicating findings.

## Projects

### 01 | House-price data preparation

Prepare and explore a housing-sales dataset for downstream price modelling. The notebook examines missing values and feature types, transforms the target with a logarithm, explores outliers, and applies data-cleaning and feature-selection techniques.

- Dataset: 2,919 housing records and 13 source columns.
- Methods: pandas, NumPy, scikit-learn, correlation analysis, IQR, visual exploration.
- Notebooks: [Team submission](notebooks/tp1/TP1_equipe54.ipynb) · [Development version](notebooks/tp1/TP1_version_developpement.ipynb) · [Course template](notebooks/tp1/TP1_template.ipynb)
- Data: [Housing data](data/tp1/data.csv)

### 02 | Retail market-basket analysis

Analyze retail transactions to identify product groups that are frequently purchased together. Compare Apriori with a hand-built FP-Growth workflow and examine how support and confidence thresholds affect the results.

- Data: retail transaction workbook and a product-to-category mapping covering 31 groups.
- Methods: transaction aggregation, one-hot encoding, Apriori, FP-tree construction, support, confidence, and lift.
- Notebooks: [Completed analysis](notebooks/tp2/TP2_solution.ipynb) · [Course template](notebooks/tp2/TP2_template.ipynb)
- Data: [Transactions](data/tp2/retail_dataset.xlsx) · [Product groups](data/tp2/grouped.json)

### 03 | E-commerce fraud and anomaly detection

Explore statistical, clustering, reconstruction-based, and local-density methods for detecting unusual e-commerce transactions, then evaluate their ability to identify labelled fraud.

- Methods: robust statistics, clustering, autoencoders, and Local Outlier Factor (LOF).
- Notebook: [Anomaly-detection study](notebooks/tp3/TP3_detection_anomalies.ipynb)
- Data requirement: `transactions_ecommerce.csv` is not included because it was not among the supplied repository files. Obtain it from the course materials and place it in `data/tp3/` before running the data-loading cells.

## Run the notebooks

Use Python 3.10 or newer where supported by the required packages. From the repository root:

```bash
python3 -m venv .venv
source .venv/bin/activate
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
```

Open a notebook in VS Code or Jupyter and select `.venv` as its kernel. TensorFlow installation support depends on the Python version and platform.

## Repository layout

```text
data/       Supplied datasets and data notes, organized by assignment
notebooks/  Notebooks organized by assignment
README.md   Project overview and execution notes
requirements.txt
```

## Context

These are course assignments and include course templates and team-submission material. They demonstrate applied coursework rather than a production-ready package. Review team identifiers and course rules before publishing the repository publicly.
