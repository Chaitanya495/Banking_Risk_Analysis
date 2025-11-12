# 📊 Banking Risk Analysis Dashboard

## 🧠 Overview

The Banking Risk Analysis Dashboard is a Python-based project designed to analyze a bank's client portfolio and identify key risk and exposure drivers across financial products, client demographics, and banking relationships.

It provides actionable insights on credit behavior, loan exposures, risk weightings, and client segmentation, helping banks optimize lending strategies, mitigate credit risks, and manage portfolio concentration effectively.

## 🚀 Key Features
- 📈 **Risk Distribution Analysis** – Visualizes customer distribution across risk levels (low, medium, high) and highlights exposure concentration.
- 📊 **Demographic Insights** – Examines trends based on nationality, age, occupation, and gender to uncover high-risk segments.
- 💳 **Financial Product Exposure** – Analyzes Credit Card Balances, Bank Loans, Deposits, and Business Lending patterns.
- 🔍 **Outlier Detection – Identifies** extreme values in loans, deposits, and credit balances using IQR for anomaly or fraud detection.
- 🧭 **Correlation & Trend Analysis** – Explores relationships between income, savings, deposits, loans, and risk weightings.
- 🖼️ **Interactive Visualizations** – Includes scatter plots, bar charts, pie charts, and key metrics for intuitive insights.

## 🧩 Dataset Information
The dataset Banking_data.xlsx contains three sheets:
1. Banking :

*Main client data (3,000 rows) including:*

- **Client ID**
- **Name**
- **Age**
- **Location**
- **Joined Bank**
- **Banking Contact**
- **Nationality**
- **Occupation**
- **Fee Structure**
- **Loyalty Classification**
  
*Financial metrics:*

- **Estimated Income**
- **Superannuation Savings**
- **Credit Card Balance**
- **Bank Loans**
- **Deposits**
- **Accounts**
- **Business Lending**
- **Properties Owned**
- **Risk Weighting**
- **BRId (Banking Relationship ID)**
- **GenderId**
- **IAId (Investment Advisor ID)**

2. Gender : Mapping of GenderId to Gender (e.g., 1: Male, 2: Female)
3. Banking Relationship : Mapping of BRId to Banking Relationship (Retail, Institutional, Private Bank, Commercial)
4. Investment Advisor : Mapping of IAId to advisor names

The dataset spans 1995–2005 and financial metrics are in USD (loans in billions, savings in millions).

## ⚙️ Tools & Technologies
- **Power BI Desktop**
- **Power Query (Data Transformation)**
- **DAX (Data Analysis Expressions)**
- **Data Visualization and Modelling**
- **Python 3**
- **Google Colab**
- **Libraries: Pandas, NumPy, Matplotlib, Seaborn, SciPy/Statsmodels**


## 📊 Insights Highlighted
- Risk Concentration: 40.73% of clients are low-risk, but high-risk clients (16.39%) account for 68% of total loan exposure.
- Demographic Patterns: African nationalities show the highest average risk (2.29). High-income clients are 4x more likely to be high-risk.
- Exposure Correlations: Strong positive correlation between Bank Loans and Business Lending; outliers may indicate fraud risk.
- Portfolio Concentration: Certain clients hold loans ranging from $78K (low-risk) to $310K (high-risk), with a Risk LDR of 1.98.
- Recommendations: Diversify high-risk segments, monitor outliers, and tailor banking products by occupation and nationality.


## 🖼️ Dashboard Preview
https://app.powerbi.com/links/Hy1EBB-O3c?ctid=33e01945-42fa-4a16-9451-0300635b5524&pbi_source=linkShare
