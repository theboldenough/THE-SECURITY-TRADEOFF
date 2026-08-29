# THE-SECURITY-TRADEOFF
Power BI analysis of military expenditure, peace and terrorism outcomes across 143 countries, 2020–2025.
# The Security Trade-Off

## Military Expenditure, Peace & Terrorism | 2020–2025

## 📌 Project Overview

The Security Trade-Off is a data analytics project built in Power BI to explore the relationship between changes in military expenditure, peace and terrorism-related outcomes across countries between 2020 and 2025.

The project integrates military expenditure, peace, terrorism and population data to identify patterns in how security indicators changed over the five-year period.

The final analysis contains comparable 2020–2025 observations for 143 countries.

---

## 🎯 Analytical Question

> Does increased military expenditure correspond with improved peace and terrorism outcomes?

The project focuses on identifying relationships and patterns rather than establishing causation.

---

## 📊 Data Sources

The analysis combines four datasets:

- SIPRI Military Expenditure
- Global Peace Index (GPI)
- Global Terrorism Index (GTI)
- Population data

---

## 🧹 Data Preparation

The datasets were cleaned and integrated before visualization.

Key preparation steps included:

- Standardizing country names
- Standardizing year formats
- Matching countries using ISO3 codes where available
- Merging datasets using country-year identifiers
- Checking for duplicate country-year combinations
- Handling missing observations
- Calculating population-normalized terrorism fatalities
- Calculating 2020–2025 changes
- Creating combined security outcome profiles

The merged master dataset contained 922 rows and 12 columns.

There were 0 duplicate ISO3-Year combinations.

After accounting for missing values, 143 countries had usable observations for the final 2020–2025 comparison.

---

## 📐 Key Metrics

### Military Spending Change

Military expenditure change was calculated as the percentage difference between 2020 and 2025.

### Peace Change

Peace outcomes were evaluated using changes in Global Peace Index scores between 2020 and 2025.

### Terrorism Fatalities per Million

Terrorism fatalities were normalized by population to make comparisons between countries of different population sizes more meaningful.

---

## 🔐 Security Outcome Profiles

Countries were classified into six combined peace and terrorism outcome profiles:

| Profile | Description |
|---|---|
| DP/ST | Deteriorated Peace / Stable Terrorism |
| IP/ST | Improved Peace / Stable Terrorism |
| IP/IT | Improved Peace / Improved Terrorism |
| DP/DT | Deteriorated Peace / Deteriorated Terrorism |
| DP/IT | Deteriorated Peace / Improved Terrorism |
| IP/DT | Improved Peace / Deteriorated Terrorism |

Final distribution:

| Security Profile | Countries |
|---|---:|
| Deteriorated Peace / Stable Terrorism | 55 |
| Improved Peace / Stable Terrorism | 44 |
| Improved Peace / Improved Terrorism | 14 |
| Deteriorated Peace / Deteriorated Terrorism | 13 |
| Deteriorated Peace / Improved Terrorism | 13 |
| Improved Peace / Deteriorated Terrorism | 4 |

---

## 📈 Power BI Dashboard

The dashboard contains three analytical pages:

### 1. Global Overview

Provides a high-level view of:

- Countries analyzed
- Average military spending change
- Average terrorism fatalities per million
- Total 2025 military expenditure
- Security profile distribution

### 2. Security Outcomes

Examines:

- Peace and terrorism outcome profiles
- Peace vs terrorism changes
- Military spending change vs peace change

### 3. Military Investment

Examines:

- Top military spenders
- 2020 vs 2025 expenditure
- Largest military spending increases
- Largest military spending decreases

---

## 🔎 Key Findings

- The final analysis covers 143 countries with comparable 2020–2025 observations.
- 81 countries experienced deteriorated peace outcomes, while 62 experienced improved peace outcomes.
- 55 countries were classified as Deteriorated Peace / Stable Terrorism.
- Military expenditure changes varied substantially across countries.
- Countries with the largest military budgets were not necessarily the countries with the largest percentage increases.
- Increased military expenditure did not consistently correspond with improved peace outcomes.

---

## ⚠️ Limitations

This project identifies associations and patterns rather than causal relationships.

Military expenditure cannot be interpreted as directly causing changes in peace or terrorism outcomes. Other factors such as armed conflict, political instability, governance, economic conditions and regional security dynamics can influence these indicators.

---

## 🛠️ Tools & Technologies

- Python
- Pandas
- Google Colab
- Microsoft Power BI
- Data Cleaning
- Data Transformation
- Data Visualization
- Exploratory Data Analysis

---

## 📁 Project Structure

```text
The-Security-Tradeoff/
│
├── README.md
│
├── data/
│   └── Security_Tradeoff_PowerBI.csv
│
├── powerbi/
│   └── The_Security_Tradeoff.pbix
│
├── dashboard/
│   └── The_Security_Tradeoff.pdf
│
└── screenshots/
    ├── global_overview.png
    ├── security_outcomes.png
    └── military_investment.png
