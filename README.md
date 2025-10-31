**Defne Çatana – DSA210 Section D**

# Europe’s Right-Wing Rise and Word Uncertainty Index (WUI)

---

## Project Overview

This project investigates how rising uncertainty levels measured through the World Uncertainty Index (WUI) correlate with the growing support for right-wing political parties across Europe over the last decade.

By combining political, economic, and text-based uncertainty data, the project aims to understand whether periods of heightened uncertainty, such as financial crises, migration surges, or geopolitical shocks, contribute to shifts in voter behavior toward right-wing parties.

This analysis integrates political science and data science through the use of panel datasets, hypothesis testing, and machine learning models to quantify how uncertainty and macroeconomic indicators shape electoral outcomes.

---

## Objectives

1. Quantify political responses to uncertainty by examining whether increases in national uncertainty levels are associated with greater electoral support for right-wing and populist parties.

2. Identify economic amplifiers by evaluating whether macroeconomic conditions such as unemployment and inflation strengthen the relationship between uncertainty and right-wing voting behavior.

3. Explore migration and media effects to determine if migration inflows or public attention to immigration topics amplify the political impact of uncertainty.

---

## Motivation

In recent years, Europe has faced multiple overlapping crises — the Eurozone debt crisis, refugee movements, Brexit, the pandemic, and ongoing geopolitical tensions. These events have generated unprecedented economic and informational uncertainty, reflected in both traditional media and public discourse.  

At the same time, right-wing and nationalist parties have seen growing support across many European democracies. This project aims to investigate whether there is a systematic statistical connection between these two phenomena, offering insights into how societies respond to instability.

Understanding these dynamics benefits political scientists studying voter polarization and populism, economists modeling uncertainty shocks, and policy-makers designing stability-oriented interventions.

---

## Dataset

This project integrates multiple open datasets for a comprehensive analysis.

### 1. European Election Data (EED / ParlGov)
The European Election Database and ParlGov provide country-year-level election results across Europe.  
The dataset includes variables such as country, year, party name, vote share, and party family.  
It is used to measure right-wing vote share as the dependent variable.

### 2. World Uncertainty Index (WUI)
The World Uncertainty Index, developed by Ahir, Bloom, and Furceri (IMF, 2024), is a text-based measure of national uncertainty extracted from Economist Intelligence Unit country reports.  
It includes country, quarter, and uncertainty index variables and covers the period 1996–2024 (converted to annual averages).  
The dataset is publicly available through the IMF.

### 3. Enrichment Variables
To strengthen the analysis, several additional datasets are used:
- From the World Bank and Eurostat: GDP growth, unemployment rate, inflation rate, and Gini index to control for economic conditions.
- From UNHCR and Eurostat: net migration rate and asylum application numbers to capture migration intensity.
- From Google Trends and the European Social Survey (ESS): indicators such as search interest in “immigration”, “security”, or “economy” topics to measure media attention and social sentiment.

---

## Hypothesis

The project tests whether uncertainty influences political outcomes.

**Main Hypothesis (H₁):**  
Higher uncertainty levels are associated with an increase in right-wing vote share.

**Null Hypothesis (H₀):**  
The World Uncertainty Index (WUI) has no significant effect on right-wing vote share.

**Extended Hypotheses:**  
- The impact of uncertainty is amplified in periods of high unemployment.  
- Immigration surges strengthen the uncertainty–right-wing relationship.

These hypotheses are tested using panel regression, correlation, and fixed-effects models.

---

## Analysis Plan

1. **Data Cleaning and Preparation**  
   The datasets will be merged by country-year, missing values handled, and all variables normalized. Right-wing vote share ratios will be computed, and the uncertainty index will be log-transformed for scaling.

2. **Exploratory Data Analysis (EDA)**  
   Trends between WUI and right-wing vote share will be visualized over time. Correlation matrices and time-series heatmaps will be created to identify co-movements. Key temporal spikes such as the 2015 migration crisis and 2020 pandemic will be highlighted.

3. **Hypothesis Testing**  
   Fixed-effects regression models will be used to estimate the relationship between uncertainty and right-wing voting. Interaction terms such as “uncertainty × unemployment” will be added to test moderating effects. Significance will be evaluated using p-values and R² metrics.

4. **Machine Learning Models**  
   A Random Forest Regressor will be trained to predict right-wing vote share using variables such as uncertainty index, unemployment rate, migration rate, GDP growth, and inflation rate. SHAP analysis will be used to interpret feature importance.

5. **Visualization and Interpretation**  
   Results will be presented through line charts showing the evolution of uncertainty and vote share, geographic heatmaps showing regional variation, and feature importance plots summarizing machine learning results.

---

## Findings and Insights

Preliminary findings suggest that periods of high uncertainty are consistently associated with increases in right-wing vote share, particularly in Southern and Eastern Europe.  
Economic conditions appear to amplify this relationship — unemployment and inflation intensify the effects of uncertainty on voting behavior.  
Migration spikes, such as those during 2015–2016, coincide with both higher uncertainty and right-wing electoral surges.  





