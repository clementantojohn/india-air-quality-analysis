# 🌿 India Air Quality Analysis (2015–2020)

## 📌 Project Overview
This project analyses ambient air quality data across 26 major Indian cities 
from 2015 to 2020 using Microsoft Excel. The goal is to identify pollution 
trends, seasonal patterns, city-level disparities and key pollutant drivers 
of India's Air Quality Index (AQI).

---

## 📂 Dataset
- **Source:** [Kaggle — Air Quality Data in India](https://www.kaggle.com/datasets/rohanrao/air-quality-data-in-india)
- **Provider:** Central Pollution Control Board (CPCB), India
- **File Used:** city_day.csv
- **Time Period:** 2015 to 2020
- **Cities Covered:** 26 major Indian cities

---

## 🛠️ Tools Used
- Microsoft Excel — Data Cleaning, EDA, Charts, Dashboard

---

## 🧹 Data Cleaning Steps
- Identified and handled 88,488 blank cells across 16 columns
- Dropped columns with more than 50% missing data — PM10, NH3 and Xylene
- Filled numeric blank cells with column median — chosen over mean due to 
  right-skewed pollution data with extreme outliers
- Filled AQI_Bucket blanks using IF formula based on CPCB AQI thresholds —
  not estimated independently as it is a derived column
- Added Season column derived from Date column using IF and MONTH formula
- Documented all cleaning decisions in Data Cleaning Log

- ## 📦 Cleaned Dataset
Also available on Kaggle:
[India Air Quality — Cleaned Dataset](https://www.kaggle.com/datasets/clementantojohn/india-air-quality-analysis-20152020/data)

---

## 📊 Analysis Performed
- Descriptive Statistics — Mean, Median, Min, Max, Std Deviation
- City Rankings by Average AQI
- Yearly AQI Trend Analysis (2015–2020)
- Seasonal AQI Analysis — Winter, Summer, Monsoon, Post-Monsoon
- Pollutant Correlation Analysis with AQI

---

## 🔍 Key Findings

### 🔴 PM2.5 Crisis
- National average PM2.5 of 64.51 µg/m³ is **4× above WHO safe limit** of 15 µg/m³
- Maximum recorded value of 949.99 µg/m³ is 63× the safe limit

### 🏙️ City Rankings
- **Most Polluted:** Ahmedabad (AQI 339.86 — Severe category)
- **Cleanest:** Aizawl (AQI 36.24 — Good category)
- Clear North-South divide — all top 6 polluted cities are from North/Central India

### 📅 Yearly Trend
- Overall AQI improved 36.7% from 179.62 (2015) to 113.74 (2020)
- **2020 recorded sharpest single-year drop** — directly attributed to 
  COVID-19 lockdown halting factories and vehicles nationwide
- 2018 anomaly — AQI rose after 2017 improvement due to economic growth 
  surge and weak monsoon

### 🌡️ Seasonal Pattern
- **Most Polluted:** Winter (AQI 204.10) — temperature inversion traps pollutants
- **Second Most Polluted:** Post-Monsoon (AQI 201.52) — stubble burning season
- **Cleanest:** Monsoon (AQI 115.98) — rainfall washes pollutants naturally
- Winter and Post-Monsoon are separated by only 2.58 AQI points despite 
  completely different causes

### 🔗 Correlation Analysis
- **CO (r = 0.650)** — Strongest AQI driver — vehicular and combustion emissions
- **PM2.5 (r = 0.634)** — Second strongest — fine particulate matter
- **Benzene (r = 0.052)** — Negligible correlation — localised industrial source
- Vehicular emissions confirmed as the single highest-impact intervention target

---

## 📁 Excel File Structure

| Sheet | Description |
|---|---|
| Dashboard | One page summary of all key findings |
| city_day_RAW | Original unmodified Kaggle dataset |
| city_day_CLEAN | Cleaned and analysis-ready dataset |
| Blank % Analysis | Documentation of missing data by column |
| EDA_Summary | Descriptive statistics with observations |
| City_Analysis | City rankings by average AQI |
| Year_Analysis | Yearly AQI trend 2015 to 2020 |
| Seasonal_Analysis | AQI breakdown by season |
| Correlation_Analysis | Pollutant correlation with AQI |
| Charts | All visualisations |

---

## 💡 Conclusions
India's air quality data reveals a nation facing a serious pollution crisis 
driven primarily by vehicular emissions and seasonal factors. The COVID-19 
lockdown of 2020 demonstrated that human activity is directly responsible 
for a significant portion of pollution — AQI dropped 36.7% when activity 
halted. Targeted city-level and seasonal interventions — particularly 
addressing stubble burning and vehicular emissions — represent the highest 
impact opportunities for improvement.

---

## 👤 Author
**Clement Anto John**  
Aspiring Data/Business Analyst  
[GitHub](https://github.com/clementantojohn)
