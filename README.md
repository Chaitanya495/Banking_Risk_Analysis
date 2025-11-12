# Banking Risk Analysis

-Banking Dashboard Screenshot : path - Banking_Risk_Analysis/Images/Dashboard Screenshots

## Project Overview

This project analyzes a dataset of 3,000 banking customers to identify key risk and exposure drivers across financial products, client demographics, and banking relationships. It explores trends in credit behavior, loan deposits, risk weightings, and more to provide actionable insights for optimizing lending strategies, credit risk mitigation, and client segmentation.

The analysis is conducted using Python in a Jupyter Notebook, with data cleaning, exploratory data analysis (EDA), risk segmentation, outlier detection, and visualizations.

## Problem Statement

Analyze the bank's client portfolio data to identify key risk and exposure drivers across financial products, client demographics, and banking relationships. Uncover age-related trends, nationality-based patterns, and high-risk outliers in risk weightings. Align client profiles against loyalty classifications and fee structures to optimize lending strategies, credit risk mitigation, and client segmentation for enhanced financial stability and reduced portfolio concentration risk.

## Objectives

- Perform data profiling and cleaning to ensure accuracy.
- Explore key indicators like Credit Card Balance, Bank Loans, and Risk Weighting across demographics.
- Segment customers into risk tiers (low, medium, high) based on Risk Weighting.
- Detect outliers in credit and loan values to identify potential anomalies or fraud.
- Analyze correlations between exposures, risks, and client profiles.
- Deliver insights to improve banking strategies and reduce risks.

## Dataset Description

The dataset is stored in `Banking_data.xlsx` and includes the following sheets:

- **Banking**: Main client data with 3,000 rows and columns such as:
  - Client ID, Name, Age, Location ID, Joined Bank, Banking Contact, Nationality, Occupation, Fee Structure, Loyalty Classification, Estimated Income, Superannuation Savings, Amount of Credit Cards, Credit Card Balance, Bank Loans, Bank Deposits, Checking Accounts, Saving Accounts, Foreign Currency Account, Business Lending, Properties Owned, Risk Weighting, BRId (Banking Relationship ID), GenderId, IAId (Investment Advisor ID).
  
- **Gender**: Mapping of GenderID to Gender (e.g., 1: Male, 2: Female).

- **Banking Relationship**: Mapping of BRId to Banking Relationship (e.g., 1: Retail, 2: Institutional, 3: Private Bank, 4: Commercial).

- **Investment Advisor**: Mapping of IAId to Investment Advisor names.

The data spans years from 1995 to 2005 and includes financial metrics in USD (e.g., loans in billions, savings in millions).

**Note**: The dataset is truncated in some views, but the full Excel file is used for analysis.

## Tools and Technologies

- **Programming Language**: Python 3
- **Libraries**: 
  - Pandas (for data manipulation)
  - NumPy (for numerical computations)
  - Matplotlib and Seaborn (for visualizations)
  - SciPy/Statsmodels (for statistical analysis, if needed)
- **Environment**: Jupyter Notebook (`Banking_Risk_Analysis.ipynb`)
- **Data Source**: Excel file (`Banking_data.xlsx`)

## Analysis Steps

1. **Data Loading and Profiling**:
   - Loaded data from Excel using Pandas.
   - Checked for data types, missing values, duplicates, and basic statistics.
   - Handled cleaning: Standardized formats, filled missing values, removed duplicates.

2. **Exploratory Data Analysis (EDA)**:
   - Analyzed distributions of key variables (e.g., Age, Estimated Income, Risk Weighting).
   - Grouped data by demographics (e.g., Nationality, Gender, Occupation) and banking relationships.

3. **Risk Segmentation**:
   - Categorized customers into risk levels based on Risk Weighting (e.g., 1-5 scale).
   - Calculated exposure concentrations in each tier.

4. **Outlier Detection**:
   - Used Interquartile Range (IQR) to identify extreme values in loans, deposits, and credit balances.

5. **Correlation and Visualizations**:
   - Computed correlations between variables (e.g., Bank Deposits vs. Saving Accounts).
   - Created scatter plots with regression lines for pairs like:
     - Bank Deposits vs. Saving Accounts
     - Checking Accounts vs. Saving Accounts
     - Age vs. Superannuation Savings
     - Estimated Income vs. Checking Accounts
     - Bank Loans vs. Credit Card Balance
   - Dashboard views include pie charts for risk distributions, bar charts for deposits/loans by nationality/occupation, and key metrics like Total Clients (2,940), Avg Risk (2.25), Total Deposits ($3.77Bn).

6. **Insights Generation**:
   - Identified high-risk segments (e.g., 16.39% high-risk clients with $429.31M in high-risk loans).
   - Noted trends like higher risks in African nationalities (Avg Risk 2.29) and correlations between income and risk.

## Key Insights

- **Risk Distribution**: 40.73% of clients are at Risk Level 1 (low), but high-risk clients (Levels 4-5) drive 68% of total loan exposure.
- **Demographic Trends**: African nationalities show the highest average risk (2.29). Higher-income clients are 4x more likely to be high-risk.
- **Exposure Patterns**: Strong positive correlations between Bank Loans and Business Lending. Outliers in credit balances may indicate fraud risks.
- **Portfolio Concentration**: 16% of clients hold loans from $78K (low-risk) to $310K (high-risk), with a Risk LDR of 1.98.
- **Recommendations**: Focus on diversifying high-risk segments, enhancing monitoring for outliers, and tailoring products by occupation/nationality.

For detailed visuals, refer to the notebook or screenshots below:

![Summary Dashboard](images/summary-dashboard.png) <!-- Replace with your actual image path -->
![Deposit Analysis](images/deposit-analysis.png)
![Loan Deposit Analysis](images/loan-deposit-analysis.png)

## How to Run the Project

1. **Clone the Repository**:
