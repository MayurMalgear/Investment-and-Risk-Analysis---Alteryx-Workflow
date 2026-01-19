# Investment Performance and Risk Analysis Reporting
Automated financial workflow that processes transaction data, converts currencies, assesses risk, calculates rolling averages, and generates comprehensive PDF reports with investment performance, risk profiles, and regional summaries.

## 📘 Project Overview

This Alteryx Designer workflow automates the analysis and reporting of financial transaction data, focusing on investment performance, risk profiling, and regional transaction summaries. It transforms raw CSV data into a structured, multi-layered PDF report, enabling stakeholders to assess investment trends, risk exposure, and regional activity with clarity and precision.

## 🔄 Workflow Steps

<img width="940" height="503" alt="image" src="https://github.com/user-attachments/assets/2cff4046-0219-418e-b598-005473c24f9d" />


## 🚀 Features:

- Data Ingestion & Cleansing: Reads CSV data, infers data types, and cleanses records
- Currency Conversion: Converts GBP and EUR transactions to USD using fixed exchange rates
- Risk Categorization: Classifies transactions as 'High Risk' (score ≥ 7) or 'Low/Medium Risk'
- Rolling Averages: Calculates 3-period rolling averages of transaction amounts per account
- Multi-Path Analysis:
   - Investment Category & Regional Summaries
   - High-Risk Investment Details
- Automated Reporting: Generates a professional PDF report with:
   - Investment Category & Risk Profile Table
   - Regional Transaction Summary with Bar Graphs
   - Detailed High-Risk Investments Table

## 🛠️ Tools & Technologies

- Data Processing: Alteryx Designer (or similar workflow tool)
- File Format: CSV input, PDF output
- Key Operations:
  - Data type inference & cleansing
  - Formula-based transformations
  - Multi-row calculations
  - Data summarization & aggregation
  - Table formatting with visual elements
  - Report header creation & layout management

## 📈 Data Overview

The dataset contains financial transactions with the following columns:
  - Date: Transaction date
  - Account_ID: Unique account identifier
  - Region: Geographic region (APAC, UK, EU)
  - Currency: Transaction currency (USD, GBP, EUR)
  - Transaction_Type: Type of transaction (Buy, Sell, Deposit, Withdrawal)
  - Amount: Transaction amount in original currency
  - Risk_Score: Numeric risk assessment (1-10)
  - Investment_Category: Asset class (Equity, Bond, Forex, Commodity)

## 🔍 Insights Generated

  - Regional Performance: Which regions have highest transaction volumes?
  - Risk Distribution: How many transactions are high-risk?
  - Investment Preferences: Which categories dominate per region?
  - Currency Impact: How do exchange rates affect USD totals?
  - Temporal Trends: Rolling averages show transaction pattern stability

## 📝 Notes

  - Exchange rates are fixed (GBP: 1.25, EUR: 1.10) - update for real-time accuracy
  - Risk threshold set at ≥7 for "High Risk" - adjustable based on policy
  - Sample data contains 250+ transactions across 3 regions
  - Workflow is modular and extensible for additional analyses 
