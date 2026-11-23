# MachineLearning-2026.2

Final project for the Machine Learning course (2026.2), Internet Systems program. Instructor: Anthony Lins.
Track 3: Mobility and subscriptions.

| Task           | Dataset                         | Target  | Notebook                            |
|----------------|---------------------------------|---------|-------------------------------------|
| Regression     | Bike Sharing, hourly (UCI #275) | `cnt`   | `notebooks/01_regression.ipynb`     |
| Classification | Telco Customer Churn (IBM)      | `Churn` | `notebooks/02_classification.ipynb` |

Each task covers ETL, EDA, data-quality treatment, cross-validated modeling and statistical model comparison.
Dataset sources: [Bike Sharing](https://archive.ics.uci.edu/dataset/275/bike+sharing+dataset), [Telco Customer Churn](https://github.com/IBM/telco-customer-churn-on-icp4d).

## Setup

```bash
pip install -r requirements.txt
```

Notebooks run end to end on Google Colab (Runtime > Run all).

## Structure

```text
├── datas/
│   ├── raw/          original datasets, unmodified
│   └── processed/    cleaned datasets, data dictionary
├── notebooks/        regression and classification
├── reports/          report, AI usage log, slides
└── requirements.txt
```

## Conventions

- Random seed: 42.
- Train/test split precedes any fitted transformation.
- Preprocessing and resampling run inside `Pipeline` objects.
- AI usage is logged in `reports/ai_usage_log.xlsx`.

## Authors

- André Luís Gomes da Silva Filho
- Arthur Azevedo Costa de Paula
- Dayvson da Conceição de Moura
- Hallason Matias da Silva
- José Heitor Felix Guimarães
- Vinícius de Almeida Silva
