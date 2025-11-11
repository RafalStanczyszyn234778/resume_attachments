# Wealth vs. Homicide Rate Dashboard

A data-driven interactive dashboard exploring the relationship between wealth indicators and homicide rates across countries and regions. Inspired by United Nations 17 Sustainable Development Goals.

[Open the Power BI report (interactive)](https://app.powerbi.com/view?r=eyJrIjoiNjk5OTBhN2UtNDlhYy00ZWRiLTlkZTEtNzYyZjU2ZTBmNjYwIiwidCI6IjBhMzM1ODliLTAwMzYtNGZlOC1hODI5LTNlZDA5MjZhZjg4NiIsImMiOjl9)

---

## Introduction

Homicide is widely recognized as a serious crime, yet its prevalence varies greatly around the world. In 2021:
- The Netherlands recorded a homicide rate of **0.65** per 100,000 people.
- Chile recorded a homicide rate of **3.63** per 100,000 people.

A common hypothesis is that wealthier societies experience lower homicide rates. This dashboard investigates whether and to what extent this correlation holds, and explores potential implications for policy.

---

## Research Questions

1. **Correlation Analysis**: What is the correlation between various wealth indicators (GDP per capita PPP, unemployment rate, poverty rate) and the homicide rate across countries?
2. **Impact of Poverty Reduction**: To what extent can a reduction in poverty lead to a decrease in homicides?

---

## Features & Overview

1. **Period & Country Selection**: Filter data by year range and specific country.
2. **Global & Regional Views**: Toggle between continent-level and world-level analyses.
3. **Correlation Coefficient**: View the Pearson correlation coefficient for the selected variables.
4. **Linear Regression**: Inspect linear regression plots with trend lines.
5. **Variable Comparison**: Switch among wealth measures (GDP per capita PPP, GDP per capita growth, poverty rate, unemployment rate) and compare them against homicide rate.

---

## Data Sources

1. **Homicide Rate (UNODC)**  
   https://ourworldindata.org/grapher/homicide-rate-unodc
2. **GDP per Capita, PPP (World Bank)**  
   https://data.worldbank.org/indicator/NY.GDP.PCAP.PP.CD
3. **Poverty Rate (Our World in Data)**  
   https://ourworldindata.org/grapher/share-of-population-in-extreme-poverty
4. **GDP per Capita Growth (Our World in Data)**  
   https://ourworldindata.org/grapher/gdp-per-capita-growth
5. **Unemployment Rate (Our World in Data)**  
   https://ourworldindata.org/grapher/unemployment-rate

---

## Considerations & Limitations

- **Data Gaps**: Many countries (especially in Africa) have limited or sporadic homicide data.
- **Data Quality Issues**: Some post-Soviet countries exhibit corrupted or inconsistent records.
- **Wealth Measures**: GDP-based indicators and poverty rates are imperfect proxies for "wealth." They may not capture income distribution (e.g., Gini index) or non-monetary aspects of well-being.
- **Regional Anomalies**: Some countries (e.g., Greece, Ireland) deviate from broader continental trends, suggesting local factors at play.
- **Additional Variables**: Incorporating metrics like the Gini coefficient or measures of societal health could enhance analysis.

---

## Summary & Key Findings

- **GDP per Capita (PPP)** shows a clear negative correlation with homicide rates in Europe and Asia, but this pattern weakens or reverses in Africa and North America. South American trends vary significantly by country.
- **GDP Growth** has little to no consistent correlation with homicide rates, suggesting short-term economic fluctuations do not drive homicide trends.
- **Poverty Rate** and **Unemployment Rate** exhibit mixed correlations: sometimes positive, sometimes negative, depending on the country and region. This undermines the stereotype that poverty universally predicts higher homicide.

**Implications:**  
- Policies aimed at raising per-capita wealth may reduce homicides in regions where a strong correlation exists (Europe, Asia).  
- In other regions, targeted studies should explore alternative drivers of violence (e.g., social, cultural, institutional factors).  
- Future research should incorporate finer-grained data (e.g., regional or community-level) and broader measures of inequality and societal well-being.

---

## How to Use the Dashboard

1. Select the **year range** using the timeline slider.
2. Choose a **specific country** or **continent** from the dropdown menu.
3. Toggle among wealth indicators with the category buttons.
4. View the **correlation coefficient** and **regression plot** below the charts.
5. Hover over data points for precise values and trend insights.

---

## License

This project is licensed under the MIT License. Feel free to use, adapt, and redistribute.

