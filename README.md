# Used Cars Data Analysis

Understanding the factors that influence the price of used cars is crucial for both buyers and sellers. This project explores a dataset of used cars to determine which characteristics most impact pricing, helping users make more informed decisions.

## Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Data Cleaning](#data-cleaning)
- [Analysis Workflow](#analysis-workflow)
- [Key Findings](#key-findings)
- [Visualizations](#visualizations)
- [How to Reproduce](#how-to-reproduce)
- [References](#references)

## Overview

This project analyzes a dataset of used cars to uncover insights into how various features—such as fuel type, horsepower, and other characteristics—affect their market price. The analysis is done in Python using Pandas and other data science libraries.

## Dataset

- **Source:** [IBM SkillBuild](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0101EN-SkillsNetwork/labs/Data%20Files/auto.csv)
- **File Name:** `usedcars.csv`
- The dataset includes details such as make, fuel-type, body-style, horsepower, and price.

## Data Cleaning

The dataset contains missing values, indicated by `'?'`. The following cleaning steps were performed:
1. **Replace Missing Values:** All `'?'` entries were converted to `NaN` (Not a Number).
2. **Data Type Conversion:** Columns were converted to appropriate types (e.g., numeric for price and horsepower).
3. **Handle Missing Data:** Rows with critical missing values were handled through imputation or removal.

## Analysis Workflow

1. **Exploratory Data Analysis (EDA):** Statistics and distributions of key features.
2. **Data Transformation:** Categorical variables such as `fuel-type` were converted to dummy variables using `pd.get_dummies()`.
3. **Data Visualization:** Created plots (histograms, boxplots) to visualize distributions and relationships.
4. **Feature Engineering:** Binned continuous variables like `horsepower` for deeper insights.
5. **Modeling:** Analyzed relationship between features and price using correlation and regression (if applicable).

## Key Findings

- Most used cars have lower horsepower, with only a few high-powered outliers.
- Certain features, such as fuel type and body style, have noticeable impacts on price.
- Data cleaning and transformation significantly improved analysis accuracy.

## Visualizations

Below is an example of binning the `horsepower` category:

![Horsepower Binning](https://github.com/user-attachments/assets/e4ea9201-7242-44c3-9767-8ebdce18835d)

Histogram of horsepower distribution:

![Horsepower Histogram](https://github.com/user-attachments/assets/9a693b6b-386f-4fbc-93b1-5f8a1dcde5b5)

*Figure 1: Most used cars have a low level of horsepower, while very few have high horsepower.*

## How to Reproduce

1. Clone this repository.
2. Install required libraries:
   ```bash
   pip install pandas numpy matplotlib seaborn
   ```
3. Run the analysis scripts (replace `analysis.py` or `notebook.ipynb` with actual file names if different):
   ```bash
   python analysis.py
   ```
   or open and run the Jupyter notebook.

## References

- Dataset: [IBM SkillBuild auto.csv](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0101EN-SkillsNetwork/labs/Data%20Files/auto.csv)

---

*If you have any questions or suggestions, feel free to open an issue or contribute!*
