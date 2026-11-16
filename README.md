# Customer Churn Prediction

An end-to-end data science project to explore customer churn, identify its key drivers, and build an interpretable machine-learning model to estimate churn risk.

> **Project status:** Setup and data exploration phase. Model results will be added only after experiments are run and validated.

## Business problem

Customer churn affects recurring revenue and makes retention planning harder. This project will use customer account and service information to:

- Measure and describe customer churn.
- Explore which customer characteristics are associated with churn.
- Build and evaluate classification models.
- Explain model predictions and translate findings into practical retention insights.

## Dataset

The project is designed around the **IBM Telco Customer Churn** dataset.

- Source: [IBM Telco Customer Churn on GitHub](https://github.com/IBM/telco-customer-churn-on-icp4d)
- Alternative download page: [Kaggle – Telco Customer Churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)

Download the data yourself and follow [data/README.md](data/README.md). The raw dataset is intentionally not committed to this repository.

## Planned workflow

1. **Data understanding:** inspect schema, data quality, target distribution, and business context.
2. **Exploratory analysis:** examine churn patterns across contract, tenure, billing, and service features.
3. **SQL analysis:** answer business questions using joins, CTEs, aggregations, and window functions where appropriate.
4. **Feature preparation:** handle missing values, encode categorical variables, and establish leakage-safe preprocessing.
5. **Modeling:** create a baseline and compare suitable classification models.
6. **Evaluation:** use metrics appropriate for class imbalance, including precision, recall, F1, ROC-AUC, and PR-AUC.
7. **Interpretation:** analyze important features and model behavior.
8. **Deployment extension:** expose the selected model through an API and document reproducible usage.

## Repository structure

```text
.
├── data/
│   └── README.md
├── notebooks/
│   └── README.md
├── sql/
│   └── README.md
├── src/
│   └── README.md
├── reports/
├── requirements.txt
└── README.md
```

## Getting started

Create and activate a virtual environment, then install dependencies:

```bash
python -m venv .venv
# macOS / Linux
source .venv/bin/activate
# Windows PowerShell
.venv\Scripts\Activate.ps1

pip install -r requirements.txt
```

Place the downloaded CSV at `data/raw/WA_Fn-UseC_-Telco-Customer-Churn.csv` (or update the notebook path to match your downloaded filename).

## Current status

- [x] Create repository and project documentation
- [ ] Download dataset and verify its source
- [ ] Complete data-quality checks and exploratory analysis
- [ ] Write SQL business analyses
- [ ] Establish baseline model
- [ ] Compare and interpret models
- [ ] Add tests and reproducible training pipeline
- [ ] Build and document prediction API

## Reproducibility

Python dependencies are listed in [requirements.txt](requirements.txt). Random seeds, evaluation choices, and experiment settings will be documented as the project develops.

## Author

Created as a portfolio project demonstrating practical data analysis, SQL, machine learning, and reproducible engineering practices.
