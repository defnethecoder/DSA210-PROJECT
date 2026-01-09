**Defne Çatana – DSA210 Section D**

#  How Political and Economic Uncertainty Affects the Rise of Right-Wing Parties in Europe - DSA210 Project
---

## Project Overview

This project investigates how rising uncertainty levels measured through the World Uncertainty Index (WUI) correlate with the growing support for right-wing political parties across Europe over the last decade. By combining political, economic, and uncertainty data, this project aims to understand whether periods of heightened uncertainty, such as financial crises, migration surges, or geopolitical shocks, contribute to shifts in voter behavior toward right-wing parties.

---

## Objectives

1. Quantify political responses to uncertainty by examining whether increases in national uncertainty levels are associated with greater electoral support for right-wing and populist parties.

2. Identify economic amplifiers by evaluating whether macroeconomic conditions such as unemployment and inflation strengthen the relationship between uncertainty and right-wing voting behavior.

3. Explore migration and media effects to determine if migration inflows or public attention to immigration topics affect the political impact of uncertainty.

---

## Motivation

In recent years, Europe has faced multiple overlapping crises, such as the Eurozone debt crisis, refugee movements, Brexit, the pandemic, and ongoing geopolitical tensions. These events have generated unprecedented economic and informational uncertainty, reflected in both traditional media and public discourse.  

At the same time, right-wing and nationalist parties have seen growing support across many European countries. In this project, I aim to investigate whether there is a systematic statistical connection between these two phenomena, offering insights into how societies respond to instability. 

---

## Dataset

This project integrates multiple open datasets for a comprehensive analysis. Mentioned datasets are available under the file "data"

### 1. European Election Data (EED / ParlGov)
The European Election Database and ParlGov provide country-year-level election results across Europe.  
The dataset includes variables such as country, year, party name, vote share, and party family.  
It is used to measure right-wing vote share as the dependent variable.
Dataset Name: "Election.csv"

### 2. World Uncertainty Index (WUI)
The World Uncertainty Index, developed by Ahir, Bloom, and Furceri (IMF, 2024), is a text-based measure of national uncertainty extracted from Economist Intelligence Unit country reports.  
It includes country, quarter, and uncertainty index variables and covers the period 1996–2024 (converted to annual averages).  
The dataset is publicly available through the IMF.
Dataset Name: "WUI Europe (3).csv"

### 3. Enrichment Variables (migration rates)
The dataset is taken from EuroStat, which a statistics devolopment by EU. 
Dataset Name: "migration.csv"

---

## Hypothesis

The project tests whether uncertainty influences political outcomes.

**Main Hypothesis (H₁):**  
Higher uncertainty levels are associated with an increase in right-wing vote share.

**Null Hypothesis (H₀):**  
The World Uncertainty Index (WUI) has no significant effect on right-wing vote share.

**Extended Hypotheses:**  
The impact of uncertainty is increased in periods of high immigration.  
Immigration surges strengthen the uncertainty–right-wing relationship.

---

## Analysis Plan

1. **Data Cleaning and Preparation**  
   The datasets will be merged by country-year, missing values handled, and all variables normalized. Right-wing vote share ratios will be computed, and the uncertainty index will be log-transformed for scaling.

2. **Exploratory Data Analysis (EDA)**  
   Trends between WUI and right-wing vote share will be visualized over time. Correlation matrices and time-series heatmaps will be created to identify co-movements. Key temporal spikes such as the 2015 migration crisis and 2020 pandemic will be highlighted.

3. **Hypothesis Testing**  
   Fixed-effects regression models will be used to estimate the relationship between uncertainty and right-wing voting. Also to see a relationship between voter behavior and migration/ representation on media.

4. **Visualization and Interpretation**  
   Results will be presented through line charts showing the evolution of uncertainty and vote share, geographic heatmaps showing regional variation, and feature importance plots summarizing machine learning results.

---

## Findings and Insights

Preliminary findings suggest that periods of high uncertainty are consistently associated with increases in right-wing vote share, particularly in Southern and Eastern Europe.   
Migration spikes, such as those during 2015–2016, coincide with both higher uncertainty and right-wing electoral surges.  

---

## Limitations

The quarterly nature of the WUI data and the irregular timing of elections require data aggregation, which may affect short-term effects.  
There is also potential endogeneity: political shifts toward the right could themselves increase perceived uncertainty.  
Defining “right-wing” parties consistently across countries is challenging due to ideological variation.
2025 data are unavailable and in WUI Europe data, it is the most "uncertain" year to analyze.




