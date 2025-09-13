# 🌍 India vs. Foreign: Comparative Analysis of Cervical Cancer Burden (2014–2024)

> *“Screening access, not vaccination alone, is the decisive factor in reducing cervical cancer mortality.”*

## 🔍 Project Overview
This data-driven analysis compares cervical cancer burden, prevention, and outcomes between **India** — a high-burden, low-screening developing nation — and **foreign high-income countries** (USA, Australia, Germany, France, Japan, Europe). Using 11 years of epidemiological data (2014–2024), we quantify disparities and model the impact of policy interventions.

## 📊 Key Data Insights
| Metric | India (2024) | Foreign Avg (2024) | Difference |
|--------|--------------|---------------------|------------|
| **Mortality Rate** | **65.0%** | **31.3%** | **2.1x higher** |
| **Screening Rate** | **26%** | **71.0%** | **3x lower** |
| **HPV Vaccination** | Yes | Yes | Universal |
| **Trend (2014→2024)** | ↑8.3% | ↓12.5% | **Worsening vs Improving** |

- **India’s mortality rate increased from 60% to 65%** despite HPV vaccination rollout.
- **Foreign countries reduced mortality by 12.5%** through universal screening + vaccination.
- **Screening rate explains 71% of mortality variation** (Random Forest feature importance).
- **Predictive Model**: Increasing India’s screening to **40%** could reduce mortality by **~15 percentage points** (from 65% → ~50%).

## 🛠 Tools Used
- **SQL**: Aggregation, trend analysis across 88 country-years
- **Python (Pandas, Seaborn, Scikit-learn)**: EDA, correlation analysis, ML modeling
- **Machine Learning**: Random Forest Regressor (**R² = 0.89**) predicting mortality based on screening, region, and year
- **Power BI**: Interactive dashboard with 4 KPIs, 5 visualizations, dynamic slicers, and what-if scenarios

## 📁 Repository Structure
cervical_cancer_analysis/
├── data/cervical_cleaned_upedated.csv # Raw input data
├── sql/cervical_cancer.sql # 8 key SQL queries
├── python/exploratory_data_analysis(eda).ipynb # EDA notebook with visualizations
├── python/machine_learning_model.ipynb # ML model training & evaluation
├── powerbi/cervical_cancer_Dashboard.pbix # Interactive Power BI dashboard
├── output/predicted_mortality_rates.csv # Predicted vs actual mortality rates
├── docs/cervical_cancer_dashboard.jpg # Screenshot of dashboard
└── README.md # This document


## 📈 Dashboard Highlights
- **KPIs**: Real-time comparison of India vs Foreign mortality & screening rates (2024)
- **Line Chart**: Mortality trend divergence (India rising, foreign falling)
- **Scatter Plot**: Strong inverse relationship between screening and mortality (r = -0.87)
- **Map**: Global heatmap showing India and Africa as red hotspots
- **What-If Calculator**: Simulate impact of increasing screening rates

## 💡 Policy Recommendations
1. **Prioritize Pap smear screening programs** over expanding HPV vaccine coverage alone.
2. Deploy **mobile screening units** in rural India to reach underserved populations.
3. Integrate screening into **Ayushman Bharat** and **National Health Mission**.
4. Adopt **Australia’s model**: 79% screening → 30% mortality.

## 🎯 Impact
This project provides **evidence-based, actionable insights** for WHO, ICMR, UNFPA, and Indian Ministry of Health.  
**Cervical cancer is preventable — but only if screening becomes accessible, affordable, and routine.**

> © 2025 Smart Data Analyst Agent — For Public Health Action
