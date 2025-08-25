# Econometrics-EU-Trade
Econometrics project on trade, crises and inequality in the European Union

## Introduction
In a context of globalization, international trade plays a central role in economic growth and development, shaping wealth distribution and poverty reduction. However, crises such as the Eurozone debt crisis or the COVID-19 pandemic disrupt this process, affecting exports and widening inequality.  

This project investigates how **exports influence economic and social development in the EU (2010–2023)**, focusing on growth, poverty, and inequality, and how these effects are conditioned by crisis periods.

## Literature Review
Previous research has shown mixed results:
- **Trade openness and growth** → Frankel & Romer (1999), Crespo-Cuaresma et al. (2008) highlight positive effects of exports on GDP per capita.  
- **Trade and inequality** → Helpman, Itskhoki & Redding (2010) argue trade can increase wage inequality in developed economies.  
- **Trade and poverty** → Dollar & Kraay (2004), Winters et al. (2004) show trade can reduce poverty if supported by strong institutions and social policies.  
- **Impact of crises** → Baldwin & Tomiura (2020), Berthou et al. (2022) underline how shocks disproportionately harm vulnerable groups, amplifying inequality.  

## Data
We used **World Bank Open Data (2010–2023)** as the main source.  

**Indicators included:**
- GDP growth (% annual)  
- Exports of goods and services (% annual growth)  
- Gini index (income inequality)  
- Poverty headcount ratio ($2.15/day, 2017 PPP)  

The raw datasets were downloaded from the [World Bank Data Catalog](https://datacatalog.worldbank.org/) and merged into a single CSV file to facilitate the analysis.

## Key Findings / Conclusion
- Export growth is positively associated with GDP growth in the EU.  
- Economic crises (2012 Euro crisis, 2020 COVID-19) reduced GDP, showing strong negative shock effects.  
- The interaction between exports and crises suggests that trade plays an even more important role during crises.  
- Higher inequality (Gini index) negatively impacts GDP growth.  
- Robustness tests (Chow, Breusch-Pagan, White, AIC/BIC) confirm that **2020 represented a structural break**, and Model 4 (with inequality and poverty) had the best fit.  
- Overall, exports are a crucial driver of EU economic growth, especially in crisis periods, but international trade alone has **limited impact on reducing poverty and inequality**. Social investment (e.g., education) is necessary to complement trade benefits.  

## Methods
- Data cleaning and visualization in **R**  
- **Econometric models**: panel data regression, heteroskedasticity tests, structural break analysis  
- Model comparison using AIC/BIC  

## Repository Structure
- `trade_analysis.R` → main R script with data analysis and econometric models  
- `eu_trade_inequality.csv` → merged dataset created from World Bank indicators  
- `README.md` → project documentation  

##  Authors
- Diana Borges  
- João Duarte  
- Maria Eduarda Ferreira  
- Rafael Ferreira  

