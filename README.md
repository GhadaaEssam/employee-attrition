# Employee Attrition Multivariate Analysis

This repository contains a multivariate statistics final project analyzing employee attrition using the IBM HR Analytics Employee Attrition & Performance dataset. The project studies attrition as an interconnected workforce problem rather than a single-variable HR metric.

The main analysis is implemented in a Jupyter notebook:

- `code/MULTIVARIATE_STATISTICS__FINAL_PROJECT.ipynb`

## Project Overview

Employee attrition creates financial, operational, and knowledge-retention risks for organizations. This project applies multivariate statistical methods to understand how employee characteristics such as age, compensation, rates, and tenure jointly describe workforce behavior and attrition risk.

The analysis focuses on the following response vector:

- `Age`
- `MonthlyIncome`
- `DailyRate`
- `HourlyRate`
- `YearsAtCompany`

These variables represent a mix of demographics, compensation, work-rate measures, and organizational tenure.

## Dataset

The notebook uses the IBM HR Analytics Employee Attrition & Performance dataset from Kaggle:

- Dataset: `pavansubhasht/ibm-hr-analytics-attrition-dataset`
- Records: 1,470 employees
- Features: 35 columns
- Target context: employee attrition and workforce profile analysis

The dataset is downloaded inside the notebook using `kagglehub`.

## Analysis Workflow

The notebook includes the following stages:

1. Data loading and feature selection
2. Data profiling, missing-value checks, and descriptive statistics
3. Distribution visualization for selected HR variables
4. Covariance and correlation analysis
5. Standardization of numeric variables
6. Mahalanobis-distance outlier detection
7. One-sample Hotelling T-squared test
8. Two-sample Hotelling T-squared test comparing employees who left vs. stayed
9. Confidence regions and simultaneous confidence intervals
10. Paired Hotelling T-squared analysis for initiative evaluation
11. Final business interpretation and HR recommendations

## Methods Used

- Mean vector analysis
- Covariance matrix
- Correlation matrix
- Standardization
- Mahalanobis distance
- Multivariate outlier detection
- Principal Component Analysis support
- Variance Inflation Factor support
- Hotelling T-squared tests
- Simultaneous confidence intervals
- Business-focused statistical interpretation

## Main Findings

The notebook reports several important conclusions:

- The average employee is approximately 37 years old, earns about $6,500 per month, and has about 7 years of tenure.
- Monthly income is right-skewed, suggesting a smaller group of highly compensated senior employees or specialists.
- Mahalanobis distance identified 70 multivariate outliers, approximately 4.8% of employees.
- The outliers are interpreted as meaningful workforce profiles rather than simple data errors.
- One-sample Hotelling T-squared testing suggests the workforce profile differs significantly from generic benchmark assumptions.
- Two-sample Hotelling T-squared testing shows statistically distinct multivariate profiles between employees who left and employees who stayed.
- Compensation-related variation appears to be a major source of uncertainty and retention risk.

## Strategic Recommendations

Based on the analysis, the project recommends:

- Building predictive attrition monitoring systems
- Creating targeted retention programs for high-value employees
- Replacing generic HR benchmarks with internal workforce analytics
- Using risk-aware compensation planning
- Expanding wellness and work-life programs
- Segmenting employees into strategic workforce groups
- Integrating HR analytics into executive decision-making
- Establishing continuous multivariate workforce monitoring

## Requirements

The notebook uses Python 3 and the following main libraries:

```text
kagglehub
matplotlib
numpy
pandas
scikit-learn
scipy
seaborn
statsmodels
```

Install the dependencies with:

```bash
pip install kagglehub matplotlib numpy pandas scikit-learn scipy seaborn statsmodels
```

## How to Run

1. Clone or download this repository.
2. Install the required Python packages.
3. Open the notebook in Jupyter Notebook, JupyterLab, VS Code, or Google Colab.
4. Run the notebook cells from top to bottom.

The notebook downloads the dataset automatically through KaggleHub. If Kaggle authentication is required in your environment, configure your Kaggle API credentials before running the data-loading cell.

## Repository Structure

```text
employee-attrition/
|-- README.md
`-- code/
    `-- MULTIVARIATE_STATISTICS__FINAL_PROJECT.ipynb
```

## Authors

Course: Multivariate Statistics

Team members:

- Ghada Essam Khalifa
- Nancy Youseef Zaher
- Sara Yehia Abdelaziz
- Omnya Mohamed Abdelfatah
- Menna Moamen Madani