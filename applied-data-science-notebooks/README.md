# Applied Data Science Notebooks

Python notebooks from ISM4543 Applied Data Science (University of South Florida, Fall 2026).
Each one solves a business problem for a client, from framing the question to a recommendation in dollars.

**Tools:** Python, pandas, NumPy, Matplotlib, seaborn, scikit-learn, Google Colab

## Projects

| # | Client | Business question | Methods |
|---|---|---|---|
| 1 | [Bay Harbor Coffee](notebooks/01_bay-harbor-coffee_ai-assisted-eda.ipynb) | What drives a busy day at a café, and can staffing be planned from sales data? | Exploratory analysis, correlation, problem framing |
| 2 | [Northwind Fitness](notebooks/02_northwind-fitness_data-cleaning-churn.ipynb) | Which gym members are leaving, and why? | Data cleaning (duplicates, missing values, messy labels), NumPy, groupby, charts |
| 3 | [ClearPath Health](notebooks/03_clearpath-health_feature-engineering.ipynb) | Preparing patient data for analysis | Data preparation, feature engineering |
| 4 | [Pelican Row Growers](notebooks/04_pelican-row-growers_regression.ipynb) | Find the hidden relationship in farm data | Regression |
| 5 | [QuickLend Financial](notebooks/05_quicklend_logistic-regression-credit-risk.ipynb) | Which loan applicants are likely to default, and where should the approval cutoff sit? | Logistic regression, pipelines, confusion matrix, cost-based threshold tuning, odds ratios |
| 6 | [ClearView Auto Insurance](notebooks/06_clearview-insurance_knn-churn.ipynb) | Who should the retention team call first each month? | K-nearest neighbors, scaling, feature selection, cross-validation, ranking by expected savings |

## Highlights

- **Credit risk (QuickLend):** chose the approval threshold from the real cost of each mistake ($15,000 per missed default vs. $3,000 per rejected good loan) instead of the default 0.5 cutoff.
- **Insurance churn (ClearView):** built a ranked call list that reached 82 of 104 leavers with 200 calls in the test set, saving about $84,000 vs. a random list. Scaling and dropping weak features raised leavers found by 58 and 29.
- **Verification habit:** every notebook checks AI-generated code against the data and logs the errors caught.

## How to run

Open any notebook in Google Colab or Jupyter. Datasets load from the course data repository by URL, so no downloads are needed.

## Note

Datasets are simulated for teaching. Assignment prompts were written by the course instructor; the analysis, code checks and written answers are my own.
