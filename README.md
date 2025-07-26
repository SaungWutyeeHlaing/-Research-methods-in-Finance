# -Research-methods-in-Finance
This is a group research project for a Finance Research Methods course. It applies panel data regression analysis using R to investigate the determinants of firm value in the Vietnamese trading sector.

This repository contains the R code for our **group research project** titled:

**"Determinants of Firm Value: An Empirical Analysis of Listed Trading Companies in the Vietnamese Market."**
Credit to the original owner of the research paper.
The project was completed as part of the **Research Method in Finance (B03021)** course during the 2024–2025 academic year at **Ton Duc Thang University**.
the following R code is created by reading the research paper and following the idea of the publisher. 

---

## Project Overview

- **Course**: Research Method in Finance – B03021  
- **Academic Year**: 2024–2025  
- **University**: Ton Duc Thang University   
- **Language**: English & Vietnamese (comments and data structure)  
- **Tools Used**: R, panel data models (FEM, REM), regression diagnostics  

---

## File Contents

Full R script used for:
  - Data cleaning and preparation  
  - Descriptive statistics and correlation analysis  
  - VIF test for multicollinearity  
  - Fixed effects and random effects panel regressions  
  - Hausman test for model selection  
  - Summary outputs using `stargazer`

---

## Methodology Summary

- **Regression model**:  
  `VAL = β0 + β1 * SIZE + β2 * CS + β3 * ROE + β4 * LIQUIDITY + u`

  Where:
  - **VAL**: Firm value  
  - **SIZE**: Firm size  
  - **CS**: Capital structure  
  - **ROE**: Return on equity  
  - **LIQUIDITY**: Liquidity  
  - **u**: Error term

- **Model estimation techniques**:
  - Fixed Effects Model (FEM)  
  - Random Effects Model (REM)  
  - Hausman Test for model appropriateness  
  - Diagnostic checks (VIF, correlation, R², p-values)

---

## Key Findings

- **Firm Size (SIZE)** has a strong positive impact on firm value  
- **Capital Structure (CS)** and **Liquidity** negatively affect firm value  
- **ROE** surprisingly shows a negative relationship in this sample  
- **Hausman Test** supports using the **Fixed Effects Model** over REM  

---

## R Packages Used

```r
plm       # Panel data modeling (FEM, REM)
sandwich  # Robust standard errors
lmtest    # Hypothesis testing
dplyr     # Data wrangling
psych     # Descriptive statistics
car       # VIF for multicollinearity
stargazer # Summary table output
